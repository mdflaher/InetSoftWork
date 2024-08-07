The date comparison utility allows a designer or end user to compare measures (numeric values) for two or more date ranges. This document demonstrates the most common use cases. A live [online example](https://www.inetsoft.com/public/app/viewer/view/global/Dashboards/Date%20Comparison) is provided that you can play along with.

For charts and crosstabs with a date dimension, Date Comparsion becomes available on the component's built-in menu. In the example,
right click on the chart to see a menu of options, click on 'Date Comparison'

![](screenshots/right-click-menu.PNG)
<br/>
Clicking 'Date Comparison' will bring up the Date Comparison dialog box.

![](screenshots/date-comparison-dialog.png)

# Most Common Date Comparisons
[How do I compare the most recent week in a dataset to the same week last year?](#week)

[How do I compare this past week to the previous week?](#previous)

[How do I calculate percent change year over year in a table?](#table)

[How do I compare two arbitrary periods?](#nonconsecutive)





## How do I compare the most recent week in a dataset to the same week last year? <a name="week"></a>
[Instructions](#inst1)

Similar case #1 [When displaying the percent change from the same week last year](#percent)

Similar case #2 [When displaying the percent change and change in value together](#percentplus)

Similar case #3 [When comparing the current week to the same week last year](#prev1)

Similar case #4 [When comparing this past month to the same month last year](#month)

Similar case #5 [When comparing this past month to the same month for the past five years](#five)

Similar case #6 [When starting with a previous month](#prev2)

Similar case #7 [When starting from the middle of a week](#middle1)

Similar case #8 [When comparing periods of multiple weeks](#multiple1)




### Instructions<a name="inst1"></a>

The example is performed using the dashboard linked [here](https://www.inetsoft.com/public/app/viewer/view/global/Dashboards/Date%20Comparison)

Make sure you are on the 'Standard Periods' tab.  In the first two dropdown menus, the type and number of date periods included are selected. For this example, enter '2' In 'Previous', and select 'Years' in the second dropdown menu. Uncheck box for 'Today' since the dataset does not cover today's date. Instead, enter the range end date for the data. In this example, the range end date is 2022-5-28 . Check the box for 'Include Year For End Date'. Uncheck 'From Beginning of Each Year To...' since we want to compare the full previous year.

![](screenshots/compare-two-previous-years.PNG)

<br/>

The next dropdowns cover which periods are being compared and in what units of time. Select 'Same Week' under 'Compare Data of',  'Year' in 'For Each', and 'Week' under 'Granularity'. Check box for 'Use Range End Date'. Click 'Ok'.

![](screenshots/compare-same-week.PNG)
<br/>
The chart should change to show only the two data points, one for the most recent week, and one for the same week last year.

![](screenshots/compare-same-week-result.PNG)

## How do I display the percent change between both weeks?<a name="percent"></a>

Perform the steps above, except where it says 'Display' select '%Change'.

How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/percent-change-both-weeks.PNG)  |  ![](screenshots/percent-change-both-weeks-result.PNG)


## How do I display the percent change alongside the change in value?<a name="percentplus"></a>

Perform the steps above, except where it says 'Display' select '%Change & Value'.

How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/percent-change-plus.PNG)  |  ![](screenshots/percent-change-plus-result.PNG)

## How do I compare this current week to the same week last year?<a name="prev1"></a>

Perform the steps above, except where it says 'Range End Date' check the box for 'Today' .
How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/compare-current-week.PNG)  |  ![](screenshots/compare-current-week-result.PNG)

## How do I compare this past month to the same month last year? <a name="month"></a></a>
Select 'Same Month' under 'Compare Data of',  'Year' in 'For Each', and 'Month' under 'Granularity'. Check box for 'Use Range End Date'. Click 'Ok'.
How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/compare-current-month.PNG)  |  ![](screenshots/compare-current-month-result.PNG)
## How do I compare this past month to the same month of the past five years? <a name="five"></a><a name="five"></a>
Enter '5' In 'Previous', and select 'Years' in the second dropdown menu. Select 'Same Month' under 'Compare Data of',  'Year' in 'For Each', and 'Month' under 'Granularity'. Check box for 'Use Range End Date'. Click 'Ok'.
How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/same-month-five-years.PNG)  |  ![](screenshots/same-month-five-years-result.PNG)
##  How do I compare a previous month to the same month last year?<a name="prev2"></a>
Perform the steps above, except where it says 'Range End Date' uncheck the box for 'Today' and instead manually enter the last day of the month you want to compare with the same month last year.
How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/compare-same-month.PNG)  |  ![](screenshots/compare-same-month-result.PNG)

## How do I compare the past seven days starting in the middle of the week to the same period last year?<a name="middle1"></a>
Use the  [Custom Periods](#arb) tab and enter date ranges of the seven day periods you want to compare.
How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/compare-seven-days.PNG)  |  ![](screenshots/compare-seven-days-result.PNG)
## How do I compare the past two or three weeks with the same period last year?<a name="multiple1"></a>
Use the  [Custom Periods](#arb) tab and enter the start and end date of the periods you want to compare.
How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/compare-three-weeks.PNG)  |  ![](screenshots/compare-three-weeks-result.PNG)



<br/><br/><br/>




# How do I compare this past week to previous week? <a name="previous"></a>
[Instructions](#inst2)

Similar case #1 [When comparing a current month to previous month](#prev3)

Similar case #2 [When comparing seven day periods starting in the middle of the week](#rolling)


### Instructions<a name="inst2"></a>

The example is performed using the dashboard linked [here](https://www.inetsoft.com/public/app/viewer/view/global/Dashboards/Date%20Comparison)

Right click on the chart to see a menu of options, click on 'Date Comparison'.

![](screenshots/right-click-menu.PNG)
<br/>
Make sure you are on the 'Standard Periods' tab.  Enter '1' in 'Previous' and select 'Weeks' in the dropdown menu. Check box for 'Today' and 'Include Week For End Date'. Uncheck the box for 'From Beginning of Each Week To...'

![](screenshots/compare-one-week.PNG)

<br/>

Select 'All' under 'Compare Data of', and 'Week' under 'Granularity'. Click 'Ok'.

![](screenshots/compare-past-two-weeks.PNG)
<br/>
The chart should change to show only the two data points, one for the most recent week, and one for the same week last year.

![](screenshots/compare-past-two-weeks-result.PNG)

### How do I compare this past month to the previous month?<a name="prev3"></a>

Follow the instructions above, except select 'Months" instead of 'Weeks' in both dropdowns.
How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/current-to-previous-month.PNG)  |  ![](screenshots/current-to-previous-month-result.PNG)

### How do I compare the past two seven day periods, starting in the middle of the week?<a name="rolling"></a>

Use the  [Custom Periods](#arb) tab and enter the start and end date of the periods you want to compare.
How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/current-to-previous-week.PNG)  |  ![](screenshots/current-to-previous-week-result.PNG)

# How do I calculate percent change year over year in a table? <a name="table"></a>

[Instructions](#taleinst)

Similar case #1 [When comparing this past month to the same month last year](#month2)

Similar case #2 [When starting from the middle of a month](#middle3)

Similar case #3 [When starting with a previous month](#prev4)

Similar case #4 [When comparing periods of multiple months](#multiple3)



## Instructions<a name="taleinst"></a>



This example will use the crosstab table in the product return dashboard found in the InetSoft gallery


[here](https://www.inetsoft.com/evaluate/bi_visualization_gallery/dashboard.jsp?dbIdx=9)

![](screenshots/product-return-table.PNG)

Click on the ... button on the top right corner of the table to access menu options. Click 'Date Comparison'.

![](screenshots/table-menu.PNG)

Make sure you are on the 'Standard Periods' tab.  Enter '2' in 'Previous' and select 'Years' in the dropdown menu. Check box for 'Today' and 'Include Year For End Date'. Uncheck the box for 'From Beginning of Each Year To...'

![](screenshots/table-compare-past-two-years.PNG)

Select 'All' under 'Compare Data of', and 'Year' under 'Granularity'. Select '%Change & Value'. Click 'Ok'.


![](screenshots/table-percent-change-and-value.PNG)

The table should update with the most recent year displaying the original aggregates plus the percent change from the previous year.

![](screenshots/table-date-comparison-plus-percent.PNG)

## How do I compare this past month to the same month last year? <a name="month"></a><a name="month2"></a>
Select 'Same Month' under 'Compare Data of',  'Year' in 'For Each', and 'Month' under 'Granularity'. Check box for 'Use Range End Date'. Click 'Ok'.
How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/table-compare-past-month.PNG)  |  ![](screenshots/table-compare-past-month-result.PNG)
##  How do I compare a previous month to the same month last year?<a name="prev4"></a>
Perform the steps above, except where it says 'Range End Date' uncheck the box for 'Today' and instead manually enter the last day of the month you want to compare with the same month last year.
How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/table-compare-previous-month.PNG)  |  ![](screenshots/table-compare-previous-month-result.PNG)
##  How do I compare the past thirty days starting in the middle of the month to the same thirty days last year?<a name="middle3"></a>
Use the  [Custom Periods](#arb) tab and enter the start and end dates of both thirty day periods.
How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/table-past-thirty-days.PNG)  |  ![](screenshots/table-past-thirty-days-result.PNG)
## How do I compare the past two or three months with the same months last year?<a name="multiple3"></a>
Use the  [Custom Periods](#arb) tab and enter the start and end dates of the periods you want to compare.
How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/table-past-three-months.PNG)  |  ![](screenshots/table-past-three-months-result.PNG)


# How do I compare two arbitrary periods?<a name="nonconsecutive"></a>

[Comparing Arbitrary Periods](#arb)

[Instructions](#inst3)

Similar case #1 [Adding additional periods for comparison](#add)

## Comparing Arbitrary Periods with the Custom Periods Tab<a name="arb"></a>
In addition to comparing nonconsecutive months, the Custom Periods tab can also be used for other comparisons of arbitrary periods, such as comparing the past 7 days starting in the middle of the week, the past 30 days starting in the middle of a month, or comparing clusters of multiple weeks or months. Follow the directions below but enter date ranges that address your query.
![](screenshots/add-additional-custom-ranges.PNG)

## Instructions<a name="inst3"></a>
This example will show how to compare two nonconsecutive months from the same year. Right click on the chart to see a menu of options, click on 'Date Comparison'.

![](screenshots/right-click-menu.PNG)
<br/>
If you want to compare two nonconsecutive months, such as March and May, of the same year or different years, click the 'Custom Periods' tab on the top right of the Date Comparison menu. When in the 'Custom Periods' tab, enter the start and end dates of the months you want to compare and click 'OK'.

![](screenshots/compare-non-consecutive-months.PNG)

The chart should change to show only the two data points, one for each month you entered the date ranges of.

![](screenshots/compare-non-consecutive-months-result.PNG)

##  How do I compare three or more months?<a name="add"></a>
You may compare as many periods as you like in the 'Custom Periods' tab, click the + button underneath the visible date ranges to add more periods.

How To             |  Result
:-------------------------:|:-------------------------:
![](screenshots/compare-three-custom-periods.PNG)  |  ![](screenshots/compare-three-custom-periods-result.PNG)



