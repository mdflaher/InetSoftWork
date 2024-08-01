# How do I recreate my Excel report with InetSoft's tool?

This document contains instructions on how to recreate your Excel report using InetSoft's Style Intelligence. It covers the most common usage needs for table style reports.

[How do I combine multiple pivot tables into one table?](#pivot)

[How do I include multiple lists in the same table?](#lists)

[How do I group table columns under subheaders?](#sub)




# How do I combine multiple pivot tables into one table? <a name="pivot"></a>

 

This   [multilevel freehand table example](https://www.inetsoft.com/public/app/viewer/view/global/Dashboards/Return%20Analysis%20Table)   uses the Orders Details dataset. This table displays the information that would require three separate pivot tables if made in excel. The goal is to have a combined pivotable that can scroll sideways to see the three tables displayed as one. This table that combines pivot tables displaying orders by month broken down by team and salesperson, product category and product, and company.

![](screenshots/combined-pivot-table1.PNG) ![](screenshots/combined-pivot-table2.PNG) ![](screenshots/combined-pivot-table3.PNG)




Begin by dragging out a freehand table element and selecting 'Edit'.

Then right click on a cell and click 'Insert Row'. 

![](screenshots/insert-row-highlight.png)


Right click on a cell again and select 'Insert Rows/Columns'.

![](screenshots/insert-rows-columns-highlight.png)


Insert 3 extra columns, after the selection.

![](screenshots/insert-extra-rows-columns-highlight.png)

Drag out dimension 'Order Date' into the bottom left cell. 

![](screenshots/order-date-into-bottom-left-column-highlight.png)

Select the cell containing 'Order Date', and set group to the 'Month' level. Set 'Expand Cell' to 'Vertical'.

![](screenshots/set-grouping-to-by-month-highlight.png)



Add dimensions 'Sales Team' and 'Sales Rep' to the cells where they are pictured below.

![](screenshots/add-sales-team-highlight.png)





Make sure that on 'Sales Team', and 'Sales Rep', expand is set to 'Horizontal'.

Add 'Gross Amount' to the bottom cell of the second column.

![](screenshots/add-gross-amount-dimension-highlight.png)

Next, move dimensions 'Category' and 'Product' into the first two cells of the third column. Make sure expand on both is set to Horizontal.

![](screenshots/move-in-category-and-product-highlight.png)



Drag 'Gross Amount' into the bottom cell of the third column.

![](screenshots/drag-out-gross-amount-again-highlight.png)

Select the top two blank cells on the right. Right click  and select 'Merge Cells'.

![](screenshots/merge_cells-highlight.png)

Drag 'Customer' dimension into the merged cells. Make sure it is set on Horizontal.

![](screenshots/drag-customer-into-fourth-space-highlight.png)


Drag 'Gross Amount' measure into the bottom right cell.

![](screenshots/drag-gross-amount-into-fourth-highlight.png)

Click 'Finish'. You now have a freehand table which combines three pivot tables into one. To enhance readability, we are going to set month of the year as a header column. Select the table by clicking on it's header. Right click, select 'Properties'.

![](screenshots/table-properties.PNG)

In the Freehand Table Properties menu, selec the 'Advanced' tab. Under 'Header Columns', enter '1'. Click 'Ok'.

![](screenshots/table-properties-menu.PNG)

You now have a table aggregates order data into rows based on month of the year. The table begins with columns for team and subcolumns for employee.

  ![](screenshots/combined-pivot-table1.PNG)

It then breaks the orders down by columns of product category and product.

![](screenshots/combined-pivot-table2.PNG)

It ends with columns for company.

![](screenshots/combined-pivot-table3.PNG)








# How do I include multiple lists in the same table? <a name="lists"></a>

This example uses the Orders dataset to create combined lists of total sales and product quantities, by product category and region.

![](screenshots/combined-lists.PNG)

Begin by dragging out a freehand table from the left side panel. Click the edit button in the middle of the new table.

![](screenshots/drag-out-freehand-table.PNG)

Select one of the cells in the table representation. Right click, select 'Insert Column'. Right click again, click 'Insert Rows/Columns'.

![](screenshots/right-click-menu.PNG)

Select 'Rows', under 'Number' insert  '2'. Click 'Ok'.

![](screenshots/insert-two-rows.PNG)

Select the top left cell. Make sure 'Text" is selected, type "Product Category" into the accompanying field and press enter.

![](screenshots/insert-category-label.PNG)

 On the left side data panel, open query 'Product" and drag dimension 'Category' into the second to top cell on the left. Make sure 'Expand Cell' is selected, and set to 'Vertical'.
 
![](screenshots/drag-category-into-cell.PNG)

 On the left side data panel, open query 'Customer" and drag dimension 'Region' into the bottom cell on the left. Make sure 'Expand Cell' is selected, and set to 'Vertical'.

![](screenshots/drag-region-into-cell.PNG)

Select the center cell in the top row. Make sure 'Text" is selected, type "Total Sales" into the accompanying field and press enter.

![](screenshots/enter-sales-label.PNG)

 On the left side data panel, open query 'Product" and drag measure 'Total' into the second to top cell second to the left. Make sure 'Summarize' is selected, and set to 'Sum'. Click the pencil icon next to 'Summarize' to see aggregation options. Click the checkmark once 'Sum' has been selected.

![](screenshots/drag-product-total-into-cell.PNG)

Drag dimension 'Total' into the bottom center cell. Make sure 'Summarize' is selected, and set to 'Sum'. Click the checkmark once 'Sum' has been selected.

![](screenshots/drag-product-total-into-bottom-cell.PNG)

Select the top cell on the right. Make sure 'Text" is selected, type "Quantities" into the accompanying field and press enter.

![](screenshots/enter-quantities-label.PNG)

 On the left side data panel, open query 'Product" and drag measure 'Quantity Purchased' into the second to top right cell. Make sure 'Summarize' is selected, and set to 'Sum'. Click the pencil icon next to 'Summarize' to see aggregation options. Click the checkmark once 'Sum' has been selected.


![](screenshots/drag-quantity-purchased-into-cell.PNG)

 On the left side data panel, open query 'Order" and drag measure 'Order:Num' into the second to top cell on the right. Make sure 'Summarize' is selected, and set to 'Distinct Count'. Click the checkmark once 'Distinct Count' has been selected.

![](screenshots/drag-order-number-into-last-cell.PNG)

click 'Finish'. We now have a combined lists of total sales and product quantities, by product category and region.

![](screenshots/combined-lists.PNG)

