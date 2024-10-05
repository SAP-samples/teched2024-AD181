# SAP Build Apps

## New Purchase Page - Logic for Data Variables

1.  Go to UI Canvas \> Variables \> Data Variables

<img src="images/image1.png"
style="width:6.5in;height:2.24028in" />

2.  Add 2 data variables: A_ProductBasicText and Customers

- Select SAVE

Note: Please make sure that you have same data variable names in your
screen: A_ProductBasicText1 and Customers1

<img src="images/image2.png"
style="width:6.5in;height:2.14722in" />

3.  Select Customers1 data entity. Select the \[X\] icon under Filter
    condition.

<img src="images/image3.png"
style="width:6.5in;height:2.74583in" />

4.  Select Object with Properties

<img src="images/image4.png"
style="width:6.5in;height:2.92569in" />

5.  Add a condition:

    - Property: *customerNumber*.

    - Condition type: *equal*.

    - Select the ‘123’ icon under Compared value

<img src="images/image5.png"
style="width:6.5in;height:2.85625in" />

6.  Go to Formula \> Select into the Formula field

<img src="images/image6.png"
style="width:6.5in;height:3.61111in" />

7.  Enter the formula below and Save the formula afterwards

INTEGER(params.SelectedCustomerNumber)

<img src="images/image7.png"
style="width:6.5in;height:4.26667in" />

8.  Save the condition

<img src="images/image8.png"
style="width:6.5in;height:4.50625in" />

9.  Switch to VIEW.

10. Drag & Drop the UI Components with the following order:

    - Dropdown field

    - Input field

    - Button

<img src="images/image9.png"
style="width:6.5in;height:3.7375in" />

11. Switch to VARIABLES \> PAGE VARIABLES \>

12. Create 2 Page Variables

    - Variable 1: Name: PurchaseValue Variable Value type: number

    - Variable 2: Name SelectedProduct Value type: text

13. Select Save

<img src="images/image10.png"
style="width:6.5in;height:2.09931in" />

14. Switch back to VIEW then:

    - Select Dropdown field.

    - Rename the Label text: Select Product.

    - Select the ‘\[ \]’ icon under Option list.

<img src="images/image11.png"
style="width:6.5in;height:3.91597in" />

15. Go to Formula

16. Enter the formula below

MAP(data.A_ProductBasicText1, {label:item.Product, value:item.Product})

17. Save the Formula

<img src="images/image12.png"
style="width:6.5in;height:3.94931in" />

16. Select the X under Selected value

17. Go to Data and Variables \> Page variable \> SelectedProduct \>
    select Save

<img src="images/image13.png"
style="width:6.5in;height:3.89722in" />

18. Select Input field and Rename label: Purchase Value

19. Select the ‘X’ icon under Value

<img src="images/image14.png"
style="width:6.5in;height:4.17778in" />

20. Go to Data and Variables \> Page variable \> PurchaseValue

21. Select Save

<img src="images/image15.png"
style="width:6.5in;height:3.78403in" />

22. Select Button \> Rename label: Add Points!

23. Open Logic Canvas

<img src="images/image16.png"
style="width:6.5in;height:4.44514in" />

23. Drag & Drop the logic components below to create the logic
    and join each component.

    - Create record

    - Alert

    - Navigate back

24. Select Save

<img src="images/image17.png"
style="width:6.5in;height:2.86458in" />

25. Select Create record function \> Select the data
    entity Purchases and Save.

26. Select the Custom Object

<img src="images/image18.png"
style="width:6.5in;height:3.85486in" />

27. Select the ABC icon under ID \> Formula

28. Select the Formula bar.

<img src="images/image19.png"
style="width:6.5in;height:5.34444in" />

28. Enter the following formula and Save:

GENERATE_UUID()

<img src="images/image20.png"
style="width:6.5in;height:4.23125in" />

28. Select the \[X\] icon under customer_ID \> Formula \> Create formula

<img src="images/image21.png"
style="width:6.5in;height:5.34792in" />

29. Enter the following formula and Save:

data.Customers1\[0\].ID

<img src="images/image22.png"
style="width:6.5in;height:4.2375in" />

30. Select the \[X\] icon under purchaseValue \> Formula \> Create
    formula

<img src="images/image23.png"
style="width:6.5in;height:5.35972in" />

31. Enter the following formula and Save:

INTEGER(pageVars.PurchaseValue)

<img src="images/image24.png"
style="width:6.5in;height:4.24583in" />

32. Select the \[X\] icon under selectedProduct \> Data and Variables \>
    Page Variable \> SelectedProduct

<img src="images/image25.png"
style="width:6.5in;height:5.35486in" />

33. Save the window

<img src="images/image26.png"
style="width:6.5in;height:5.34931in" />

34. Select *Alert* component \> Select the *ABC* icon under Dialog title
    \> Formula

<img src="images/image27.png"
style="width:6.5in;height:3.5375in" />

35. *Copy* and *Paste* (as plain text) the formula below \> Save

data.Customers1\[0\].name + " has successfully earned " +
outputs\["Create record"\].response.rewardPoints + " points!"

<img src="images/image28.png"
style="width:6.5in;height:3.95069in" />

36. Save the project

## [Next Lesson ⎘](../ex3.4/)
