
# Exercise 3 - Access Site via SAP Mobile Start
In this exercise you’ll access your SAP Build Work Zone site from your mobile device using the native SAP Mobile Start app.

> [!IMPORTANT]
> Wherever ### is mentioned, please replace this with your assigned User ID. For example, 'WZ Site 001' instead of 'WZ Site ###'.

## Exercise 3.1 - Enable SAP Mobile Start in Site Settings
After completing these steps you will have enabled your site for SAP Mobile Start.

1. Access the Site Directory and Click the Settings icon for your **WZ Site ###**.
  ![](/exercises/ex3/images/sms_1.png)

2. Click Edit.
![](/exercises/ex3/images/sms_2.png)

3. Make sure the toggle for SAP Mobile Start is enabled.
![](/exercises/ex3/images/sms_3.png)

4. Save and Navigate back to Site Directory.
![](/exercises/ex3/images/sms_4.png)



## Exercise 3.2 - Add mobile app as content
In this step you are adding additional content that will become available in SAP Mobile Start.

1. Access the Content Manager (side menu) and Create a new Application.
  ![](/exercises/ex3/images/mobile_content_1.png)

2. Add **SuccessFactors App ###** as Title
![](/exercises/ex3/images/mobile_content_2.png)

3. Change the App UI Technology to Native iOS or Android (depending on your device) and enter the application details for SAP SuccessFactors:

- URL to Launch App: bizx://?urlType=deeplink\&amp;deeplinkType=profile
- URL to Install App: https://apps.apple.com/de/app/successfactors/id426562526

    ![](/exercises/ex3/images/mobile_content_3.png)

    If you are using Android, please use the following values:
- URL to Launch App: __bizx://?urlType=deeplink\&amp;deeplinkType=profile__
- URL to Install App: https://play.google.com/store/apps/details?id=com.successfactors.successfactorsInformation

4. Add Navigation Parameters
- Semantic Object: **SFSF**
- Action: Launch
![](/exercises/ex3/images/mobile_content_4.png)

5. Select Device Type to Mobile (only):
![](/exercises/ex3/images/mobile_content_5.png)

6. Navigate to Content Manager and Verify App.
![](/exercises/ex3/images/mobile_content_6.png)

7. Create a new Group.
  ![](/exercises/ex3/images/group_1.png)

8. Add **Mobile Content ###** as Title
![](/exercises/ex3/images/group_2.png)

9. Add Applications to Group.
![](/exercises/ex3/images/group_3.png)

10. Save.

11. Navigate back to Content Manager (side menu).

12. Select the **XP262_###_Role**.
![](/exercises/ex3/images/role_1.png)

13. Add newly created application to role.
![](/exercises/ex3/images/role_2.png)

14. Save.


## Exercise 3.3 - Activate Your site in SAP Mobile Start
After completing these steps you will have connected your site with SAP Mobile Start.

1. Navigate to Site Directory (side menu) and Launch Site.
![](/exercises/ex3/images/sms_5.png)

2. On the site, open the user menu via the user icon on the top right. Then choose Settings.
  ![](/exercises/ex3/images/activate_mobile_1.png)

3. In the Settings screen, select the SAP Mobile Start Application tab.
![](/exercises/ex3/images/activate_mobile_2.png)

In this screen you can select your device type (iOS or Android) and switch between the two QR Codes via the toggle button:
- Install: This QR-Code can be used to install the SAP Mobile Start app on your device. It’s a direct link to the Apple app store page.
- Register: This QR-Code is used later within the SAP Mobile Start app to register it to your site.

> [!NOTE]
> For the deployment to end-users it’s possible to make use of Mobile Device Management (MDM). Administrators can deploy a managed app configuration via the MDM that contains site information. With that end-users can onboard without the need to scan a QR code. See the documentation for further information.

4. Install SAP Mobile Start on your mobile device
<br>Use the Install QR-Code from Step 2 to install SAP Mobile Start on your Mobile Device. Alternatively, you can search for SAP Mobile Start in the respective App Stores.

5. Open the SAP Mobile Start app on your mobile device, press the Scan button and make sure to allow camera access.
![](/exercises/ex3/images/activate_mobile_3.png)
<br> Below the scan button you will find the option to enter the demo mode. This will demonstrate how a fully configured site with the addition of SAP Task Center looks like.

6. Next, use your device camera to scan the Register QR-Code in the launchpad user settings from Step 2. If the scan succeeded, you can continue with the onboarding process.
![](/exercises/ex3/images/activate_mobile_4.png)

7. Follow the guided onboarding process within the app:
- Log in with your user
- Accept the End User License Agreement and Data Privacy Statement
- Depending on your setup you might need to create a passcode / allow biometric authentication.

    After completing the onboarding process, you will be directed to the initial Start screen.

## Exercise 3.4 - Validate and explore content on your mobile device

1. Application Layout
    <br>You can use the navigation icons on the bottom the move between the Start, Apps and the To Do screens.
    - The Start screen offers an overview for quick access to your most used apps. 
    - The Apps screen lists all the Groups and Apps available.
    - The To Do screen lists all To Dos coming from SAP Task Center.

![](/exercises/ex3/images/mobile_app_1.png)

2. Within the Application screen you can use the search bar to find specific applications.

3. From the profile and settings you can choose Sign Out to return to the initial onboarding screen, in case you want to connect to a different site.

