Should I aggregate my data in the data worksheet, or in the dashboard itself? This document addresses the pros and cons of both approaches and describes cases where one approach is required.

[What are the benefits of leaving aggregation to the dashboard level?](#dash)

[What are the benefits of doing aggregation at the worksheet level?](#work)

[Types of use cases where doing aggregation in the worksheet is necessary](#work2)

[Summary](#sum)

# Benefits of leaving aggregation to the dashboard <a name="dash"></a>

One thing to consider is that if your data is coming into the dashboard pre-aggregated, the 'Show Details' function on a chart or crosstab will often end up showing the same level of detail that the chart or crosstab provides, not giving any further layer of granularity.

The main benefit of leaving the data at the transactional/detail level is that by leaving the greatest level of detail available you can have build a dashboard with a large variety of output elements all grouping and summarizing the data in completely different ways without having to work around whatever way the data is pre-aggregated.

Performing calculations on pre calculated data can be problematic. When attempting to build the same dashboard with pre-aggregated data, you may find that a desired calculation can be in contrast to how the data was pregrouped and summarized it in the data layer.  For example if data was pre-aggrated as averages of records across a variety of dimensions, record count would be an unavailable metric. SO pre aggregating makes the data less flexible when it comes to design choices.  


When you leave your data at the detail level and do your aggregations in dashboard output elements like charts and crosstabs, you can give your users the full benefit of ad hoc editing, letting them change chart dimensions and calculation levels and types.

Many InetSoft users will begin with complicated pre-aggregated queries coming in from their database, only to find that these are only good for one dashboard output element. Once they see the kind of aggregations and summations that can be performed in the dashboard, they end up de-aggregating their data at the source and leaving the aggregation to the dashboard. Leaving your data at the detail level gives dashboard designers greater flexibility to change metrics without having to go back to the data layer.  Using the same data worksheet for many different dashboards can reduce the worktime on dashboard development and also help preserve the integrity of the data.



For this reason we enncourage users to leave as much aggregation to the dashboard level as is possible, as otherwise data can be pre-summarized to a level which leaves little flexibility and no drilldown capability. However, there are certain types of use cases in which aggregation will need to be done at the worksheet level instead of the dashboard level. These use cases will be described in the next section.

# When to pre-group and summarized data in the worksheet <a name="work"></a>

When your use of analytics involveindustry or company specific calculations and you are concerned about them being performed in the correct way, it's better to lock off these aggregations in  a data worksheet to make sure employees are using the calculations correctly. An added benefit is that these calculations could be changed at companywide level by changing the single worksheet, resulting in an update to all the dashboards pulling the calculation from the single worksheet.
Also reduces data volume. 
Not all data needs to be looked at at the transactional level by all your users
Pre aggregating can save space on a materialized view

# Cases where pre-aggregation is necessary <a name="work2"></a>
If you’re doing a mashup of different levels of detail data you'd want to do in the worksheet. There may be instances where you are performing calculations with detail level data and nongralular data such as goal numbers, or important companywide numbers such as budgets.  For example, you may be comparing aggregate sales transactions to sales goals.

For this youd do a data mashup in the data worksheet. However. mashing up sum numbers with detail level  would add a column that’s not applicable since its an aggregate in a detail row. For this reason it'd make more sense to pre aggregate the data to match the sum values yourre comparing them too.
The worksheet is also needed for step through calculation, such as adding a column for a fields max value. This would be needed to perform the detail level calculation of comparing individual values to the max value. Sums, counts, and other quantities can be useful as detail level rows for calculating ratios against detail cells.

So worksheet calculations are necessary for either aligning data from different locations at different levels of details, combining data without double counting or summing of values, multiple stage calculations, combined displays or step thorugh calculations.

# Summary <a name="sum"></a>


If you can, best to leave aggregation to the dashboard and not sell yourself short on design flexibility,  giving your users the most flexibility with different types of summarizations and different combinations of dimensions as well as full 'Show Details' capability.  However there are instances where the data must go through multiple separate then combined levels of calculations, in which case it is necessary to perform the aggregation in the worksheet. So leave it to dashboard level if you don’t have different  queries at different levels of granularity.

