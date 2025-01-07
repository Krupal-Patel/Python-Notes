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
Field's data type can be edited in several ways. In the data grid, you can either right-click the field header, click the triangle in the top-right corner of the field, or click on the data tape icon. All of these options will bring up the same menu to edit Data Type.

### Dirty Data Examples

Type | Description | Example
|---|---|---|
Invalid data | Values that are not possible | Negative values in an Age field
Incorrect data | Values that are possible but not accurate | Outdated information
Inconsistent data | Values that are represented differently | "Monday," "Mon," and "M" in a Day of Week field
Inconsistent data types | Values that are represented using different types of data | The word "eight" and the numeral "8" in an Hours Slept field
Duplicate data | Data that was unintentionally recorded more than once | Multiple votes from the same person
Missing or incomplete data | Values that are either entirely missing or incomplete | "John" found in a Full Name field (missing the last name)
