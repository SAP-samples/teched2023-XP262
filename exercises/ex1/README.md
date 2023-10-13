# Exercise 1 - Create and configure you SAP Build Work Zone, standard edition site
In this exercise you’ll create a business site and then add business apps to this site, both locally created and integrated from SAP S/4HANA Cloud.

> [!IMPORTANT]
> Wherever ### is mentioned, please replace this with your assigned User ID. For example, 'WZ Site 001' instead of 'WZ Site ###'.

## Exercise 1.1 Create your "site" 
After completing these steps you will have created a site in SAP Build Work Zone and configured for the desired layout.

1. Click 'Create' in SAP Build Lobby.
  ![](/exercises/ex1/images/lobby_create.png)

2. Select 'Build a Business Site' in SAP Build Lobby.
  ![](/exercises/ex1/images/lobby_business_sites.png)

3. Click 'Configure Site in Admin Console'.
  ![](/exercises/ex1/images/lobby_create_site.png)

4. Site Directory.
  ![](/exercises/ex1/images/site_directory.png)
When you access the SAP Build Work Zone, standard edition, the Site Directory is in focus. From here you’ll create your new site.
> [!NOTE]
> In the side panel, you’ll see four tools. The Site Directory where you’re going to create a new site. All sites that you create will be displayed here. The Content Manager where you’ll manage cross-site content such as business apps. The Channel Manager where you manage different channels that expose business content that you can integrate into your sites. The fourth icon opens Settings where you can configure various settings related to your subaccount.

5. Create Site.
  ![](/exercises/ex1/images/create_site.png)

6. Enter 'WZ Site ###' as Site Name amd click **Create**.
  ![](/exercises/ex1/images/create_site_2.png)

6. Click Edit in the top right corner of the screen.
  ![](/exercises/ex1/images/create_site_2.png)
You’ve just created a site called WZ Site ###.

7. Enter 'WZ Site ###' as Site Name amd click **Create**.
  ![](/exercises/ex1/images/create_site_2.png)
You’ve just created a site called WZ Site ###.

8. Click **Edit** in the top right corner of the screen.

9. Select the Spaces and Pages - New Experience view mode
  ![](/exercises/ex1/images/edit_site_mode.png)
Under Display, select Spaces and Pages - New Experience.

10. Click Save.

11. Navigate back to the Site Directory to view the site tile.
  ![](/exercises/ex1/images/edit_site_back.png)
Your site is empty for now. In the next steps, you’re going to add business apps to your site.


## Exercise 1.2 - Integrate an SAPUI5 App
After completing these steps you will have added an existing SAPUI5 app to a site in the SAP Build Work Zone.

1. Open Content Manager
   Click the Content Manager icon in the side panel to open the Content Manager.
  ![](/exercises/ex1/images/content_manager.png)
> [!NOTE]
> When you open the Content Manager you’ll see a list of content items that have been added to your subaccount. From here you can manually configure new content items and view any other available content items. You can also access the Content Explorer where you can explore exposed content from available channels, select the content, and add it to your own content.

2. Click Create and select App from the list.
  ![](/exercises/ex1/images/create_app.png)

3. In the app editor, enter a title **New Orders ###**.
  ![](/exercises/ex1/images/ui5_app_1.png)

4. Under the Configuration tab, enter the following values (some will already be there by default):
   - Open App: In place
   - System: No System
   - App UI Technology: URL
   - URL: https://sapui5.hana.ondemand.com/test-resources/sap/m/demokit/cart/webapp/index.html  
   ![](/exercises/ex1/images/ui5_app_2.png)

> [!NOTE]
> When working in your own environment, it’s better to integrate SAPUI5 apps by configuring a destination to the relevant system and setting the app properties to use this destination. In this case in the App UI Technology dropdown list, you would select SAPUI5. This configuration allows you to better manage your content in the Dev-QA-Prod lifecycle.

5. Click the Navigation tab to specify the intent of your app.
   The unique combination of a semantic object and an action is called an intent. It is used to define navigation to an application.

