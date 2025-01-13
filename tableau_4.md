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
