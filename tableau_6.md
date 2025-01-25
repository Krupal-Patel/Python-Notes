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

## Candle Stick Chart
- A candlestick chart is a dual-axis visualization used to analyze financial markets. Candlestick charts reveal patterns within the data that show how the emotions of traders affect price movements. This means that candlestick charts show the common repeating patterns that occur as a result of human emotion. Financial market analysts can use this information to predict the future, increasing the likelihood of making profitable company decisions. 

- A candlestick chart is made up of two overlaying, vertically staggered bars for each time interval used in the data visualization. In the following candlestick chart, each bar represents a day.

#### Build High Low Chart
-   Since the candlestick chart is a dual-axis chart, and since the high/low bars sit behind the open/close bars, you will build the high/low chart first.

        - Drag the Date dimension onto the Columns shelf and convert the time interval for Date to continuous "Day."
        - Drag the Low measure onto the Rows shelf. (Low is being used as a starting point. In a moment, you'll be incorporating the High measure to give the bars the appropriate heights.)
        - Convert the mark type from Line to Gantt Bar.
        - To size the bars accordingly, you will need to know the difference between the high and low prices for the day. Create a calculated field called High Low Range, which will be [High] - [Low].
        - Drag High Low Range to the Size property in the Marks card.
        - Since the bars are all sitting toward the top, take a moment to examine the highest value and the lowest value and adjust the y-axis accordingly to make the most of the space available. In this case, you can set the y-axis to range from 66 to 75.

#### Add the Open/Close Chart

    - Drag Open to the Rows shelf as a starting point. (Similar to the process earlier, you'll be giving this height in a moment by incorporating the Close value.)
    - Right-click on the Sum(Open) measure in the Rows shelf and select "Dual Axis."
    - Next, you'll want to synchronize the left and right y-axes, so right-click on the right axis, and select "Synchronize Axis."
    - Create a calculated field called Open Close Range with the formula [Close] - [Open], which will be used in a moment to give the bars the appropriate heights.
    - Drag Open Close Range to the Size property in the Marks card.

#### Adjust the Sizes
    - In the SUM(Low) Marks card, change the size to 25%.
    - In the SUM(Open) Marks card, change the size to 50%.

#### Adjust the Colors
    - In the SUM(Low) Marks card, change the Low color to gray.
    - Since the open/close bars are not going to be a single color like the high/low bars, you'll need to create a calculated field to determine the color. Create a calculated field called Color with the following formula:
        IF [Close] >= [Open] THEN "Green"
        ELSE "Red"
        END
    - Drag the Color calculated field to the Color property in the SUM(Open) Marks card.
    - In the SUM(Open) Marks card, adjust the colors, so that "Green" is green and "Red" is red.
