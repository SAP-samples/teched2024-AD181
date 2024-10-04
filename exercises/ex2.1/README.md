# Prepare & Deploy CAP Application

## Deployment

The final step in SAP Build Code is to deploy the application to
CloudFoundry. This process also involves the automatic creation of
destinations, enabling ODATA services to be utilised by other tools such
as SAP Build Apps.

1.  For the deployment go to Task Explorer and select the Play icon
    (Run) next to Enable Discovery and Deploy option.

    - Please be patient as this may take a few minutes.

<img src="images/image1.png"
style="width:6.34722in;height:6.65278in" />

2.  Check if the task has launched in the terminal

<img src="images/image2.png"
style="width:6.5in;height:2.44722in" />

3.  During the deployment a new page will be opened to to sign into
    Cloud Foundry.

<img src="images/image3.png"
style="width:6.5in;height:6.4375in" />

4.  Please note that this is a shared landscape so we need to minimise
    the size of your application. Before deploying the application to
    Cloud Foundry, we need to set the memory footprint of the
    application.

    - Select the EXPLORER icon and open the mta.yaml file.

<img src="images/image4.png"
style="width:6.5in;height:3.72569in" />

- Search the memory parameter of your application and change the value
  to 64MB.

<img src="images/image5.png"
style="width:6.5in;height:3.38889in" />

- Right select the mta.yaml file and select Build MTA Project

<img src="images/image6.png"
style="width:6.5in;height:5.59306in" />

- When the job is complete, the following message is printed to
  the Terminal.

<img src="images/image7.png"
style="width:6.5in;height:2.08958in" />

5.  Return to the Cloud Foundry Sign In and Targets page.

    - Enter the correct
      endpoint: https://api.cf.eu10-004.hana.ondemand.com

    - Select Open a new browser page to generate your SSO passcode

<img src="images/image8.png" style="width:6.5in;height:6.475in" />

6.  Enter academy-platform and select Sign in with alternative identity
    provider.

<img src="images/image9.png"
style="width:6.5in;height:6.39792in" />

7.  Copy the Temporary Authentication Code.

<img src="images/image10.png"
style="width:6.5in;height:2.77014in" />

8.  Paste the Code and Sign In.

<img src="images/image11.png"
style="width:6.5in;height:6.56181in" />

9.  Select the Organization and Space as specified here:

    - Organization: sap-build-code-eu10

    - Space: AC_SAPBUILD

    - Select Apply

<img src="images/image12.png"
style="width:6.5in;height:6.29792in" />

10. After the successful deployment (May take several minutes) you will
    find the link of the deployed application in the terminal.

- Use Ctrl+click to try it out!

<img src="images/image13.jpeg"
style="width:6.5in;height:3.62778in" />

11. Explore the UIs that you have created

<img src="images/image14.jpeg"
style="width:6.5in;height:3.74375in" />

12. Select Go in each of the tiles (Customers, Purchases. Redemptions)
    in the Customer Loyal UI to see the generated data.

<img src="images/image15.png"
style="width:6.5in;height:3.03056in" />

Congratulations! You have used the generative AI capabilities of Joule
in SAP Build Code, to create a CAP service for a customer loyalty
program application.

## [Next Lesson ⎘](../ex3/)