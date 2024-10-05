# SAP Build Apps

## Authentication and Data Integration

1.  Select the page name written in blue at the top left corner of your
    page. Go to the page: New Purchase

<img src="images/image1.png"
style="width:6.5in;height:3.08333in" />

2.  Go to the AUTH tab \> Enable Authentication

<img src="images/image2.png"
style="width:6.5in;height:2.66667in" />

3.  Select SAP BTP authentication \> OK

<img src="images/image3.png"
style="width:6.5in;height:4.03125in" />

4.  Go to the DATA tab \> Add Integration

<img src="images/image4.png"
style="width:6.5in;height:5.02917in" />

5.  Select BTP Destinations

<img src="images/image5.png"
style="width:6.5in;height:2.35417in" />

6.  Select your Build Code project named **customer_loyalty-customer_loyaltySrv**

<img src="images/image6.jpg" />

7. In case you receive an error message "Request failed with status code 404", your Build Code app may be stopped. If you do not have this error, skip this step.

- In the subaccou t, go to **Cloud Foundry > Spaces** and click the **dev** space

- Select **Applications**

- If **customer-loyaltySrv** is stopped, click the **Start** button on the right.

- Repeat Step 6 above

<img src="images/image9.jpg" />

8.  In SAP Build Apps, Select Install Integration

<img src="images/image7.png" style="width:6.5in;height:4.11042in" />

9.  Select Enable Data Entity for all four (4) Data entities listed on
    the left:

    - Customers

    - Purchases

    - Redemptions

    - A_ProductBasicText

10.  Select Save

<img src="images/image8.png" style="width:6.5in;height:2.26528in" />

## [Next Lesson ⎘](../ex3.3/)
