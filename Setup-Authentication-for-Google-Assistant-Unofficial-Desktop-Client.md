# Device Registration

1. Head on to [Actions Console](https://console.actions.google.com/)

2. Click on the "`New Project`" button

![Actions Console](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/1_1_actions-console.png)

3. You will see a "**New Project**" popup. Enter _any_ project name and set other options accordingly and click on "**Create Project** button"

![Add Project](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/1_2_add-project.png)

4. Now, after your project is created, you will see the "onboarding" page. Just scroll to the bottom and click on the **"click here"** link right after the text "Are you looking for device registration?" to proceed to Device Registration

![Onboarding Page](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/1_3_onboarding_screen.png)

5. Wait until your project is created...

![Creating Project on Actions Console](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/1_4_creating_project.png)

6. Now, you will be landed in the "Device Registration" page. Here, click on "**Register Model**" button

![Device Registration Page](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/1_5_device_reg_screen.png)

7. You will see a "Register Model" popup, fill all the details and for device type, select any (eg: `light`). Then, finally click on "**REGISTER MODEL**"

![Register Model](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/1_6_register-model.png)

8. Now, after you have created a model, you will be asked to download the credentials. Click on "**Download OAuth 2.0 credentials**"

![Download Credentials](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/1_7_download-credentials.png)

> Now, you are done with the registration process. But in order to authenticate, you have to "Configure Consent Screen"

# Configure Consent Screen

1. Head on to [Cloud Console](https://console.cloud.google.com/)

2. In the Navbar beside the logo, click on the button to select a project

![Select Project in Cloud Console](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_1_select-project-btn.png)

3. You will see a popup titled "*Select a project*". Click on the "*ALL*" tab and select the name of the project you just created. Then, press *OPEN* to continue

![Select Project Popup](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_2_select-project.png)

4. Now, from the hamburger menu, select "**APIs & Services**"

![APIs and Services Menu](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_3_API-and-services-menu.png)

5. Click on "**ENABLE APIS AND SERVICES**"

![Enable APIs and Services Button](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_4_enable-api.png)

6. You will be landed in "*API Library*"

![API Library](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_5_api-lib.png)

7. In the search bar, type "*Google Assistant*" and click on "**Google Assistant API**"

![API Library Search](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_6_api-lib-search.png)

8. Press "**ENABLE**" button to enable the API

![Enable API](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_7_enable-api-btn.png)

9. Wait until the API is enabled

10. Now, from the hamburger menu, click on "**Credentials**"

11. Click on the "**CONFIGURE CONSENT SCREEN**"

![Credentials Tab](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_8_credentials.png)

12. In the *OAuth Consent Screen* under *User Type*, select **External**. Then, click **CREATE**

![OAuth User Type](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_9_oauth-user-type.png)

13. In the next page, under *"App Registration"* select your email for "**User Support email**"

![Select Support E-Mail](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_10_support-email.png)

14. Scroll down to the bottom of the page. Under "*Developer Contact Information*", fill in your email address for "**Email addresses**" and click on **SAVE AND CONTINUE**

![Fill Developer Contact E-mail address](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_11_dev-contact-info.png)

15. Now skip the *"Scopes"* screen by clicking on **SAVE AND CONTINUE**

![click on "save and continue" to skip "Scopes" screen](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_12_scopes-screen.png)

16. Under "*Test Users*" click on "**ADD USERS**" button

![Add users under "Test Users"](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_13_add-users.png)

17. Under "*Add Users*", type the email address of the Gmail account that you will use to authenticate (preferably your current Gmail account). You can add multiple Gmail accounts by adding a comma after each of the Gmail accounts.

![Type Gmail account email address for authentication](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/blob/master/images/Wiki/2_14_add-users-sidebar.png)

# Final steps...

Now, you are all done. You can now go to "**Settings**" in the *Google Assistant Unofficial Desktop Client* and set the "**Key File Path**" to the path where you have kept the "**OAuth 2.0 Credentials**" and save the settings. You will be asked to reload the Assistant after which you will be presented with "*Get Tokens!*" screen which will automatically save your tokens. After this, you can use your Google Assistant.

> ## Other References
>
> **Device Registration using UI:**
> - https://developers.google.com/assistant/sdk/guides/library/python/embed/config-dev-project-and-account
>
> **Device Registration using Command Line Tool:**
> - https://developers.google.com/assistant/sdk/reference/device-registration/register-device-manual
