# Exercise 2 - Integrate and explore SAP Task Center

In this exercise, we will create a **purchase requisition** in SAP S/4HANA Cloud to get a Task for the PR approval in **SAP Task Center**.

## Exercise 2.1 create a purchase requisition in SAP S/4HANA Cloud

- To create a PR in S4HC please enter the following URL (https://myxxxx.s4hana.cloud.sap/ui#PurchaseOrder-manage&/C_PurchaseOrderTP(PurchaseOrder='4500000026',DraftUUID=guid'00000000-0000-0000-0000-000000000000',IsActiveEntity=true))

- In the upcoming screen Click now on the **copy** button:

![](images/s4prcopy_order.jpg)

- Do not change anything an press finally the **order** button:

![](images/s4prcopy_success.jpg)


## Exercise 2.2 add the SAP Task Center tile to your site

To add now the SAP Task Center web application to your newly created site please check also the official SAP documentation at [SAP Help](https://help.sap.com/docs/task-center/sap-task-center/create-task-center-tile-on-sap-build-work-zone-standard-edition)

For the integration of SAP Task Center into your new page please complete the upcoming steps:

- Enter the **site manager** from SAP Build Work Zone, please have a look on the exercise 1 for the [URL](../ex1/README.md) in case you missed it.
- Switch now over to the **content manager** to identify the content:

![](images/content_manager_access.jpg)

- In the content manager you will see now the already available SAP Task Center apps and also multiple roles like **XP262_001_Role**:

![](images/content_manager_tc.jpg)

- To add now the SAP Task Center App's please **modify** the existing page

![](images/add_tc_widget_to_page.jpg)

-  Select "Tile", to add the "SAP Task Center" tiles to your page.

![](images/widget.jpg)

![](images/add_tc_apps.jpg)

- Switch now back to the **content manager** and select the role to enable the new applications:

![](images/add_apps_to_role.jpg)

After executing successfully these steps you should now have added the **SAP Task Center** tiles to your SAP Build Work Zone site!

Afterwards you can simply select the site manager from the right hand side and launch you site by pressing the "Go to site" icon:

![](images/stc_launch.jpg)

**Congratulations you have now successfully integrated SAP Task Center in your site !!!** :wave:

## Exercise 2.3 Explore the SAP Task Center applications

By entering now your SAP Build Work Zone page as end user, you should now able to see SAP Task Center as part of your page.

![](images/bwz_page.jpg

After you select the SAP Task Center web application you should now see at least one Task in the list:

![](images/taskcenter.jpg)

By selecting now one of these tasks you wil able to see all details similar like in the "local" my inbox in S4HC:

![](images/taskdetail.jpg)

In case you want to see more details of your task click **open App**:

![](images/openapp.jpg)

You will be then automatically logged in via **Single-Sign-On**, based on the usage of **SAP Cloud Identity Services**.

---
> [!NOTE]
> The reason for this seamless integration is that we make use of multiple suite qualities to integrate across our application portfolio. In this specific case we are using the suite quality Consistent Security & Identity Management.

![](images/suite_quality_overview.jpg)
---


Continue to - [Exercise 3 - Excercise 3 ](../ex3/README.md)
