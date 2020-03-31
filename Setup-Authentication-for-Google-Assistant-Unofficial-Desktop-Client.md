# Device Registration

1. Head on to [Actions Console](https://console.actions.google.com/)

2. Click on the "`New Project`" button

3. You will see a "**New Project**" popup. Enter _any_ project name and set other options accordingly and click on "**Create Project** button"

4. Now, after your project is created, you will see the "onboarding" page. Just scroll to the bottom and select "**Device Registration**" under _More options_

5. Wait until your project is created...

6. Now, you will be landed in the "Device Registration" page. Here, click on "**Register Model**" button

7. You will see a "Register Model" popup, fill all the details and for device type, select any (eg: `light`). Then, finally click on "**REGISTER MODEL**"

8. Now, after you have created a model, you will be asked to download the credentials. Click on "**Download OAuth 2.0 credentials**"

> Now, you are done with the registration process. But in order to authenticate, you have to "Configure Consent Screen"

# Configure Consent Screen

1. Head on to [Cloud Console](https://console.cloud.google.com/)

2. In the Navbar beside the logo, click on the button to select a project

3. You will see a popup titled "*Select a project*". Click on the "*ALL*" tab and select the name of the project you just created. Then, press *OPEN* to continue

4. Now, from the hamburger menu, select "**APIs & Services**"

5. Click on "**ENABLE APIS AND SERVICES**"

6. You will be landed in "*API Library*"

7. In the search bar, type "*Google Assistant*" and click on "**Google Assistant API**"

8. Press "**ENABLE**" button to enable the API

9. Wait until the API is enabled

10. Now, from the hamburger menu, click on "**Credentials**"

11. Click on the "**CONFIGURE CONSENT SCREEN**"

12. In the *OAuth Consent Screen* under *User Type*, select **External**

13. In the next page, select your email under "**Support email**". Finally, scroll to the end of the page & click on "*SAVE*"

# Final steps...

Now, you are all done. You can now go to "**Settings**" in the *Google Assistant Unofficial Desktop Client* and set the "**Key File Path**" to the path where you have kept the "**OAuth 2.0 Credentials**" and save the settings. You will be asked to reload the Assistant after which you will be presented with "*Get Tokens!*" screen which will automatically save your tokens. After this, you can use your Google Assistant.

> ## Other References
>
> **Device Registration using UI:**
> - https://developers.google.com/assistant/sdk/guides/library/python/embed/config-dev-project-and-account
>
> **Device Registration using Command Line Tool:**
> - https://developers.google.com/assistant/sdk/reference/device-registration/register-device-manual
