# How do I make a chart that switches data bindings back and forth?

This [radio button example](https://www.inetsoft.com/public/app/viewer/view/global/Dashboards/radio%20button) example uses the orders dataset. Drag out a chart and radio button from the left hand panel.


![](screenshots/drag-out-chart-and-button.PNG)


Select the radio button so it is highlighed in orange as shown. Drag out dimensions 'Salesperson:First Name' and 'Customer:Company' into the radio button. Click on the orange squares on either side of the highlighed radio button to stretch the element to a width necessary to show its labels.

![](screenshots/drag-dimensions-into-button.PNG)


Click on the 'Edit' button in the center of the chart. If the Visualization Reccomender appears, select 'Full Editor'.

![](screenshots/select-full-editor.PNG)


In full Chart Editor, drag 'Order:Paid' into the x axis. It should default as a sum.

![](screenshots/drag-order-paid-into-x.PNG)


Drag 'Salesperson:First Name' into the y axis.

![](screenshots/drag-salesperson-into-y.PNG)


Click on the button with an F and X on it next to where 'Salesperson:First Name' was dragged into the y axis. Select 'Variable' in the dropdown that appears. The space for the y axis should now display '$(Radiobutton1)' or whatever name you gave the radio button. 

![](screenshots/change-to-variable.PNG)


Click 'Finish'. You now have a [chart](https://www.inetsoft.com/public/app/viewer/view/global/Dashboards/radio%20button) that defaults as orders by salesperson.

![](screenshots/radio-button-result.PNG)


Click the radio button for 'Supplier:Company' and watch the chart switch to displaying orders by supplier.

![](screenshots/radio-button-result2.PNG)

# How can I let the end user select any data binding?



![](screenshots/edit-button.PNG)
![](screenshots/select-chart-properties.PNG)
![](screenshots/ad-hoc-editing.PNG)
