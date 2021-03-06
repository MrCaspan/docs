---
title: Permissions
tags:
- Developers
- Framework
category: developer
menu:
  developer:
    parent: framework
    weight: 10
aliases:
- /developers/framework/permissions
---
## Permissions Overview

Vanilla uses permissions to restrict access to particular content, options, or workflows. There are a number of functions built into the framework to do this efficiently. We eschew role-detection as a means of access control. 

For example, we would never check to make sure someone was in a role named Moderator before granting access to an option, we would check a permission like `Garden.Moderation.Manage`.

### Naming Permissions

We use the same dot notation syntax for permissions as we do for config settings. A typical scheme would be: `Namespace.Keyword.Action`.

For instance, look at `Vanilla.Discussions.Add`. This permissions is registered by the Vanilla application, is related to discussions, and is specifically for adding.

For the Namespace (first dot tier), use the slug name of your addon. The `Plugins` namespace is deprecated.

The Keyword (second dot tier) should be the most concise description possible of the part of the addon it governs.

Whenever possible, use one of the following as your Action (third dot tier): 

* Add
* Edit
* View
* Manage
* Delete

Other action names are avoided and may be renamed or refactored out of the framework in the future. However, they are not forbidden and never will be.

### Using Permissions

There are two basic ways to check a permission. One is to use a true/false conditional, typically to `checkPermission()` in an `if` statement:

```
if (checkPermission('Permission.Name')) {
    // Do something special
}
```
The other is to wholesale block execution by a call to `Gdn::session()->permission()`. This method automatically triggers a permission exception:

```
public function Index() {
    Gdn::session()->permission('Permission.Name');
    // Do priviliged things safely now
}
```
Typically we don't use the first convention to trigger a permission exception manually because the second will cover it.

### Multiple Permissions

You can use either method above to check multiple permissions by passing an array of permission names as the first parameter.

By default, it will require ALL permissions named to pass. If you pass a second parameter of `false`, then only ONE of the permissions is needed to pass.

You may find additional permission checks in Vanilla for permission names that do not appear in the Dashboard using this style: a normal permission name is passed in an array along with an "invisible" one. This is to allow plugins to define the additional permissions for more granular checks if needed.

### The Owner Flag

The forum owner's account (the one you create when installing Vanilla) gets a special flag set on it. This is accomplished by setting the `Admin` column equal to `1` in the `User` table.

Accounts with this flag set bypass all permission checks. `checkPermission` will always return `true` and no permission exception will ever be thrown for it. It will do this regardless of any role assignment.

For this reason, it is extremely important to test your addons with a non-owner account to see your permission checks in action.

### The System Flag

The System account is generated for general use by addons and cases where content must be generated by the forum. This account is designated by setting the `Admin` column equal to `2` in the `User` table.

This grants the same privileges as the Owner flag, and protects the account from deletion or banning.

### Reversed Permission

A special case in the framework is the `Vanilla.Approval.Require` permission. It is checked with the `checkRequirement` function. A `true` result means their content must go to the Moderation queue for approval. Therefore, a `true` result actually grants you _less_ permission. We don't generally recommend using this construct.
