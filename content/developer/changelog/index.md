---
title: Change Log
tags:
- Developers
- Changes
- Bug fixes
- Security
category: developer
menu:
  developer:
    identifier: changelog
aliases:
- /developers/changelog
---

This is for packaged, gold releases of the self-hosted product. We publish beta and release candidate change logs on the [forum](https://open.vanillaforums.com/categories/blog). We provide separate [cloud release notes](http://docs.vanillaforums.com/help/releases/) since they are scheduled differently.

Vanilla numbers major releases with the first decimal place. A second decimal indicates a minor patch release.

## 2.8.x

- Rich Editor is the new default editor.
- Keystone is the new default desktop & mobile (responsive theme)
- Numerous bug-fixes and security patches
- The full feature list and details can be found on [the 2.8 release notes discussion](https://open.vanillaforums.com/discussion/37120/vanilla-2-8-release-notes).

### 2.8.0

* [Released 7 February 2019](https://open.vanillaforums.com/discussion/36983/vanilla-2-8-is-now-available)

### 2.8.1

* [Released 15 March 2019](https://open.vanillaforums.com/discussion/37121/vanilla-2-8-1-is-now-available-security-patches-bug-fixes)

### 2.8.2

There was an error while creating this release so it was never distributed.

### 2.8.3

* [Released 23 April 2019](https://open.vanillaforums.com/discussion/37245/vanilla-2-8-3-is-now-available-for-download-security-patches)

### 2.8.4

* [Released 4 June 2019](https://open.vanillaforums.com/discussion/37347/vanilla-2-8-4-is-now-available-for-download-important-security-patches)

## 2.7.x

_Vanilla 2.7 was only distributed to Vanilla Cloud. The accumulated open source release notes from this release are incorporated into the [the 2.8 release notes discussion](https://open.vanillaforums.com/discussion/37120/vanilla-2-8-release-notes)._

## 2.6.x

_Vanilla 2.6 is the first version of Vanilla that requires PHP 7.0._

New Features:

- Category Following
- API v2 In-Dashboard Docs
- API v2 Changes and Additional Endpoints
- Numerous bug-fixes and security patches
- The full feature list and details can be found on [the 2.6 release announcement and discussion](https://open.vanillaforums.com/discussion/comment/252706/#Comment_252706).

### 2.6.0

*[Released 14 May 2018](https://open.vanillaforums.com/discussion/36260/vanilla-2-6-is-here-includes-security-fixes)*

## 2.5.x

_Vanilla 2.5 is the last version of Vanilla that supports PHP 5.6. As such many additional security fixes have been backported to this release. If you cannot currently run a later version of Vanilla, be sure to run the latest 2.5 patch release._

Highlights of this released include:

- Dashboard Redesign
- Flat categories
- Native API (APIv2)
- Full IPv6 support.

A full feature list can be found on [the 2.5 release schedule and features discussion](https://open.vanillaforums.com/discussion/34616/vanilla-2-5-release-schedule-features).

### 2.5.2

*[Released 14 May 2018](https://open.vanillaforums.com/addon/vanilla-core-2.5.2)*

### 2.5.1

*[Released 12 Feb 2018](https://open.vanillaforums.com/discussion/35925/vanilla-2-5-1-now-available-security-update)*

### 2.5.0

*[Released 23 Dec 2017](https://open.vanillaforums.com/discussion/35687/vanilla-2-5-is-now-available)*

## 2.4.x

A full vanilla 2.4 version was never released. Instead, [Release 2.5](#2-5) was branched. A [beta was distributed]((https://open.vanillaforums.com/discussion/33066/preview-release-2-4-beta)), but a full version was never released.

## 2.3.x

*[Released 18 Nov 2016](https://open.vanillaforums.com/discussion/32822/vanilla-2-3-is-now-available)*

## 2.2.x
### 2.2.1

*[Released 7 May 2016](https://open.vanillaforums.com/discussion/32109/vanilla-2-2-1-now-available)*

### 2.2

*[Released 12 Nov 2015](https://open.vanillaforums.com/discussion/31121/vanilla-is-proud-to-present-version-2-2)*

## 2.1.x
### 2.1.13

*[Released 29 Oct 2015](https://open.vanillaforums.com/discussion/31046/vanilla-2-1-13-security-updates)*

### 2.1.12

*[Released 15 Oct 2015](https://open.vanillaforums.com/discussion/30966/vanilla-2-1-12-released-security-update)*

### 2.1.11

*[Released 12 June](https://open.vanillaforums.com/discussion/30123/vanilla-2-1-11-released-security-patch)*

### 2.1.10

*[Released 4 May 2015](https://open.vanillaforums.com/discussion/29835/vanilla-2-1-10-released-critical-security-update)*

### 2.1.9

*[Released 18 Mar 2015](https://open.vanillaforums.com/discussion/29555/vanilla-2-1-9-released)*

### 2.1.8

*[Released 15 Jan 2015](https://open.vanillaforums.com/discussion/29016/critical-vanilla-2-1-8-released)*

### 2.1.7

*[Released 9 Jan 2015](https://open.vanillaforums.com/discussion/28961/vanilla-2-1-7-released)*


### 2.1.6

*[Released 21 Nov 2014](https://open.vanillaforums.com/discussion/28555/vanilla-2-1-6-released)*

* Security: Fixes an SQL injection vector.
* Security: Adds a PDO option to harden against SQL injection.
* Security: Improves the security of password resets by increasing token length and limiting them to 1 hour expiration.
* Adds vBulletin 5.1 password hashing to allow seamless password migrations. All previous versions continue to be supported.

### 2.1.5

*[Released 31 Oct 2014](https://open.vanillaforums.com/discussion/28337/vanilla-2-1-5-released-and-2-0-18-14)*

* Security: An Insecure Direct Object Reference was fixed that allowed unauthorized comment editing.
* Security: Potential CSRF vectors were closed, including one that could allow account hijacking.
* Fixes issue where enabling cleditor would permanently allow style parameter in comments.
* Fixes issue notifying users of new comments in certain cases where they did not have permission to then view them.
* Fixes OpenID bug effecting Google Sign In.
* Multiple community-contributed bug fixes.
* 2.1.4 had a merge conflict which this release replaced.

### 2.1.3

*[Released 9 Sept 2014](https://open.vanillaforums.com/discussion/27822/vanilla-2-1-3-security-release)*

* 3 newly discovered XSS vectors were fixed.
* The timezone bug introduced in 2.1.1 is fixed.
* Fixes invalid DeliveryType in plugins management.
* 2.1.2 had a Javascript error which this release replaced.

### 2.1.1

*[Released 2 Aug 2014](https://open.vanillaforums.com/discussion/27540/vanilla-2-1-1-important-security-bug-release)*

* HtmLawed was upgraded to close an XSS vector (thanks to Psych0tr1a for responsibly disclosing this to us & to HtmLawed for a fast patch in response).
* Multiple XSS exploits were fixed (thanks to @x00 for responsibly disclosing and both he and @businessdad for assistance in making our patches as bulletproof as possible).
* Fixed a Twitter SSL bug (thanks @Adrian for the patch).
* Fixed a missing permission check in the sorting utility (thanks @R_J for the patch).
* cleditor was patched to fix a crippling IE11 bug.
* Profile Extender was upgraded and a security flaw in it was fixed.
* Fixed a bug in Announcing while starting a discussion.
* Corrected the default theme README.
* Backported GDN_UserAuthenticationProvider.IsDefault so the latest version of jsConnect will work with 2.1.1.
* Fixes a theme screenshot bug (thanks @hgtonight‌ for the patch).

### 2.1

*[Released 28 April 2014](https://open.vanillaforums.com/discussion/26685/vanilla-2-1-stable-released)*

Vanilla internals were completely revamped for 2.1. Many views and several plugin hooks were changed, so **themes and plugins must be tested** and may need to be refactored before upgrading.

* Better localization support.
* Improved embedding.
* Performance and caching enhancements.
* Revamped Activity structure.
* Framework improvements.
* Hundreds of bug fixes.

Incremental changelogs from the [first 2.1 beta](https://open.vanillaforums.com/discussion/23322/vanilla-2-1b1-released) through RC1 can be found in their individual release announcements:

* [Beta 2](https://open.vanillaforums.com/discussion/24845/vanilla-2-1b2-released)
* [Beta 3](https://open.vanillaforums.com/discussion/26518/vanillla-2-1-beta-3)
* [Release Candidate 1](https://open.vanillaforums.com/discussion/26626/vanilla-2-1-release-candidate)

## 2.0.x

### 2.0.18.14

***Prior to 2.1, Vanilla used the third decimal in the version to indicate new features, and a fourth decimal for minor patches.***

*[Released 30 Oct 2014](https://open.vanillaforums.com/discussion/28337/vanilla-2-1-5-released-and-2-0-18-14)*

* Security: An Insecure Direct Object Reference was fixed that allowed unauthorized comment editing.
* Security: Potential CSRF vectors were closed, including one that could allow account hijacking.
* Fixes DeliveryType issue in plugins managements.

### 2.0.18.13

*[Released 5 Aug 2014](https://open.vanillaforums.com/discussion/27541/vanilla-2-0-18-13-security-release-for-old-2-0-18-installs)*

* HtmLawed is upgraded and its filtering tightened (thanks @x00 & Psych0tr1a)
* parseJSON() is substituted for eval() in 2 places
* Refactored the definitions list into Javascript instead of using the DOM
* Fixes HTMLawed error in 2.0.18.12 which this immediately replaced.

### 2.0.18.11

*[Released 21 Apr 2014](https://open.vanillaforums.com/discussion/26627/vanilla-2-0-18-11-security-release)*

* 3 security patches.
* Ditches troublesome "Remove" option on the plugins page.

### 2.0.18.10

*[Released 21 Dec 2013](https://open.vanillaforums.com/discussion/25668/dec-2013-security-update-2-0-18-10-and-2-1b2)*

* Removes flawed update checker.

### 2.0.18.9

*[Released 26 Nov 2013](https://open.vanillaforums.com/discussion/25458/security-update-vanilla-2-0-18-9)*

* Use SafeRedirect() instead of Redirect() in the discussion controller.
* Added TrustedDomains() and SafeRedirect().
* Don't allow user id override on post.
* Fix Flagging security flaw
* Filter discussion title on categories/all
* Comment notifications should only be sent to people with the "NewComment" preference set.
* Twitter: Change api version to 1.1.
* Tagging: Fix xss bug in tagging.
* Do not add linebreaks twice on search.

### 2.0.18.8

*[Released 4 Apr 2013](https://open.vanillaforums.com/discussion/23339/security-update-vanilla-2-0-18-8)*

* Call & check for FilterForm() properly.

### 2.0.18.7

* Disable the ability to call functions in escaped SQL strings.

### 2.0.18.6

* Switch update checks to JSON to prevent object injection hacks.

### 2.0.18.5

* Prevent object injection hacks.
* Make sure the admin password is hashed when inserting the admin user on an already installed Vanilla.
* Fix Facebook plugin for the 5 Dec 2012 Facebook update.
* Add class attributes for all the menu item elements.
* Cache-control logic improvements.
* Add the proper username parameter to profile/edit.
* Filter activity, discussion, and comment forms.
* Fixed security hole where on profile/picture and profile/preferences. Allow moderators to change users' pictures from the profile page.
* Added joomla password hashing.

### 2.0.18.4

*[Released 26 Mar 2012](https://open.vanillaforums.com/discussion/19542/vanilla-2-0-18-4-released)*

* Patch form tampering possibility.
* Fix canonical URL issues.

### 2.0.18.3

*[Released 5 Mar 2012](https://open.vanillaforums.com/discussion/19285/security-vulnerability-flagging-plugin-2-0-18-2-and-earlier)*

* Flagging plugin security fixes.

### 2.0.18.2

*[Released 21 Jan 2012](https://open.vanillaforums.com/discussion/18749/vanilla-2-0-18-2-release)*

* Fixed bug where Gravatar was using name instead of email for Vanillicons.
* vBulletin import improvements.
* SSO fixed for non-English.
* Embed improvements.
* Tagging fix.
* Fix malformed install screen.
* Various other bug fixes.

### 2.0.18.1

*[Released 7 Nov 2011](https://open.vanillaforums.com/discussion/17643/vanilla-2-0-18-final-release)*

* Fixed bug in the Twitter plugin.
* Fixed some bugs with connecting.
* Prevent too many "photo changed" activities.
* Added the ability to include announcements in the /categories/discussions page.
* Fix so people with custom domains don't see strange text.
* Fixes mass-approve/deny for Applicants
* Correct title on /categories pages
* Fixed jQuery syntax errors.

### 2.0.18
*[Released 3 Nov 2011](https://open.vanillaforums.com/discussion/17643/vanilla-2-0-18-final-release)*

Major Features:

* Added moderation, bans, and delete/edit logging.
* Added notifications (Growl-like popups).
* Added advanced category management.
* Added IP logging to core.
* Added Split/Merge plugin to core.

Changes:

* Added ability to chain Vanillicons into Gravatars with c(Plugins.Gravatar.UseVanillicons) = true
* Added ability to use IE targetting for CSS and JS files
* Disabled CLEditor for IE6 users
* Disabled popups in IE7 or less
* Added Session support, see: Gdn_Session()->stash()
* Turns off Embed by default
* Added WebOS to mobile user agents

Fixes:

* Fixed bug in 2.0.17 that could (on rare occassion) wipe your config.php file
* Fixed issue that could cause VanillaStats to stop working
* Many new translatable strings added or fixed
* Fixed support for PHP 5.2 on Windows (fnmatch)
* Fixed profile to not ask for old password if one was never set (via SSO)
* Fixed hundreds of other bugs too numerous to list, including dozens of SQL-related bugs.

### 2.0.17.1 - 2.0.17.10

* Fixed bug where analytics hooked before Garden.Installed=true, causing a fatal error on install.
* Fixed bug where analytics registration would occur repeatedly if config file was read-only.
* Repackaged distribution without OS-Specific meta data, and fixed ajax information exposure bug.
* Fixed problem with dashboard structure file where Activity and Profile permissions were not granted automatically on fresh install.
* Fixed problem with category permissions where some configurations would result in too restrictive defaults.
* SECURITY: Fixed potential querystring XSS and cookie HMAC Timing vulnerabilities in core.
* Updated analytics client and server software to fix a bug in stats transmission and rendering.
* Fixed a packaging problem that caused the contents of index.php to be duplicated.
* SECURITY: Fixed cookie theft vulnerability.
* SECURITY: Fixed Facebook, Twitter, and Embed plugins' access control.

### 2.0.17

*Released 2011-01-18*

* Fixed bug where plugins and themes could fail to enable due to extra whitespace.
* Fixed bug where search results were not properly sorted by date after relevance.
* Fixed bug where links in profile status cause the profile to clear when clicked.
* Fixed bug where signing in from the comment form button would not refresh the page.
* Fixed bug where administrators could not change user's picture without 404 errors.
* Fixed bug where stack trace would display when testing plugins, even if not in DEBUG mode.
* Fixed bug where signin would not properly redirect if javascript was disabled.
* Fixed bug where editing a role was erroneously selecting the default permission in the UI when editing.
* Fixed bug where discussion autorefresh would sometimes disable itself.
* Fixed bug where when markdown is enabled urls would not get auto-converted to clickable links.
* Fixed bugs in OpenID and GoogleSignIn where redirect targets were not getting sent to the signin.
* Fixed bug where mobile theme would sometimes display incorrect "last comment date".
* Optimized Announced Discussions query to improve performance.

## Older Releases

*Unlisted versions were skipped or replaced the same day.*

* 2.0.16 - 2010-12-02
* 2.0.15 - 2010-11-25
* 2.0.14 - 2010-11-09
* 2.0.13 - 2010-10-27
* 2.0.11 - 2010-10-06
* 2.0.10 - 2010-09-30
* 2.0.9 - 2010-09-15
* 2.0.6 - 2010-09-01
* 2.0.3 - 2010-08-11
* 2.0.1 - 2010-08-04
* 2.0.0 - 2010-07-22
* 1.1.10 - 2009-11-23
* 1.1.9 - 2009-09-10
* 1.1.8 - 2009-08-02