6. Enter the following values:
   - Semantic Object: Order
   - Action: Display
  ![](/exercises/ex1/images/ui5_app_3.png)
    
7. Click the Visualization tab.
   In this tab, you specify how the app will be displayed in the site.

8. Enter the following values:
   - Subtitle: Shopping Cart
   - Information: Order Now!
   - Icon: Click the browse icon, type my-sales-order, and click on the displayed icon to add it to your tile.

    ![](/exercises/ex1/images/ui5_app_4.png)

9. On the right, you can see a preview of the tile with all the properties you entered. Click Save.

10. View the app that you created
    Go back to the Content Manager by clicking on the breadcrumbs. You can see your app in the list of content items:
    ![](/exercises/ex1/images/ui5_app_created.png)

## Exercise 1.3 - Integrate a URL App 
Create a URL app and add it to your site.

1. Click Create and select App from the list.
  ![](/exercises/ex1/images/url_app_1.png)

2. In the app editor, enter a title **External Community ###**.
  ![](/exercises/ex1/images/url_app_2.png)

3. Under the Configuration tab, enter the following values (some of them are already there by default):
   - Open App: In a new tab
     - It’s preferable to open apps in place, but this time, we’ll open the app in a new tab.
   -  System: No System
   -  App UI Technology: URL
   -  URL: https://community.sap.com/topics/work-zone
![](/exercises/ex1/images/url_app_3.png)

4. Click the Navigation tab and enter the intent of your app.
The unique combination of a semantic object and an action is called an intent. It is used to define navigation to an application.

5. Enter the following values:
   - Semantic Object: Home
   - Action: Display
![](/exercises/ex1/images/url_app_4.png)

6. Click the Visualization tab.
   - Subtitle: SAP Build Work Zone
   - Information: Join Us Now!
   - Icon: Click the browse icon, type visits, and click on the displayed icon to add it to your tile.
  ![](/exercises/ex1/images/url_app_5.png)

7. Click Save.
   You have configured the URL app and in the next step you’ll go back to the Content Manager to see it in the list of content items.

8. View the app that you created
   Go back to the Content Manager by clicking on the breadcrumbs. You can see your app in the list of content items:
   ![](/exercises/ex1/images/url_app_result.png)


## Exercise 1.4 - Create a Page

1. Open the Content Manager.
  
2. Click Create and from the dropdown list, select Page.
   ![](/exercises/ex1/images/create_page_1.png)

3. Enter a title for the page: **Overview ###**.
   ![](/exercises/ex1/images/create_page_2.png)

4. Click Add Section.
   ![](/exercises/ex1/images/create_page_3.png)
   
5. Give the section a title, **My Local Apps** and click Add Widget.
   ![](/exercises/ex1/images/create_page_4.png)
   
6. In the Add Widgets screen, click Tiles.
  ![](/exercises/ex1/images/create_page_5.png)

7. Select the **External Community ###** and the **New Orders ###** apps and click Add.
   ![](/exercises/ex1/images/create_page_6.png)

8. Click Add Section.
   ![](/exercises/ex1/images/create_page_7.png)

9. Give the section a title, **My S/4HANA Cloud Apps**.
   ![](/exercises/ex1/images/create_page_8.png)
   
10. Click Add Widget.
    ![](/exercises/ex1/images/create_page_9.png)

12. In the Add Widgets screen, click Tiles.
    ![](/exercises/ex1/images/create_page_10.png)

13. Search for integrated S/4HANA Apps, select them & click Add (3):
  - Delivery Schedules
  - Incoming Sales Orders
  - Track Sales Orders
    ![](/exercises/ex1/images/create_page_11.png)

13. Observe the following apps being added.
    ![](/exercises/ex1/images/create_page_12.png)

14. Save.
    ![](/exercises/ex1/images/create_page_13.png)
    
16. Go back to your Content Manager using the breadcrumbs at the top.
    ![](/exercises/ex1/images/create_page_14.png)

## Exercise 1.5 - Create a Space

## Exercise 1.6 - Add Content to Role & Site

## Summary

You've now ...

Continue to - [Exercise 2 - Exercise 2 Description](../ex2/README.md)

