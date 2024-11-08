# Prepare & Deploy CAP Application

## Deployment

The final step in SAP Build Code is to deploy the application to
CloudFoundry. This process also involves the automatic creation of
destinations, enabling ODATA services to be utilised by other tools such
as SAP Build Apps.

1.  For the deployment go to Task Explorer and select the Play icon
    (Run) next to the **Enable Discovery and Deploy** option.

    - Please be patient as this may take a few minutes.

<img src="images/image1.png"
style="width:6.34722in;height:6.65278in" />

2. You will be prompted for several build configuration values:

- For UI5 Version, select the latest (currently **1.130.0**)

<img src="images/image3.jpg" />

- For UI5 Theme, select **sap_fiori_3**

<img src="images/image4.jpg" />

- For Vendor Dependency, select **No**.

<img src="images/image5.jpg" />

- For Build Code Service Plan, select **No**.

<img src="images/image6.jpg" />

3. Building the app will take a minute or two. After building the app, a new tab will be opened to to sign into Cloud Foundry for deployment.

- Select **SSO Passcode** for the authentication methods

- Click on the link **Open a new browser page to generate your SSO passcode**. A new browser tab will open.

<img src="images/image16.jpg" />

4. If you are prompted to login using sap.ids, select **Sign in to another account** (you may not be prompted for this).

<img src="images/image17.jpg" />

4. Log into the cloud foundry environment:

- For the origin key of the alternate identity provider, enter **lcap-platform**

- Select **Sign in with alternate identity provider**

<img src="images/image2.jpg" />

5. Copy the Temporary Authentication Code.

<img src="images/image18.jpg" />

6.  Paste the code and Sign In.

<img src="images/image19.jpg" />

7. Set the Cloud Foundry deployment target:

- For Cloud Foundry Organization, select **TechEdLCAP_lcapteched**

- For Cloud Foundry Space, select **dev**

- Click **Apply**

<img src="images/image20.jpg" />

8. After the successful deployment (may take several minutes) the terminal will indicate that the Build/Deploy task has completed and that your service is discoverable.

<img src="images/image7.jpg" />

9. Near the bottom of the terminal, there will be a link **Project Overview URL**. This link will allow you to access the deployed application UI and services.

- Use **Ctrl+Click** (PC) or **Cmd+Click** (Mac) to try it out!

<img src="images/image21.jpg" />

10. Explore the UIs that you have created

<img src="images/image14.jpeg" style="width:6.5in;height:3.74375in" />

11. Select Go in each of the tiles (Customers, Purchases. Redemptions)
    in the Customer Loyal UI to see the generated data.

<img src="images/image15.png" style="width:6.5in;height:3.03056in" />

Congratulations! You have used the generative AI capabilities of Joule
in SAP Build Code, to create a CAP service for a customer loyalty
program application.

## [Next Lesson ⎘](../ex3/)