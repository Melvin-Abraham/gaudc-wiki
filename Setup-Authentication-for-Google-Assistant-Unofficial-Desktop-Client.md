## Device Registration

1. Head on to [Actions Console](https://console.actions.google.com/)

2. Click on the "`New Project`" button

    ![Actions Console](./assets/actions-console.png)

3. You will see a "**New Project**" popup. Enter _any_ project name and set other options accordingly and click on "**Create Project** button"

    ![Add Project](./assets/add-project.png)

4. Now, after your project is created, you will see the "onboarding" page. Just scroll to the bottom and click on the **"click here"** link right after the text "Are you looking for device registration?" to proceed to Device Registration

    ![Onboarding Page](./assets/onboarding_screen.png)

5. Wait until your project is created...

    ![Creating Project on Actions Console](./assets/creating_project.png)

6. Now, you will be landed in the "Device Registration" page. Here, click on "**Register Model**" button

    ![Device Registration Page](./assets/device_reg_screen.png)

7. You will see a "Register Model" popup, fill all the details and for device type, select any (eg: `light`). Then, finally click on "**REGISTER MODEL**"

    ![Register Model](./assets/register-model.png)

8. Now, after you have created a model, you will be asked to download the credentials. Skip this by clicking on **Next**.

    ![Download Credentials](./assets/download-credentials.png)

> Now, you are done with the registration process. But in order to authenticate, you have to "Configure Consent Screen"

## Configure Consent Screen

1. Head on to [Cloud Console](https://console.cloud.google.com/)

2. In the Navbar beside the logo, click on the button to select a project

    ![Select Project in Cloud Console](./assets/select-project-btn.png)

3. You will see a popup titled "*Select a project*". Click on the "*ALL*" tab and select the name of the project you just created. Then, press *OPEN* to continue

    ![Select Project Popup](./assets/select-project.png)

4. Now, from the hamburger menu, select "**APIs & Services**"

    ![APIs and Services Menu](./assets/API-and-services-menu.png)

5. Click on "**ENABLE APIS AND SERVICES**"

    ![Enable APIs and Services Button](./assets/enable-api.png)

6. You will be landed in "*API Library*"

    ![API Library](./assets/api-lib.png)

7. In the search bar, type "*Google Assistant*" and click on "**Google Assistant API**"

    ![API Library Search](./assets/api-lib-search.png)

8. Press "**ENABLE**" button to enable the API

    ![Enable API](./assets/enable-api-btn.png)

9. Wait until the API is enabled

10. Now, from the hamburger menu, click on "**Credentials**"

11. Click on the "**CONFIGURE CONSENT SCREEN**"

    ![Credentials Tab](./assets/credentials.png)

12. In the *OAuth Consent Screen* under *User Type*, select **External**. Then, click **CREATE**

    ![OAuth User Type](./assets/oauth-user-type.png)

13. In the next page, under *"App Registration"* select your email for "**User Support email**"

    ![Select Support E-Mail](./assets/support-email.png)

14. Scroll down to the bottom of the page. Under "*Developer Contact Information*", fill in your email address for "**Email addresses**" and click on **SAVE AND CONTINUE**

    ![Fill Developer Contact E-mail address](./assets/dev-contact-info.png)

15. Now skip the *"Scopes"* screen by clicking on **SAVE AND CONTINUE**

    ![click on "save and continue" to skip "Scopes" screen](./assets/scopes-screen.png)

16. Under "*Test Users*" click on "**ADD USERS**" button

    ![Add users under "Test Users"](./assets/add-users.png)

17. Under "*Add Users*", type the email address of the Gmail account that you will use to authenticate (preferably your current Gmail account). You can add multiple Gmail accounts by adding a comma after each of the Gmail accounts.

    ![Type Gmail account email address for authentication](./assets/add-users-sidebar.png)

## Configure Credentials

1. Select **Credentials** from the sidebar. Then, under the **OAuth 2.0 Client IDs**, click on **Web Client** to edit the web client credentials.

    ![Credentials Page](./assets/cred-page.png)

2. Update the redirct URI under the **Authorized redirect URIs** section to:

    ```
    https://localhost:5754/auth/handler
    ```

    ![Updated Redirect URI](./assets/cred-config-redirect-uri.png)

3. Now, click on **Save**. This will redirect you back to the credentials page.

4. Click on **Web Client** *again* in order to reset the client secret.

5. Click on **Reset Secret** on the top. This will display a popup for confirmation. Click on **Reset** to confirm.

    ![Reset Client Secret](./assets/cred-config-reset-secret.png)

6. Click on **Save** again.

7. Now, click on the download button against **Web Client**

    ![Credential Download Button Click](./assets/cred-download.png)

8. This will open a popup dialog. Click on **Download JSON** button. This is your **OAuth 2.0 Credential**.

    ![Credential Download Dialog Popup](./assets/cred-download-dialog.png)

## Setting authentication in the app

1. Run and launch the **Google Assistant Unofficial Desktop Client** app

2. Click on the "**Settings**" button in the top-left corner of the application

3. Under the "**Authentication**" section, set the "**Key File Path**" to the path where you have kept the "**OAuth 2.0 Credentials**" and leave the "**Saved Tokens Path**" empty. Now click on "**Save**" button

    ![Authentication: Set Key File Path](./assets/assist-settings-auth.png)

4. You will be prompted to automatically create a path for "*Saved Tokens Path*". Click on "**Automatically set a path**"

    ![Automatically set a Saved Tokens Path](./assets/assist-set-tokens-path.png)

5. You will be asked to reload the Assistant. Click on "**Relaunch Assistant**" button

    ![Relaunch assistant](./assets/assist-relaunch-assistant.png)

6. Now, you will be presented with the "*Get Token!*" screen. An authentication page will be opened in your default browser

    ![Get Tokens screen](./assets/assist-get-tokens.png)

7. Select the preferred Gmail account to authenticate

    ![Choose Gmail account to authenticate](./assets/choose-gmail-account.png)

8. You might come across the following warning: "**Google hasn't verified this app**". Since the project is created by you, this should be safe to proceed with. Click on "**Continue**"

    !["Google hasn't verified this app" warning screen](./assets/app-not-verified-err.png)

9. Now grant permission to the project by clicking on "**Continue**"

    ![Project Permission](./assets/grant-app-permission.png)

10. You will now be presented with the authorization code screen. Click on the *copy* button

    ![Authorization Code Screen](./assets/copy-auth-code.png)

11. Switch to the application and paste the code in the respective field. Now click on "**Submit**"

    ![Paste Authorization Code](./assets/assist-paste-code.png)

12. You will be prompted to relaunch the app again. Click on "**Relaunch Assistant**"

Now, you are all set! You can finally use the Google Assistant Unofficial Desktop Client and customize it the way you want... 😉

## Enabling Personal Results (Optional)

> Personal results are results that are fetched from Google Services like Gmail, Google Calendar, Google Photos, etc. These results are not shown by default as they might be part of user activity and personal data. If you want the assistant to show you your personal results when asked for it, you must explicitly enable it. Below are the steps to help you enable personal results.

1. Once your assistant app is ready to use after having followed the proper steps, you must ask the assistant specific queries to trigger personal results. For example, "What's my name?", "Show me my photos" or "What's on my calendar next?".

    ![Trigger Personal Result Query](./assets/assist-personal-results-permission.png)

2. As mentioned in the above screenshot, you might receive a notification on your phone to turn on personal results. Tap on the notification.

    ![Allow Personal Answers - Phone Notification](./assets/phone-allow-personal-answers-notification.jpeg)

3. You will come across a screen like the one below. Tap on **"Device Name"**. _(Do not toggle Personal Results right away)_

    ![Allow Personal Answers - Initial Screen](./assets/phone-allow-personal-answers-screen.jpeg)

4. Now, enter any device name, say, "G Assist" and tap on **"OK"**.

    ![Allow Personal Answers - Device Name Prompt](./assets/phone-allow-personal-answers-device-name.jpeg)

5. After the device name has been set, tap on **"Personal Results"** to enable personal results.

    ![Allow Personal Answers - Personal Results Toggle](./assets/phone-allow-personal-answers-toggle.jpeg)

That's it. Now, you can ask the assistant to show your personal results. If you are still prompted to allow personal results, that probably means that personal results could not be enabled in your current project. In this case, you might have to [start afresh and create a new actions project](#device-registration) if you want to enable this feature.

## Experiencing an issue?

You can check out the [Frequently Asked Questions (FAQ)](https://github.com/Melvin-Abraham/Google-Assistant-Unofficial-Desktop-Client/wiki/Frequently-Asked-Questions-(FAQ)).

## Other References

> **Device Registration using UI:**
>
> - https://developers.google.com/assistant/sdk/guides/library/python/embed/config-dev-project-and-account
>
> **Device Registration using Command Line Tool:**
>
> - https://developers.google.com/assistant/sdk/reference/device-registration/register-device-manual
