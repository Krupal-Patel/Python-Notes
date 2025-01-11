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

      Numeric Format | Example
      |---|---|
      Number | 10
      Currency	| $10.00
      Percentage	| 10.00%
