# Should I use a table or a crosstab?

 You can begin your search for the ideal chart oubput by making a note of what our product would assume by using InetSoft's Visualization Reccomender. This is the option that first appears when you create a dashboard. It selects an ideal dashboard output option based on which columns from the dataset are selected. 
 
 The first thing that the wizard Recommender considers is whether or not you're working with a dimension versus a measure. Selecting a dimension automatically results in a chart. So if you're just grabbing a simple text phrased field, it's going to automatically do a chart. However, If you start introducing additional dimensions. And you get to a third dimension it may suggest a crosstab table.


Should I use a table or a crosstab? This depends on whether you want to display row level data or display grouped and summarized data.

Using the reccomender wizard can help you get an idea for how to display your data. What method of displaying data does the product assume? this will vary based on whether dimensions or measures are chosen and how many of each.

Once you get to three or more dimensions the reccomender often starts reccomending a flat detail level table, as that is the common use case for several dimensions with no measures, since without measures there can't be aggregation. Adding a measure from there switches back to a chart as it assumes an aggregated measure.

A simple flat tables does not aggregate metrics; it simply displays individual detail level rows of the columns selected, limited by dashboard filters.

Switching to a crosstab results in the reccomender choosing a pivot style table based on fields selected and the order they were added, 
with horizontal and vertical groupings along row and column headers, with calculated values populated throughout.

crosstab for people who want to display data in summarized way, for people who leave detail level data available in their dashboard design
table for detail level transactional data, certain set of columns in a certain order, details no grouping or summarization, only limited by filters
options for sorting , options for hidden fields for dynamic highlighting, across a row based off of a value in that row, may involve a value that would prefer to not be shown but 
crosstab always doing grouping and summarization
select dimensions for row grouping, selecting dimensions for column groupings, and what aggregates?
question of do i want detailed transactions or summarization
the format of outer grouping > inner grouping > calculated values with default behavior of merged cells, if these defaults are not desirable than go with freehand table
freehand table enables you to control the way a grouping cell does merging
detail level can also be mixed in to a freehand table, giving you the flexibility of both
if data is very pre aggregated at worksheet level then not much aggregation will be happening in the crosstab
but in a crosstab can use show details, multiselecting desired cells and selecting show details displaying rows that make up the selected aggregates
no show details on detail table as there is no further level of data to drill down into
so a crosstab still has drilldown options to see detail level
table is selected column headers and table style, with the option to export rows
crostab default behavior is merging duplicate cells in row and column headers
with crosstabs you can introduce subtotals and grand totals, including subtotals for 
entire grand total column or row, this is not an option in a detail table (but you could make a freehand table with detail and totals, freehand table can add summary row and detail row) 
both tables support hyperlinks to other dashboards, to web pages,
both allow highlighting with data driven formatting
on a detail table you have the option to highlight across the entire row, in a crosstab individual cells are highlighted since they are distince aggregates
on a crosstab you cannot utilize a hidden column to calculate highlights, as you can on a detail table
fundamentally its grouping and sum vs detail
hybrid approach with freehand table
can always convert  either to freehand table to try and meet your needs
database writeback? could be done with detail table
use crosstab when they want data to be grouped and summarized or aggregated in any way
use detail table  to maintain data at detail level that is available at the dashboard level, detail level is maintained as an organized set of rows and columns
show details feature can be used in liew of detail table
some will use a detail table with flyover, using a chart or crosstab displaying aggregates and having the detail table display detail rows of the aggregate moused over "permanent show details filtered by a chart"
can also do a data tip view, to have detail table appear over data point aggregate instead oftaking up space in the dashboard
using either can export easily
detail table "what you see is what you get"
crosstab supports date comparisons, detail table does not
how important is detail data? detail table guarantees that detail data will be available upon export
crosstab will not give axxess to detail data when its exported, just the aggregates it displays
detail table useful for data grabs
detail table for displaying transactional da with data driven highlights or for use with flyover
detail table can even be hidden behind a chart to provide raw data for export only or secondary tab from high level dashboard
if you already have grouping and aggregation built into the data source or the worksheet, a detail table may not be so detailed.  
options for freehand tables make many aggregations done at the data level to be unnecessary
