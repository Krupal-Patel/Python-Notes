# Tableau Worksheets

  - When working in Tableau, you start your work within a Tableau workbook. The workbook is a file structure made up of sheets, similar to Excel or Google Sheets. Each sheet within the Tableau workbook can be one of three types: a worksheet, a dashboard, or a story.

## Dimensions and Measures
**Dimensions** are data fields that contain qualitative values. **Qualitative** data is conceptual and descriptive. Qualitative data can be expressed using text, symbols, and characteristics (text, geographic data, names, etc.).

**Measures** are data fields that contain quantitative or numerical values. **Quantitative** data can be measured, counted, and expressed using numbers (sales, number of records, profit, etc.).

Tableau programmatically categorizes fields into these groups to tell you if a field can be numerically manipulated (a **measure**) or not (a **dimension**). 

In Tableau, when a **measure** is added to the visualization, the field is automatically aggregated. Aggregation means that the field is summarized using mathematical equations such as sum total, median, or average. 

Because a dimension cannot be measured, it is used to create groups.

## Discrete and Continuous

  **Discrete**: Individually separate and distinct. When a discrete field is plotted, there are gaps between each point of data — signifying that each point of data is separate from the whole.
  - An example of discrete would be counties. You’re always in a specific county, and there are county lines — the moment you cross over the county line, the name of the county you’re in changes. There is no gradual transition — the name of the county “jumps” from one to the next.
  - In Tableau, discrete fields are shown in the worksheet in blue.
  - A blue "pill" that says "Discrete."

  **Continuous**: Forming an unbroken whole; without interruption. When a continuous field is plotted on a line graph, the line is unbroken.

  - An example of continuous would be your weight: There are an infinite number of values your weight could be. In other words, there is always another weight between any two weights (e.g., between 152.46 lbs and 152.47 lbs is 152.465 lbs). Continuous data is always a number.
  - In Tableau, continuous fields are shown in the worksheet as green.
