Why does the assistant not launch?
==================================

By default the assistant will be hidden and minimized to tray when launched. You will need to follow either steps to launch the assistant after running the application:

- Try launching the assistant with the keyboard shortcut `Super + Shift + A`
- Right-click on the Google Assistant tray icon and click on **"Launch Assistant"**

**PS:** The assistant will take some time to initialize _(indicated by grayscale Google Assistant icon)_. Executing any of the above steps during this time will not launch the assistant. You will have to wait until you see the colorful Google Assistant Icon in the tray and then try to launch the assistant.

Why am I getting "Error 403: restricted_client"?
================================================

If you encounter this issue, you probably have not configured the consent screen. You can get help with setting up consent screen using [this link](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/wiki/Setup-Authentication-for-Google-Assistant-Unofficial-Desktop-Client#configure-consent-screen). Make sure that you follow all the steps correctly. Skipping any steps or ignoring parts of any steps would trigger the above error.

Also, make sure you are using the same Google account to authenticate whose Gmail address was specified under **"Test Users"**.

Why does the "Get Token" screen fail saving tokens?
===================================================

- If you encounter **"Error: Tried calling start() before the ready event!"** and click on ignore and then try to paste authentication code followed by clicking on "Submit", nothing would happen (only as of version `1.0.0-rc.2`).

  Until the next version is released with the bug fixed, you can either clone this project and build it yourself or if you do not want to build it yourself, you can _temporarily_ disable **Settings** > **Conversation** > **Enable microphone on application startup**, relaunch assistant and let the assistant save the tokens after which you can enable the setting again.

- If you get **"Failed to get tokens"** error, you might have one of the following issues:
  - Saved Tokens Path might point to a privileged location _(like C: in windows or /usr/local in *nix based systems)_ requiring Admin/Superuser access. In this case, try to change the Key File path and Saved Tokens File path to a location which might not require escalated privileges to access.
  - Exhausted the daily limit of requesting the tokens in which case trying it the next day might work.

Why does the setting button not work?
=====================================

If you are in the Welcome screen as below, you will have to click through **"Get Started"** and **"Proceed"** button before you can access the settings. The reason being when you launch the app for the first time, no config file is created causing errors when saving settings. Thus, the settings button is intentionally disabled.

![Welcome Screen](https://user-images.githubusercontent.com/26056183/107728586-7e429b80-6d14-11eb-98d5-f0ff63891702.png)

Have issues that are not listed here?
=====================================

I would encourage you to find if anyone already encountered the same issue as you [here](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/issues). To narrow down the list to any issues frequently encountered by others, [click here](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/issues?q=is%3Aissue+label%3Aduplicate+is%3Aclosed).

Didn't find any issues that reflect your problem? [Create a new issue](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/issues/new/choose)
