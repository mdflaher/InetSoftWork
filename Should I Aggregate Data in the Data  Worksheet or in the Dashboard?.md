# Beneifits of leaving aggregation to the dashboard

One thing to consider is that if your data is coming into the dashboard pre-aggregated, the 'Show Details' function on a chart or crosstab will often end up showing the same level of detail that the chart or crosstab provides, not giving any further layer of granularity.
The main benefit of leaving the data at the transactional/detail level is that by leaving the greatest level of detail available you can have build a dashboard with a large variety of output elements all grouping and summarizing the data in completely different ways without having to work around whatever way the data is pre-aggregated. Performing calculations on pre calculated data can be problematic. When attempting to build the same dashboard with pre-aggregated data, you may find that a calculation can be in contrast to how the data was pregrouped and summarized it in the data layer.  For example if data was preaggrated as averages of records across a variety of dimensions, record count would be an unavailable metric. SO pre aggregating makes the data less flexible when it comes to design choices.  


When you leave your data at the detail level and do your aggregations in dashboard output elements like charts and crosstabs, you can give your users the full benefit of ad hoc editing, letting them change chart dimensions and calculation levels and types.
Many InetSoft users will begin with complicated pre aggregated queries coming in from their database, only to find that these are only good for one dashboard output element. Once they see the kind of aggregations and summations that can be performed in the dashboard, they end up de-aggregating their data at the source and leaving the aggregation to the dashboard. Leaving your dat at the detail level gives dashboard designers greater flexibility to change metrics without having to go back to the data layer.  Using the same data worksheet for many different dashboards can reduce the worktime on dashboard development and also help preserve the integrity of the data.
Date volume, mixing granularity, step through calulations. .


For this reason we enncourage users to as much aggregation to the dashboard level as is possible, as otherwise data can be pre summarized to a level to leave little flexibility and no drilldown capability. However, there are certain types of use cases in which aggregation will need to be done at hte worksheet level instead of the dashboard level. These use cases will be described in the next section.

# When to pre-grouped and summarized data in the worksheet

When your use of analytics involveindustry or company specific calculations and you are concerned about them being performed in the correct way, it's better to lock off these aggregations in  a data worksheet to make sure employees are using the calculations correctly. An added benefit is that these calculations could be changed at companywide level by changing the single worksheet, resulting in an update to all the dashboards pulling the calculation from the single worksheet.
Also reduces data volume. 
Not all data needs to be looked at at the transactional level by all your users
Pre aggregating can save space on a materialized view

# Cases where pre-aggregation is necessary
If you’re doing a mashup of different levels of detail data you d want to do in the worksheet. You could have detail level data and nongralular data such as goal numbers. Or important companywide numbers such as budgets
Might want to compare individual transactions to sales goals
For this youd do a mashup in the worksheet but with mashing up sum numbers to detail levels youd add a column that’s not applicable since its an aggregate in a detail row, so you can pre aggregate the data to match the sum values yourre comparing them too
Sometimes the only way to do the layered calculation desired is to presummaryize at a certain level
Also need worksheet for step through calculation, such as column for fields max value  to be included at detail level for calculation
Sum counts and quantities  can be useful for comparing to detail level for calculating ratios
Worksheet calculations for either aligning data from different locations at different levels of details, combining without double counting or summing of values, mashup in worksheet for combined displays or step thorugh calculations
Multiple stage calculations

These are instances where the data must go through multiple separate then combined levels of calculations
Will depend on whats aggregated already at the datasource
Introduce mashup as well
What are the options for hiding aggregate columns?
What about using multiple queries?
Comparative analysis from different sources of granularity, making sure the binding and math at dashboard level is as simple and straightforward as possible

if you can, best to not sell yourself short on design flexibility. Leave it to dashboard levelif you don’t have different  queries at different levels of granularity, don’t need to reduce data volume, you can give the users show details capability and the most flexibility with different types of summarizations and different combinations of dimensions


