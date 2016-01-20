# n1-unsubscribe
This is a plugin for [Nylas N1](https://www.nylas.com/n1) that adds quick unsubscribe functionality. It is currently in a very early beta stage, and you *may* encounter issues while using it. If so, please report them [here as an issue][issues], so they can be fixed. Have a feature request or great idea? Also submit them through the issues pane and we will take a look as quickly as possible!

## Overview

- Quick action and Toolbar unsubscribe buttons
- Automated unsubscribe request for most email marketers
- Otherwise, opens a Browser Window within N1 for manual unsubscribing
- Auto-trash email after success

## Install this plugin

1. [Install N1](https://www.nylas.com/n1)

2. Download the most recent release from the [Releases page](https://github.com/colinking/n1-unsubscribe/releases).

3. From the N1 menu, select `Developer > Install a Plugin Manually...`, then select the downloaded folder and the plugin will be installed.

### The Unsubscribe Button

To unsubscribe from an email, look for the button with this icon:

![NormalIcon](/assets/unsubscribe%402x.png)

### Behind the Scenes

We use the list-unsubscribe header that is invisibly attached to most marketing emails. If there is no header, we scour the email body for an unsubscribe link or a phrase describing how to unsubscribe. Once a link is found, either an automated email will be sent or a mini browser will appear that will allow you to quickly unsubscribe without leaving N1. The email is trashed for you once this completes. An important note, if no unsubscribe action is available, the button will be hidden.

### Current Features

> Anywhere you interact with an email, we have a quick unsubscribe button for you

<!--#### Bulk Action-->

<!--(To Be Developed)-->

<!--![BulkAction](README/BulkAction.png)-->

#### Quick Action

From the comfort of your inbox view, you can easily unsubscribe from an email by tapping the new icon alongside the trash and archive buttons that you are used to. If no unsubscribe action is available, the button will be hidden.

![QuickAction](README/QuickAction.png)

#### Menu Item

While reading an email you may realize that you would like to unsubscribe, so instead of scrolling to the bottom of the email and playing the *spot the unsubscribe link game*, which is [an actual game](http://spottheunsubscribe.tumblr.com/), you can press the obvious button at the top.

![MenuItem](README/MenuItem.png)

## Future Features of n1-unsubscribe 
- Better notification of in-progress unsubscribe
- Add a bulk-unsubscribe tool bar button that is enabled when selecting multiple emails
- Add tests and Travis CI and stricter linting?

## Made by
[Kyle King](http://kyleking.me) and [Colin King](http://colinking.co)

[Also StartupHealth is a great organization, they just happened to be at the top of my inbox](https://www.startuphealth.com/)

[issues]: https://github.com/colinking/n1-unsubscribe/issues
