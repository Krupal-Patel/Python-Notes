## Preprocessing Data
  1. Change field data types 
  2. Rename fields
  3. Pivot fields
  4. Hide fields
  5. Use the Data Interpreter

## Tableau Data types
  - Whenever you connect a data source to Tableau, Tableau will automatically give each field within the table(s) a data type.
Data Type

|Data Type Icon|Description/Example|String (text)|
|---|---|---|
String | Abc | Can include letters, symbols, and numbers
Date | Date icon - looks like a calendar | E.g., 2/11/2005
Date & Time | Date & Time icon - looks like a calendar with a clock in the corner | E.g., 2/11/2005 11:45:00 AM
Numerical | # | Numbers only, with or without a decimal
Boolean | T\|F | Values that are either true or false
Geographic | Geographic icon - looks like a globe | Countries, zip codes, addresses, etc.

### How to edit Data Type
  - Field's data type can be edited in several ways. In the data grid, you can either right-click the field header, click the triangle in the top-right corner of the field, or click on the data tape icon. All of these options will bring up the same menu to edit Data Type.


### Dirty Data Examples

Type | Description | Example
|---|---|---|
Invalid data | Values that are not possible | Negative values in an Age field
Incorrect data | Values that are possible but not accurate | Outdated information
Inconsistent data | Values that are represented differently | "Monday," "Mon," and "M" in a Day of Week field
Inconsistent data types | Values that are represented using different types of data | The word "eight" and the numeral "8" in an Hours Slept field
Duplicate data | Data that was unintentionally recorded more than once | Multiple votes from the same person
Missing or incomplete data | Values that are either entirely missing or incomplete | "John" found in a Full Name field (missing the last name)

### Preprocess Data Source
  - Preprocess data by renaming, removing, and pivoting fields, and using Tableau's built-in Data Interpreter.

#### How to Rename a Field
  - Renaming a field in Tableau can be done a couple of different ways. You can either double-click the field name or right-click on the field and select "Rename." This can be done either in the data grid or the metadata grid.

#### How to Hide a Field
  - Hiding a field can be done by right-clicking the field and selecting "Hide."


#### How to Pivot Fields
  - Pivoting fields can be achieved by selecting all of the fields you would like to pivot, right-clicking, and selecting "Pivot."

### Data Interpreter
  - The Data Interpreter is a tool unique to Tableau that can detect, remove, and restructure the data in your data source.
  - You can use the Data Interpreter with spreadsheet files like Excel and Google Sheets and text files like CSVs and PDFs. The results generated from using the tool will generate an Excel file, regardless of what type of file you selected as the data source.
  - Note that the Data Interpreter does not change the underlying data. It instead focuses on adjusting/removing titles, notes, footers, and empty cells to better fit the format of the data grid in Tableau. You can proceed to continue cleaning your data in the data grid afterward.
  
  - The Data Interpreter might not be an option in the following circumstances:
      - The data is clean (format-wise)!
      - The data is already in a format that Tableau can interpret.
      - The file type of the data source is not supported.
      - The dataset is too big. The Data Interpreter option is not available when the dataset contains:
        - More than 2,000 columns or
        - More than 3,000 rows and more than 150 columns.


### Key Takeaways
  - The data type reflects the kind of information within each field of the table and also distinguishes how that field can be manipulated.
Tableau was not built for cleaning data. It is intended to be used alongside a database that handles most of the data manipulation.
  - The main data manipulation tactics that can be used in Tableau include renaming, hiding, and pivoting fields.
  - Renaming fields is essential for increasing readability. Some datasets have field names that are not as descriptive or understandable as they could be. Unclear field names leave too much room for interpretation of what that field contains.
  - Hiding fields is advantageous because it can streamline your analysis by getting irrelevant fields out of your way to better focus on the relevant content.
 - Pivoting fields in Tableau involves transforming columns into rows, which allows for a more efficient and streamlined view of data with fewer columns.
  - Care should be taken when updating a field's data type. Before changing the data type, consider why it was incorrectly classified. If you change the data type of a field, then any data that doesn't match the data type will be replaced with "null."


### Advance Data Processing
    - Calculated fields
    - Splitting fields
    - Data source filters

#### Calculated Fields
  - Right-click the field that you would like to work with. In this case, Customer Name. Then, from the dropdown, click “Create” → “Calculated Field…”
  - [Tableau Function List.](https://help.tableau.com/current/pro/desktop/en-us/functions.htm)


#### Datasource Filters
In Tableau, there are two main ways to filter data:

  - **Data Source Filters** : These are used to filter data in the data source before the data gets to the worksheet. When a data source filter is used, it affects the entire Tableau workbook. Filtering the data source is useful when dealing with larger datasets because filtering out unneeded data helps improve the performance of your Tableau creations.
  - **Worksheet Filters** : These are used to filter data for a specific data visualization. The data still exists in the data source — you have simply restricted which pieces of data appear in the visualization you're creating. You will use these often throughout your analysis to develop new perspectives on your datasets. While not an official name provided by Tableau, this course will refer to these types of filters as "worksheet filters," as you use them on a worksheet.


#### Advantages of Data Source Filters
  - Data source filters are applied across an entire workbook and are created in the data source tab. This means that any data that is filtered out will not be available to use for any visualizations in the workbook.

Data source filters provide two main advantages.
  - **Performance/optimization**: As mentioned above, data source filters essentially ask Tableau to keep only the rows that meet specific criteria. This means that there is less data Tableau has to manage and manipulate, which means the dataset will use less of Tableau's processing power. You will often see quickened performance when using data source filters, especially when working with very large datasets.
  - **Security**: Another key benefit of using data source filters is improved security when working with datasets that contain sensitive data. While a worksheet filter can block sensitive data from data visualizations, there are certain access permissions that, if set, can allow users to view the full dataset. This is an issue because some data is not meant to be shared (e.g., health records). If a dataset contains sensitive data that users should not see, you can use a data source filter so the data never makes it to Tableau in the first place.

##### How to Create a Data Source Filter
Creating a data source filter in Tableau is done in the data source page. In the top-right corner, you will see a section called "Filters" that contains an "Add" button. Click this button to create a new data source filter or to edit existing filters. If no data source filters have been created, an empty Edit Data Source Filters dialog box will appear.
