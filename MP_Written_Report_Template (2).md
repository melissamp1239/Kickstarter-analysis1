# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of the first deliverable was to develop a visualization for Louise that shows campaign outomes in relationship to launch dates and funding goals. Louise got curious about this, as her play **Fever** came close to its fundraising goal in a short amount of time.

The second deliverable's purpose was to create a visualization that portrays the percentage of successful, failed, and canceled plays based on their funding goal amount. 

## Analysis and Challenges
###First Deliverable Completion Steps
I followed the directions for deliverable one at this link: [GWU BOOTCAMP Deliverable 1 Challenge](https://courses.bootcampspot.com/courses/1020/assignments/20753?module_item_id=384168).
[] First, you need to add a *years* column to *Kickstarter_Challenge.xls* worksheet. I calculated the years column by following the directions here: [Microsoft Support Page](https://support.microsoft.com/en-us/office/year-function-c64f017a-1354-490d-981f-578e8ec8d3b9?ui=en-us&rs=en-us&ad=us).  You need to place in parenthesis next to the equals sign year, the first cell referencing the 'Date created conversion'.  This **was not challenging** for me, however it could be challenging to someone else. 
[] Next, you need to create a pivot table. The directions are here: [GWU BOOTCAMP Deliverable 1 Challenge](https://courses.bootcampspot.com/courses/1020/pages/1-dot-3-1-pivoting-toward-success). Place the pivot table in a worksheet called *Theater Outcomes by Launch Date*.
[] Then, you need to apply a filter to the pivot table on *parent category*, and filter on *theater*.  And add the field *months* to the rows.The directions for creating a pivot table are here [GWU BOOTCAMP Deliverable 1 Challenge](https://courses.bootcampspot.com/courses/1020/pages/1-dot-3-2-charting-the-parent-category).
This pivot table in the end is created:

[]By following the directions here, you create a line graph from the pivot table:[GWU BOOTCAMP Deliverable 1 Challenge](https://courses.bootcampspot.com/courses/1020/pages/1-dot-3-2-charting-the-parent-category).
[]This line graph in the end is created:

###Second Deliverable Completion Steps
I followed the directions for deliverable two at this link: [GWU BOOTCAMP Deliverable 1 Challenge](https://courses.bootcampspot.com/courses/1020/assignments/20753?module_item_id=384168).
[] First, go to the **Kickstarter_Challenge_1** worksheet.  Add a sheet to it and call it *Outcomes Based on Goals*. This sheet will be created into a table. Add to this new sheet the columns *Goal*, *Number Successful* etc. mentioned in number two under *deliverable two* of module 1 challenge. 
[]Then reference # 3 under the second deliverable's instructions for module one. *Goal* should be added to the *Outcomes Based on Goals* workseet. The row names to enter into this table under *Goal* are the following dollar ranges: *less Than 1000*, etc.
[]Next, to add in the numbers for the **Outcomes Based on Goals** worksheet,
 you need to apply a countif formula per row that will filter the **Kickstarter_Challenge_1** worksheet on the column *outcome* to get the range of the *number of successful*, *number of failed* and *number of canceled* plays. You also need to filter the **Kickstarter_Challenge_1** worksheet by adding within the same countif formula per row, a filter on the *subcategory* column to fileter on *plays*. The formula that you'll utilize will look like this:`=COUNTIFS(Kickstarter_Challenge_1!$G:$G, "successful", Kickstarter_Challenge_1!$D:$D,"<1,000", Kickstarter_Challenge_1!$Q:$Q, "plays")`.  

 []Then, I tallied the *Total Project* column by summing the *number of successful*, *number of failed* and *number of canceled* plays per row. Then, I divied the *percentage successful*, *percentage failed*, *percentage canceled* each by the denominator *total projects* for each row. This is an example of the Excel formula I used to calculate *percentage successful* `B2/E2`.
 []Finally, I created a line chart by referencing [GWU Bootcamp Deliverable #2 Challenge] (https://courses.bootcampspot.com/courses/1020/pages/1-dot-3-2-charting-the-parent-category).

 ###Challenges and Difficulties Encountered

[]For deliverable two, I found it **challenging** to figure out how to use the COUNTIFS formula if there is a range like *1000 to 4999*.  To calculate the *number of successful*, *number of failed*, and *number of canceled* plays for a range like this, I used a slightly different formula: `=COUNTIFS(Kickstarter_Challenge_1!$G:$G, "failed", Kickstarter_Challenge_1!$D:$D,">=1,000", Kickstarter_Challenge_1!$D:$D, "<=4,999", Kickstarter_Challenge_1!$Q:$Q, "plays")`.

##Results

### Analysis of Outcomes Based on Launch Date
[]May seems to be the month with the most successful plays launched.  December has the least amount of successful plays launched. 
**Here is the graphic depicting theater outcomes by launch date:**

### Analysis of Outcomes Based on Goals

Least successful plays had financial goals of between $45,000 to $49,999.
**Here is the graphic depicting play outcomes based on financial goals:**

###Limitations of this data set and recommendations for additional graphs
[]One limitation of the *kickstarter_challenge* data is that it only contains data for the years 2009 to 2017.
[]I would recommend developing a graph that would depict television success outcomes based on their financial goals.




