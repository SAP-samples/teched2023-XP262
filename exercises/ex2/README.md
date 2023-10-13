# Exercise 2 - Integrate and explore SAP Task Center

In this exercise, we will create a **purchase requisition** in SAP S/4HANA Cloud to get a Task for the PR approval in **SAP Task Center**.

## Exercise 2.1 create a purchase requisition in SAP S/4HANA Cloud

- To create a PR in S4HC please enter the following URL (https://s4hanacloudurl//ui#PurchaseOrder-manage&/C_PurchaseOrderTP(PurchaseOrder='4500000023',DraftUUID=guid'00000000-0000-0000-0000-000000000000',IsActiveEntity=true))

![](images/s4prcopy.jpg)

- In the upcoming screen Click now on the **copy** button:

![](images/s4prcopy_order.jpg)

- Do not change anything an press finally the **order** button:

![](images/s4prcopy_success.jpg)


## Exercise 2.2 add the SAP Task Center tile to your site

To add now the SAP Task Center web application to your newly created site please check also the official SAP documentation at [SAP Help](https://help.sap.com/docs/task-center/sap-task-center/create-task-center-tile-on-sap-build-work-zone-standard-edition)

To integrate the SAP Task Center applications into your new page please complete now these steps:

- Enter the site manager from SAP Build Work Zone [URL see Excercise 1](../ex1/README.md)
- Switch now over to the content manager to identify the content:

![](images/content_manager_access.jpg)

- In the content manager you will see now the already available SAP Task Center apps and also multiple roles like **XP262_001_Role**:

![](images/content_manager_tc.jpg)

- To add now the SAP Task Center App's please **modify** the existing page

![](images/add_tc_widget_to_page.jpg)

-  Select "Tile", to add the "SAP Task Center" tiles to your page.

![](images/widget.jpg)

![](images/add_tc_apps.jpg)

- Enable now the new applications in your role:

![](images/add_apps_to_role.jpg)

After executing successfully these steps you should now have added the **SAP Task Center** tiles to your SAP Build Work Zone site!

Afterwards you can simply select the site manager from the right hand side and launch you site by pressing the "Go to site" icon:

![](images/stc_launch.jpg)

After completing these steps you have now successfully integrated SAP Task Center in your site !!!


2.	Click here.


Continue to - [Exercise 3 - Excercise 3 ](../ex3/README.md)
