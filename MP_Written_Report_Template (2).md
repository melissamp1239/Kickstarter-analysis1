# Kickstarting with Excel

## Results

### Purpose
The purpose of the first deliverable was to develop a visualization for Louise that shows campaign outomes in relationship to launch dates and funding goals. Louise got curious about this, as her play **Fever** came close to its fundraising goal in a short amount of time.

The second deliverable's purpose was to create a visualization that portrays the percentage of successful, failed, and canceled plays based on their funding goal amount. 

## Analysis and Challenges
### Deliverable One
I followed the directions for deliverable one at this link: [GWU BOOTCAMP Deliverable 1 Challenge](https://courses.bootcampspot.com/courses/1020/assignments/20753?module_item_id=384168).

First, you need to add a *years* column to the *Kickstarter_Challenge1.xls* worksheet. I calculated the *years* column by following the directions here: [Microsoft Support Page](https://support.microsoft.com/en-us/office/year-function-c64f017a-1354-490d-981f-578e8ec8d3b9?ui=en-us&rs=en-us&ad=us).  You need to place in parenthesis next to *=year*, in the formula, the first cell referencing the 'Date created conversion'.  This **was not challenging** for me, however it could be challenging for someone else. 

Next, you need to create a pivot table. The directions are here for creating a pivot table: [GWU BOOTCAMP Deliverable 1 Challenge](https://courses.bootcampspot.com/courses/1020/pages/1-dot-3-1-pivoting-toward-success). Place the pivot table in a worksheet called *Theater Outcomes by Launch Date*.

Then, you need to apply a filter to the pivot table on the *parent category*, and filter on *theater*.  And add the field *months* to the rows. The directions for creating a pivot table are here: [GWU BOOTCAMP Deliverable 1 Challenge](https://courses.bootcampspot.com/courses/1020/pages/1-dot-3-2-charting-the-parent-category).

By following the directions here, you create a line graph from the pivot table:[GWU BOOTCAMP Deliverable 1 Challenge](https://courses.bootcampspot.com/courses/1020/pages/1-dot-3-2-charting-the-parent-category).

**Here is the line graph created:**
![This is a line graph image](https://github.com/melissamp1239/Kickstarter-analysis1/blob/main/Theater_Outcomes_vs.Launch.png)


### Deliverable Two
I followed the directions at this link to create deliverable2: [GWU BOOTCAMP Deliverable 2 Challenge](https://courses.bootcampspot.com/courses/1020/assignments/20753?module_item_id=384168).

First, go to the **Kickstarter_Challenge_1** worksheet in Excel.  Add a sheet to it and call it **Outcomes Based on Goals**. This sheet will eventually contain a table and also a graph, but first you'll create a data table.  Add to this new table the columns *Goal*, *Number Successful* etc. This is all mentioned in number two under *deliverable two* of the module 1 challenge. You can reference all of these direction at the *GWU BOOTCAMP Deliverable 2 Challenge* link mentioned in the first line of this section. 

Then, reference # 3 under the second deliverable's instructions for module one. *Goal* should be added to the **Outcomes Based on Goals** table. The row names to enter into this table under *Goal* are the following dollar ranges:*less Than 1000*, etc. Reference the *GWU BOOTCAMP Deliverable2 Challenge* url mentioned in the first line in this section for more thorough instructions. 

Next, add in the numbers for the **Outcomes Based on Goals** table.  In the **Outcomes Based on Goals** table, you need to apply a countif formula per row to populate the **Outcomes Based on Goals** table. The formula will filter the **Kickstarter_Challenge_1** worksheet on the column *outcome* to get the range of the *number of successful*, *number of failed* and *number of canceled* plays to populate the **Outcomes Based on Goals** table.  Additionally, you also need to filter the **Kickstarter_Challenge_1** worksheet by adding within the same countif formula, per row, a filter referencing its *subcategory* column to filter on *plays*. The formula that you'll utilize will look like this:`=COUNTIFS(Kickstarter_Challenge_1!$G:$G, "successful", Kickstarter_Challenge_1!$D:$D,"<1,000", Kickstarter_Challenge_1!$Q:$Q, "plays")`.  

Then, I tallied the *Total Project's* by row of the **Outcomes Based on Goals** table column by summing the *number of successful*, *number of failed* and *number of canceled* plays per row. Then, I divided the *percentage successful*, *percentage failed*, *percentage canceled* columns each by the denominator, which is located in the *total projects* column for each row. This is an example of the Excel formula that I used to calculate *percentage successful: `B2/E2`.
 
Finally, I created a line chart by referencing these instructions [GWU Bootcamp Deliverable #2 Challenge] (https://courses.bootcampspot.com/courses/1020/pages/1-dot-3-2-charting-the-parent-category).
 
**Here is the line chart created:**

![This is a line graph image](https://github.com/melissamp1239/Kickstarter-analysis1/blob/main/Outcomes_vs_Goals.png)

### Challenges

For deliverable two, I found it **challenging** to figure out how to use the COUNTIFS formula if there is a range like *1000 to 4999*.  To calculate the *number of successful*, *number of failed*, and *number of canceled* plays for a range like this, I used a slightly different formula: `=COUNTIFS(Kickstarter_Challenge_1!$G:$G, "failed", Kickstarter_Challenge_1!$D:$D,">=1,000", Kickstarter_Challenge_1!$D:$D, "<=4,999", Kickstarter_Challenge_1!$Q:$Q, "plays")`.

## Results

### Analysis of Outcomes Based on Launch Date
May seems to be the month with the most successful plays launched. 

December has the least amount of successful plays launched. 

**Here is the graphic depicting theater outcomes by launch date:**

![This is a line graph image](https://github.com/melissamp1239/Kickstarter-analysis1/blob/main/Theater_Outcomes_vs.Launch.png)

### Analysis of Outcomes Based on Goals
Least successful plays had financial goals of between $45,000 to $49,999.

**Here is the graphic depicting play outcomes based on financial goals:**

![This is a line graph image](https://github.com/melissamp1239/Kickstarter-analysis1/blob/main/Outcomes_vs_Goals.png)

Kickstarter-analysis1/Outcomes_vs_Goals.pn

### Limitations of this data set and recommendations for additional graphs
One limitation of the *kickstarter_challenge* data is that it only contains data for the years 2009 to 2017.

I would recommend developing a graph that would depict television success outcomes based on their financial goals.




