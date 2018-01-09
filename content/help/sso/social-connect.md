---
title: Social Connect Plugins
tags:
- Features
- Addons
- Integrations
- Github
- Facebook
- SSO
- Social Sign On
- Google Plus
- Twitter
- Linkedin
category: help
menu:
  help:
    parent: sso
aliases:
- /help/addons/social
- /help/integrations/github
- /help/addons/social/github
- /help/addons/social/facebook
- /help/addons/social/googleplus
- /help/addons/social/twitter
- /help/addons/social/linkedin
---

Vanilla Forums integrates with a number of social applications that you can use as SSO solutions. Learn more about configuring these applications to work with your forum in this section.

## Github

This plugin allows you to submit user discussion and comments as GitHub issues.

### Setup Instructions

If you already have a Github account, you need to enable API Access for this plugin to work.

1. [Create a new application in GitHub](https://github.com/settings/applications/new), and set the callback URL by appending `/profile/githubconnect` to the end of your forum’s URL. (If your forum is at `example.com/forum`, your callback URL would be `http://example.com/forum/profile/githubconnect`).
2. Once your application has been set up, you must copy the **ClientID** and **Secret** into your Github plugin settings page from your Vanilla dashboard.
3. Enter the repositories you want to be allowed into your Github plugin settings page from your Vanilla dashboard.

## Facebook

Facebook Connect allows users to sign in using their Facebook account. You must register your application with Facebook for this plugin to work.

### How to set up Facebook Connect

In order to set up Facebook Connect, you must create an "application" in Facebook at: [https://developers.facebook.com/apps](https://developers.facebook.com/apps)

Once your application has been set up, you must copy the "Application ID" and "Application Secret" into your Facebook plugin settings page from your Vanilla dashboard.

### Need help?

For a complete walk-through of the steps involved, read [How to Create a Facebook Application for Vanillaforums Single Sign-On (SSO)](http://blog.vanillaforums.com/facebook-application-for-vanillaforums-sso/).

## Google Plus

The Google Plus Sign-In adds the ability to sign to your community with Google Plus. You will need to configure your site in [Google API Console](https://code.google.com/apis/console). This [Google+ Video Tutorial](http://youtu.be/OHEb22VrZy4) also shows you how to set this up.

### Setting up social login in Google Plus

1. Once you have enabled the Google+ Plugin in your Vanilla Dashboard, go to your API Console at Google.
2. You will  need to create a project.
2. Once you have a project, click on the project name. You will be presented with a side menu. Select “Credentials”.
3. Create New ClientID and fill in the form.
4. Select Web Application as Type.
5. For authorized Javascript Origins URL will be your Vanilla Forums URL
6. For authorized redirect URL, append "/entry/googleplus" to the end of your forum’s URL. (If your forum is at `example.com/forum`, your redirect URL would be `http://example.com/forum/entry/googleplus`).
7. Copy over Client ID and Secret into appropriate fields in Vanilla Dashboard.
8. If you have never used Google APIs before you will also need to fill in Consent Screen.

![Settings in Google Plus](/img/help/addons/social/googleplus/settings.png)

## Twitter

Twitter Connect allows users to sign in using their Twitter account. You must register your application with Twitter for this plugin to work.

### Setting up social login in Twitter Connect

1. Register Vanilla with Twitter at: [https://apps.twitter.com/app/new](https://apps.twitter.com/app/new)
2. Set the Callback URL by appending `/entry/twauthorize` to the end of your forum’s URL. (If your forum is at `example.com/forum`, your Callback URL would be `http://example.com/forum/entry/twauthorize`).
3. After registering, copy the "Consumer Key" and "Consumer Secret" into your Twitter plugin settings page from your Vanilla dashboard.

![Settings in Twitter](/img/help/addons/social/twitter/settings.png)

## LinkedIn

Linked In social sign in allows users to sign in using their LinkedIn account. You must register your application with LinkedIn for this addon to work.

### How to Set up LinkedIn Social Sign in

1. Go to the LinkedIn Developer Network at [https://www.linkedin.com/secure/developer](https://www.linkedin.com/secure/developer)/
2. Click **Add New Application**. When you create the application, you can choose what to enter in most fields, but you have to make sure you enter specific information for some fields.
3. Under **Website URL** enter your forum's root url.
4. Under **Default Scope** make sure you've selected at least **r_basicprofile** and **r_emailaddress**.
5. Set the **OAuth 2.0 Redirect URLs** by appending both `/entry/connect/linkedin` and `/profile/linkedinconnect` to the end of your forum’s URL. (If your forum is at `example.com/forum`, your Redirect URLs would be `http://example.com/forum/entry/connect/linkedin` and `http://example.com/forum/profile/linkedinconnect`).
6. Once your application has been set up, you must copy the **Client ID** and **Client Secret** into your LinkedIn plugin settings page from your Vanilla dashboard.

![Settings in LinkedIn](/img/help/addons/social/linkedin/settings.jpg)