# SAP Build Code and Joule Copilot

## Create Data Entities with Joule

In this lesson, we will create the data model and the services for the
customer loyalty program application.

We could create the data model visually from the Storyboard or by
writing the code manually. However, we are going to use the generative
AI capabilities of Joule and SAP Build Code to generate the code. Thus,
significantly reducing the time and effort required to develop the
customer loyalty program application.

1.  Launch the Joule digital assistant.

    - Please wait for the digital assistant to open. If it fails to open
      then please refresh your browser.

<img src="images/image1.png"
style="width:6.5in;height:4.46528in" />

2.  Please ask Joule to generate a CAP application by
    entering /cap-gen-app into the prompt.

<img src="images/image2.png"
style="width:6.5in;height:3.96389in" />

3.  Generate the data model and services by copying and pasting the
    prompt into the box where it says ‘Describe what you need to do’.

```
Design a customer loyalty program application. Define 3 data entities:
Customers, Purchases and Redemptions. Each customer must have the
following fields: name, email, 7-digit customer number, total purchase
value, total reward points, and total redeemed reward points. All fields
for each customer should be integer except name and email that will be
stored as string. Purchases should include the following fields:
purchase value, reward points and selected product. All fields in
Purchases must be integer except selected product. Redemptions must have
1 field in integer: redeemed amount. Each purchase and redemption will
be associated to a customer. Create 5 rows for each entity.
```

4.  Select Generate.

<img src="images/image3.png"
style="width:6.5in;height:4.55347in" />

5.  The code should be generated now below your prompt.

<img src="images/image4.png"
style="width:6.5in;height:6.07847in" />

6.  Select Accept.

<img src="images/image5.png"
style="width:6.5in;height:3.49028in" />

7.  Once the code is accepted, the update will be reflected on
    the Storyboard.

<img src="images/image6.png"
style="width:6.5in;height:3.06042in" />

8.  Joule has generated a service interface for you, containing the top-level Customers entity. For our exercise, we also want to expose the Purchases and Redemptions entities.

    - Select the **Customer_Loyalty_\<INITIALS\>** service in the storyboard

    - Select **Opean in Graphical Modeler**

<img src="images/image7.jpg" />


9.  This opens the graphical service modeler, where you will see the details of the Customers entity. Add the Purchases entity to the service model:

    - Select **Add Entity**

    - Click on the canvas to place the new entity

<img src="images/image8.jpg" />

9.  The properties panel on the right will open. To add the Purchases entity:

    - In the dropdown, select the **Purchases** entity

    - Click on the checkmark button to save the entity

<img src="images/image9.jpg" />

10.  Repeat Step 9 to also add the Redemptions entity. Your completed model should look like this:

<img src="images/image10.jpg" />

And your storyboard will also show all of your exposed services:

<img src="images/image11.jpg" />

## [Next Lesson ⎘](../ex1.3/)
