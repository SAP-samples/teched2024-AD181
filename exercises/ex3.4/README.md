# SAP Build Apps

## Redeem Points Page - Logic for Data Variables

1.  Select New Purchase and Redeem Points

<img src="images/image1.png"
style="width:6.5in;height:3.5125in" />

2.  Drag & Drop the UI Components in the following order:

    - Input field

    - Button

<img src="images/image2.png"
style="width:6.5in;height:2.95694in" />

3.  Switch to Variables \> Page Variables \> Add a Page Variable

4.  Rename as follows:

- Variable Name: RedemptionAmount

- Variable Value type: Number

5.  Save

<img src="images/image3.png"
style="width:6.5in;height:2.72569in" />

4.  Select Data Variables \> ADD DATA VARIABLE \> Customers1

5.  Select X under Filter Condition

<img src="images/image4.png"
style="width:6.5in;height:3.15139in" />

5.  Select Object with Properties

<img src="images/image5.png"
style="width:6.5in;height:3.52153in" />

6.  Select Add Condition and select the following:

- Property: customerNumber

- Condition type: equal

7.  Select ‘123’ icon under Compared value

<img src="images/image6.png"
style="width:6.5in;height:2.89444in" />

7.  Select Formula \> Select the Formula Bar and Enter the following
    formula:

INTEGER(params.SelectedCustomerNumber)

8.  Hit Save twice.

<img src="images/image7.png"
style="width:6.5in;height:4.34931in" />

9.  Change to View and Select Input field

10. Rename label: Redemption Amount

11. Select \[X\] icon under Value

<img src="images/image8.png"
style="width:6.5in;height:4.15972in" />

10. Choose Data and Variables \> Page Variable \> Redemption
    Amount and Save

<img src="images/image9.png"
style="width:6.5in;height:3.96458in" />

11. Select Button \> Rename label: Redeem Points!

<img src="images/image10.png"
style="width:6.5in;height:4.02153in" />

12. Drag & Drop the logic components to create the logic flow shown
    below.

    - Create record

    - Alert

    - Navigate back

13. Join the componants and Save

<img src="images/image11.png"
style="width:6.5in;height:3.59583in" />

13. Select the Create record function

14. Select data entity: Redemptions from the drop down. Save your work

15. Select the Custom Object

<img src="images/image12.png"
style="width:6.5in;height:3.31319in" />

14. Select the ABC icon under ID

- Select Formula

- Select the Formula bar

<img src="images/image13.png"
style="width:6.5in;height:4.01736in" />

15. Enter the following formula and Save:

GENERATE_UUID()

<img src="images/image14.png"
style="width:6.5in;height:3.84236in" />

16. Select the \[X\] icon under customer_ID \> Formula \> Create formula

<img src="images/image15.png"
style="width:6.5in;height:4.06319in" />

17. Enter the following formula and Save:

data.Customers1\[0\].ID

<img src="images/image16.png"
style="width:6.5in;height:3.97292in" />

18. Select the \[X\] icon under redeemedAmount \> Formula \> Create
    formula

<img src="images/image17.png"
style="width:6.5in;height:4.09167in" />

19. Enter the following formula and Save:

INTEGER(pageVars.RedemptionAmount)

<img src="images/image18.png"
style="width:6.5in;height:4.18264in" />

20. Save the window

<img src="images/image19.png"
style="width:6.5in;height:4.06875in" />

21. Select Alert component \> Select the ABC icon under Dialog title \>
    Select Formula

<img src="images/image20.png"
style="width:6.5in;height:2.94306in" />

22. Copy and Paste (as plain text) the formula below and Save

data.Customers1\[0\].name + " has redeemed " +
pageVars.RedemptionAmount + " successfully"

<img src="images/image21.png"
style="width:6.5in;height:3.72639in" />

23. Make sure to save your work - Top right!

## [Next lesson](../ex3.5/)
