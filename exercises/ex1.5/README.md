# SAP Build Code and Joule Copilot

In this lesson, we will connect to an S4/HANA system to retrieve the
product related data. To simplify the setup, we will be using a sandbox S/4 HANA instance available through the **SAP Business Accelerator Hub**, leveraging the [Product Master (A2X)/Basic Text API](https://api.sap.com/api/API_PRODUCT_SRV/overview/). We will connect to this API through a BTP destination.

## Add External Data Resource

We'll connect to the S/4 Product API through the Service Center.

1.  In Service Center go to SAP System and find the BTP
    destination S4HANA_Joule_Product (S/4 Product).

    - Click the **Service Center** Icon on the tool bar on the left

    - Select **SAP System**

    - Enter **S4HANA** to filter the systems

    - Select **S4HANA_Joule_Product**. The service definition will open.

    - Select **Add to CAP Project**

<img src="images/image1.jpg" style="width:6.5in;height:4.26528in" />

3.  Go to Storyboard and check if the External Resource got updated.

Note: It may take a short time to update!

<img src="images/image2.png" style="width:6.5in;height:2.29097in" />

4.  We want to expose this entity through our service interface. 

    - Go to service.cds tab and Add Entity (select a service and Open Graphic Modeler if it is not open)

    - You can drop the new entity anywhere

<img src="images/image3.png"
style="width:6.5in;height:4.08472in" />

5.  Select the data entity: S4HANA_Joule_Product.A_ProductBasicText

    - Disable the Enable draft editing option.

6.  Select Save

<img src="images/image4.png"
style="width:6.5in;height:3.87222in" />

## [Next Lesson ⎘](../ex1.6/)