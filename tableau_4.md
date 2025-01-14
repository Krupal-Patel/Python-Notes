# Table Organization
  - Filtering data to remove data that is unnecessary for your analysis.
  - Sorting data to adjust the order in which the data appears.
  - Enhancing tables by including subtotals and grand totals.

## Worksheet Filters
  Recall that there are two ways to filter your data.

  - **DATA SOURCE FILTERS:** These are used to filter data in the data source before the data gets to the worksheet. When a data source filter is used, it affects the entire Tableau workbook. Filtering the data source is useful when dealing with larger datasets because filtering out unneeded data helps improve the performance of your Tableau creations.
  - **WORKSHEET FILTERS:** These are used to filter data for a specific data visualization in a single worksheet. The data still exists in the data source — you have simply restricted which pieces of data appear in the visualization you're creating. You will use these often throughout your analysis to develop new perspectives of your datasets. While not an official name provided by Tableau, this course will refer to these types of filters as "worksheet filters," as you use them on a worksheet.

### Create Worksheet Filters
  - Creating filters in worksheets is very straightforward. Simply drag the dimension(s) and/or measure(s) you would like to filter to the Filters shelf. When you drag a new field into the Filters shelf, a dialog box will appear. Make your selections and voila — your data is filtered!

### Filter Views
  - Showing the filter is very easy. Simply right-click the pill for which you want to show the filter and select "Show Filter." Hiding the filter is just as easy — right-click the pill again and deselect "Show Filter."
  - To edit the filter view default format, navigate to the filter that has been displayed on the right side of the worksheet, click on the dropdown arrow, and select "Edit Filter."

### Sorting Data
  - Sorting is the process of rearranging the order of your dataset with some purposeful sequence, such as largest-to-smallest or A→Z. Sorting makes your data much more digestible and lends itself to helping analysts quickly find patterns.
    - Ascending Order: Least → Greatest or A→Z
    - Descending Order: Greatest → Least or Z→A
  - When sorting multiple fields, the sorts occur from left to right. This means that if you have two fields being sorted in a view, the leftmost field will get sorted first. 
  - Sort values by clicking the sort icon on the column header
  - You can select column and then sort values from toolbar too.
  - If you've applied too many sorts and would like to get back to the original view, you can use the "Clear Sorts" tool from toolbar.
  
### Grand Totals and Sub Totals
  - Option 1
      - Click the Analytics tab in the sidebar.
      - Drag Totals to your table. As you drag it over, you'll see three options:
        - Subtotals
        - Column Grand Totals
        - Row Grand Totals
      - Drop Totals into the option you would like.
      - Repeat these steps if you would like additional totals.
  - Option 2
      - Click the "Totals" icon in the top toolbar.
      - Select which option(s) you would like.

## Table Customization
    - Edit numeric formatting to ensure clarity of numeric data.
    - Explore the Marks card to learn how to edit the visual display of data.
    - Use the Color property from the Marks card to highlight data and insights from a table.
    - Transform tables into heat maps in order to visually describe numerical data.
    - Use built-in Tableau formatting to customize the design of tables.

### Numeric Formatting
  Numeric formatting is a design concept that gives numbers more meaning by changing how they are displayed. Proper numeric formatting is vital to data visualization. If you don't catch formatting errors, your visuals might lead to incorrect conclusions based on errant number formats. Remember, your primary function as a business or data analyst is to find and deliver insights in the most digestible way for each audience.

The most common numeric formats you will see and edit in Tableau are:

  |Numeric Format | Example |
  |---|---|
  |Number | 10|
  |Currency	| $10.00|
  |Percentage	| 10.00%|

### Marks Card
  - Marks card allows you to control the way data is displayed in Tableau visualizations. For example, in the Marks card, there are several options that can be used to change the color and size of the data. 
  - Marks card interface is made up of three sections, which all have automatic values set by Tableau when you begin dragging fields into your view, though they are all editable later on:

  The Marks card interface is broken up into three sections. The section labeled "Type" points to a dropdown with a text symbol inside, and it reads "Automatic". 
  The second section, labeled "Properties", has buttons labeled Color, Size, Text, Detail, and Tooltip. 
  The third section is labeled "Fields" and has 4 pills: AVG(Discount) with a Color symbol, SUM(Quantity) with a Details symbol, SUM(Sales) with a Details symbol, and AVG(Discount) with a Text symbol.

  - **Mark type** is a dropdown menu that defines the kind of mark displayed. Some common types include Text, Bar, Line, and Map. Note that the use of certain mark types often depends on the types of fields (dimension and/or measures) that are dragged onto the Column and Rows shelves. 
  - Mark properties control how your data will appear inside your visualization. Note that a single field of data can be applied to multiple mark properties.
  - Fields that you have added to the Marks card will be displayed at the bottom of the Marks card. This is helpful for keeping track of which fields are being used to manipulate the various mark properties.
  - In the same way that Tableau automatically assigns data types to each field in a data source, Tableau also automatically decides which mark would best represent a field as it is added to a table.


