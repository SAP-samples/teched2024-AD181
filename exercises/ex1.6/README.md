# SAP Build Code and Joule Copilot

## UI Application

In this lesson, you’ll design a user interface to showcase and test the
content we’ve developed for the customer loyalty program application.

1.  Go back to the Storyboard and add a first UI application by
    selecting the (+)

<img src="images/image1.jpeg"
style="width:6.5in;height:2.55278in" />

2.  We will start with the user interface for the data
    entity *Purchases*. Enter the following values:

    - Display name: Purchases

    - Description: Manage Purchases

    - Data Source: customer_loyaltySrv

<img src="images/image2.jpeg"
style="width:6.5in;height:4.39444in" />

3.  Select Next

<img src="images/image3.png"
style="width:1.45833in;height:0.68056in" alt="Next" />

4.  Select Template-Based Responsive Application as the UI Application
    type.

<img src="images/image4.jpeg"
style="width:6.5in;height:4.20347in" />

5.  Select Next

<img src="images/image3.png"
style="width:1.45833in;height:0.68056in" alt="Next" />

6.  Select List Report Page

<img src="images/image5.jpeg"
style="width:6.5in;height:2.90764in" />

7.  Select Next

<img src="images/image3.png"
style="width:1.45833in;height:0.68056in" alt="Next" />

8.  Select the Purchases entity

9.  Select Finish

<img src="images/image6.jpeg"
style="width:6.5in;height:4.85417in" />

10. Close the Page Map if needed.

Repeat the same steps with the *Customer* and *Redemption* entity.

Customer:

- Display name: Customers

- Description: Manage Customers

- Data Source: customer_loyaltySrv

- UI Application type: Template-Based Responsive Application

- UI Application Template: List Report Page

- Main Entity: Customers

Wait for the UI to create.

Redemptions:

- Display name: Redemptions

- Description: Manage Redemptions

- Data Source: customer_loyaltySrv

- UI Application type: Template-Based Responsive Application

- UI Application Template: List Report Page

- Main Entity: Redemptions

Wait for the UI to create. You shoud see a message, that the files have
been generated.

<img src="images/image7.png"
style="width:3.26389in;height:0.68056in" />

Modify the UI for the Purchases

Now we are going to modify the UI for the purchases. We will include the
products from S/4HANA as value help in the purchases and hide some
fields.

1.  Go back to the Storyboard.

2.  Select the Purchases UI and open it in the Page Map.

    - To see which is the Purchases UI, move mouse pointer over the UI
      to extend the displayed name.

<img src="images/image8.jpeg"
style="width:6.5in;height:2.00417in" />

3.  We want to modify the Object page. Therefore select the edit icon

<img src="images/image9.jpeg"
style="width:6.5in;height:3.00417in" />

4.  In the Sections, expand General Information then expand Form and
    then expand Fields.

- Afterwards it will look like this:

<img src="images/image10.jpeg"
style="width:6.5in;height:5.09653in" />

The reward points are calculated automatically by the logic Joule has
created for us.

5.  Delete the Reward Points field by pressing the trash bin icon next
    to it and Confirm the deletion.

<img src="images/image11.jpeg"
style="width:6.5in;height:3.27222in" />

Instead we want to select the products from S/4HANA for the purchases.

6.  Select the field Selected Product and change the Display Type in the
    properties on the right side to Value Help.

Set the following:

- Label: Product

- Value Source Entity: A_ProductBasicText

- keep the rest as it is.

7.  Select Apply

<img src="images/image12.jpeg"
style="width:6.5in;height:3.91319in" />

## [Next Lesson ⎘](../ex1.7/)