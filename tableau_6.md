# Motion Charts

- The Pages shelf allows you to break a data visualization into a series of pages to view how a specified field affects the data. Think of the Pages shelf as a way of turning your visualization into a flipbook where each page is the same visualization filtered by a different value.
- When a dimension or measure is added to the Pages shelf, multiple visuals (pages) are created for each value within the specified field. Only one visual is visible at a time. You can access these visuals individually by using the Page Control interface, which appears on the right side of your visualization after adding a field to the Pages shelf.

## Dual Axis Chart
- In Tableau, there are two types of dual-axis charts: a single mark dual-axis chart and a combination mark dual-axis chart.
- Combination mark dual-axis charts use two or more mark types within a visualization, such as a bar and a line.
  - Imagine that you're interested in comparing the effects of sales on profit at the Superstore. To show this in a dual-axis chart, you would do the following:
  
    1. Add the Order Date field to the Columns shelf.
    2. Add Profit & Sales to the Rows shelf.
    3. This will create two line graphs. From there, you'll want to take one more step:
  
  Right-click on the measure (on the right) in the Rows shelf and select "Dual Axis" to put the line graphs on top of each other.
  - You can synchronize the axes by right-clicking either of the y-axes and selecting "Synchronize Axis"


## Time-Series Charts
  - **Gantt charts** are used by companies and teams to track the completion of a project. They are often broken up into tasks that are displayed using staggered bars over time.
  - **Candlestick charts** are used to track financial price movements and the emotions of the investors behind those movements. You have probably seen these at some point in your life. Financial market traders use these charts to predict price movements through the emotional patterns found in candlestick charts.
  - Gantt charts and candlestick charts differ wildly in the information they share. However, both types of charts are created with a time variable in the x-axis, and in Tableau they are created using the same type of marks.

### Gantt Chart
  - The dataset consists of a list of tasks, who they are assigned to, the start date, end date, and duration in days for each task.
  - To create a Gantt chart, take the following steps:
      1. Drag the Start Date field onto the Columns shelf.
      2. Change the time interval to Day.
      3. Drag the Task dimension to the Rows shelf.
      4. Set the mark type to Gantt Bar.
      To create the size of the bars, you will need the Duration in Days field. Luckily, in this dataset, that field already exists, but often you will need to create a new calculated field that subtracts the Start Date from the End Date. The duration or difference between the start and end date is what will give the Gantt bars dimension.
      
      5. Drag the Duration in Days field onto the Size property in the Marks card to make the bar as long as the allotted time duration.
      6. Add Assigned To to the Color property in the Marks card to help each team member understand which task they are in charge of.
      All of your tasks are now assigned with the correct duration. However, they are out of order, making the visualization confusing. Gantt charts are meant to show tasks in chronological order so that any team member can look at the chart and see where they fit into the overall goal. You will need to sort your tasks by Start Date. To do this, you would:
      
      7. Right-click on the Task field in the Columns shelf and select "Sort."
      8. Once the sort dialog box appears, choose to sort by "Field."
      9. Specify that you want the sort in ascending order by the field Start Date.
      10. Set the aggregation to "Minimum."