## Data Visualization

  - Your goal as a data viz analyst is to capitalize on the human brain by creating clear visualizations. The fastest way of getting visual information into a human brain is by optimizing the visual for preattentive processing.
  - Preattentive attributes of visual perception that are used to simplify the process of understanding insights include the following:
    - Color
    - Form
    - Movement
  - Foundational data visualizations used in Tableau include the following:
    - Bar graphs: Used to present categorical data
    - Line graphs: Used to show a continuous set of data points in a connected series
    - Scatter plots: Used to compare the effects of two different numeric fields
  - Tufte's data visualization guidelines include the following:
    - Remove clutter
    - Don't use pie charts
    - Use tables to visually represent small datasets
    - Communicate insights with clarity, precision, and efficiency
    - Avoid distortion
    - Limit your color palette
    - Guide the viewer to the intended conclusions
  - Gestalt theory can be broken down into six design principles:
    - Figure-ground: The thought that when we look at a scene, we separate objects so that some of the focus is on the figure (front) and other parts recede to the back, known as the ground.
    - Similarity: The notion that we place objects with similar characteristics in a group. These characteristics can include color, size, font, shape, texture, and more.
    - Proximity: The belief that we group together objects that are close to each other.
    - Closure: The idea that our minds close objects that are not necessarily together or complete to create a whole.
    - Continuity: The theory that we continue to follow objects that are visually aligned until they are interrupted.
    - Order: The belief that alignment and symmetry are attractive and essential elements of design.
  - The first significant implementation of the design principles in data visualization begins with labeling, which includes the following:
    - Titles: Used to describe the data visualization
    - Axis labels: Used to describe the field information within the rows and columns
    - Captions: Used to succinctly describe the visualization (optional)

## SHOW ME
  - The Show Me menu is a resource Tableau provides to help you build common data visualizations. The menu tells you exactly how many dimensions and measures are required to create frequently used data visualizations. As a reminder, a dimension is a categorical field that is not usually numeric, and a measure is a numeric data type that can be mathematically manipulated. This tool is a quick way to start building visualizations by clearing up any guesswork.


# Comparison Chart
  - **Bar Chart**
      - A bar chart is used to compare categories or groups of data using horizontal or vertical rectangular bars with a height or length proportional to the values each bar represents.
  - **Treemaps**
      - A treemap visualization is used to compare categorical data using both size and color to display the numerical value. Bar charts use length to compare values, whereas treemaps use length and width (area) to compare values.

# Predictive Chart
  - Predictive charts are a category of data visualizations used to reveal trends in the data, allowing analysts to hypothesize whether a similar pattern may be followed in the future.

  - **Line Graph**
      - A line graph is used to show the change of a measure — or measures over time — using a continuous line. Because line graphs are used to track a measure over time, they are also known as time series plots.

  - **Scatter Plot**
      - A scatter plot is a data visualization used to show the relationship between two variables, or how they correlate. Correlation is the relationship between variables. It is important to remember that just because one variable seems to affect another, that doesn't mean one caused the other.
      - When working with scatter plots, you'll often hear the terms independent variable and dependent variable.
        Independent Variable: In data analytics, the independent variable is the variable that you believe may influence or explain changes in the dependent variable.
        Dependent Variable: The dependent variable in data analytics is the variable you're trying to predict, explain, or understand based on changes in the independent variable(s).

      - **When presenting data, only use a trend line if your R-squared is high:** Trend lines can mislead the audience into thinking there is a trend when there is not. Generally, you don't want to use a trend line in a scatter plot presentation unless there is an R-squared value of 0.6-0.8 or higher.
      - **Use trend lines if there is added value:** Trend lines condense all the points into something often more meaningful for audiences, and you should always use these to check for correlations — however, only keep them in your viz if they add value.
   
## Trend Lines
  - There are five types of trend lines you can create in Tableau.
      1. Linear
      2. Logarithmic
      3. Exponential
      4. Polynomial
      5. Power
  - How to Create a Trend Line
      You can add a trend line by navigating to the Analytics tab and dragging "Trend Line" to the data visualizer over the "Linear" option that appears

      - **Watch out for outliers:** Outliers can skew your trend lines into giving non-realistic results. Watch out for outliers and the effect they have on the visualization.
      - **Avoid overusing trend lines:** Trend lines are not intended to be added to every visualization. Use them sparingly to add value to the story you are attempting to convey.
      - **Avoid using a trend line for small datasets:** The value of a trend line is the ability to aggregate large amounts of data into a predictable line. Trend lines are not as useful for tiny datasets.


  - The tooltip for the trend line contains statistically calculated numbers that help you diagnose if there actually is a correlation. Take a minute to examine the trend lines tooltip before moving on to learn about what each piece means.

  - There are three lines of text in the tooltip:

      1. The first is the equation of the trend line.
      2. The second is the R-squared value.
          - R-Squared is used to show the amount of variance that the trend line explains and is displayed as a number from 0 to 1.
          - Variance is the measure that calculates how far each number in the dataset is from the mean. Variance is useful to see how spread a dataset is.
      3. The third is the p-value. The P-value is used to show the probability of obtaining the desired result and is also displayed as a number between 0 and 1. 


## Statistical Charts
  - **Histograms**
    - A histogram is a statistical bar chart that is used to show the distribution of numerical data. Histograms are univariate visualizations, meaning they only plot one numerical field. This allows you to see the frequency of occurrences within the field, which helps you understand the probability of data within that numerical field.
    - Creating a Histogram creats a new dimension.
   
    - Manual Creation of Histogram
        1. Create a new field by right-clicking on the Quantity measure and clicking "Create" → "Bins..."
        2. Set the size of the bins to 2.
        3. Exit the "Edit Bins" menu by clicking the "X" in the top-right corner.
        4. Since these bins should sit along the x-axis, drag the newly created Quantity (bin) field to the Columns shelf.
        5. Since the quantity shows up along the y-axis, add the Quantity field to the Rows shelf.
        6. By default, the Quantity is aggregated using the SUM function. You will want a count of the quantities, so right-click the SUM(Quantity) pill in the Rows shelf and select "Measure" → "Count."
        7. Almost there! To remove the gaps between the vertical bars, convert the Quantity (bin) dimension from discrete to continuous by right-clicking the Quantity (bin) pill in the Columns shelf and selecting "Continuous."
   
  - **Box Plots**
    - Box plots, also known as box-and-whisker plots, are visualizations that show a statistical summary of selected data. The statistical summary is made up of five pieces: the data's minimum, maximum, median, first quartile, and third quartile values.
   



## Recape of Charts
**Comparison Charts**
  - **Comparison charts:** Graphical representations that allow for the visual comparison of data points, values, or categories.
  - **Bar chart:** A graph that presents data with either horizontal or vertical rectangular bars.
  - **Treemap:** A type of visualization that is used to display the value of data using both size and color.
**Predictive Charts**
  - **Predictive charts:** A category of data visualizations used to reveal trends in the data allowing the analyst to hypothesize whether a similar pattern may be followed in the future.
  - **Line graphs:** Data visualizations used to show the differences between variables by using a continuous line.
  - **Time series plots:** Line graphs that are used to track a measure over time.
  - **Scatter plot:** A data visualization used to show the relationship between two variables.
    - **Correlation:** The relationship between variables. Correlation does not imply causation.
      - **Independent Variable:** The variable that you believe may influence or explain changes in the dependent variable.
      - **Dependent Variable:** The variable you're trying to predict, explain, or understand based on changes in the independent variable(s).
    - **Trend lines:** Lines created using statistical functions to help you confirm trends exist. 
      - **Linear trend line:** A straight line that best fits a set of data points in a way that represents a linear trend in the data. 
      - **R-squared:** Used to show the amount of variance that the trend line explains — displayed as a number from 0 to 1.
      - **Variance:** The measure that calculates how far each number in the dataset is from the mean.
      - **P-value:** Used to show the probability of obtaining the desired result — shown as a number between 0 and 1.

**Statistical Charts**
  - **Statistical charts:**  Visual representations of data used to display and communicate various types of information, trends, and relationships. 
  - **Histogram:** A statistical bar chart that is used to show the distribution of numerical data.
    - **Bins:** A consistent value range that data is sorted into to form groups.
    - **Skewness:** The measure of symmetry or asymmetry of a distribution. Skewness describes if the curve is a symmetrical bell or if the data is bunched more to one side.

  - **Box plots:** Also known as box-and-whisker plots, they are visualizations that show a statistical five-number summary of the selected data. The statistical summary includes the minimum, maximum, median, first quartile, and third quartile. 
    - **Minimum:** The smallest value within your dataset.
    - **Maximum:** The largest value in your dataset.
    - **Median:** The middle value within your dataset. The median is also known as the second quartile (Q2). It separates the first 50% of your data from the second 50%.
    - **Quartiles:** Numbers that divide the values in your dataset, when put into a list from least to greatest, into four equal quarters.
    - **First quartile (Q1):** The value that separates the first 25% of your dataset from the next 25%. The first quartile can be found by finding the middle value between your minimum and median values.
    - **Third quartile (Q3):** The value that separates the last 25% of your dataset, from the second to last quarter. The third quartile can be found by finding the middle value between the median and the maximum values.
    - **Interquartile range (IQR):** The middle 50% of your data set. The IQR includes any values that fall between Q1 and Q3. 
    - **Whiskers:** Lines that go from each quartile to the minimum or maximum.
