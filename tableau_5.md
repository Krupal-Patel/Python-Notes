# Insights, Dashboards & Stories

## Insights

  - **Inference:** Customers who purchase Product A are more likely to also purchase Product B.
    - This is a great find! BUT, what does this mean for the company?
  - **Insight:** By bundling Products A and B together, we can increase cross-selling opportunities and overall revenue.
    - Notice that the insight is actionable: The recommendation is to bundle Products A and B together.

  - Website visitors from certain geographic regions spend more time on our pricing page.
     - Insight: Website visitors from certain geographic regions spend more time on our pricing page, so there might be varying price sensitivity across regions, prompting us to customize pricing strategies based on location.
  
  - Customer engagement is higher for emails sent on Tuesdays compared with other weekdays.
    - Insight: Customer engagement is higher for emails sent on Tuesdays compared with other weekdays, so we should schedule our email marketing campaigns for Tuesdays to maximize engagement and response rates.

  - Users who interact with our mobile app in the evening are more likely to make purchases
    - Insight: Users who interact with our mobile app in the evening are more likely to make purchases, so we should tailor our app notifications to target users during their peak engagement times, increasing the chances of conversions.

  - Customer complaints about a specific product have increased after a recent design change, which might be causing usability issues.
    - Insight: Customer complaints about a specific product have increased after a recent design change, which might be causing usability issues. Reverting to the previous design or making further improvements could enhance customer satisfaction.
    
  - Online sales drop during weekends, but in-store foot traffic increases.     
    - Insight: Online sales drop during weekends, but in-store foot traffic increases, so we should focus our online promotions during weekdays and allocate more resources to in-store sales efforts on weekends.

  - Customers who frequently return items tend to have lower satisfaction and make fewer purchases over time.     
    - Insight: Customers who frequently return items tend to have lower satisfaction and make fewer purchases over time. Implementing better product descriptions and images on the website can reduce returns and improve customer satisfaction.
    
  - Social media mentions about our brand have spiked after a recent advertising campaign.
    - Insight: Social media mentions about our brand have spiked after a recent advertising campaign, so we should monitor sentiment and engagement to assess its impact on brand perception.
   
  ## Tooltips and Annotations
  - The interactive box that appears when you hover over a data visualization is called a tooltip, and it is used to help describe information within your visual.
  - Tableau automatically creates tooltips — however, you can edit them to fit your presentation's needs by clicking Tooltip in marks card.


  ### Embed Visualizations in Tooltips
    - Embedding visualizations in tooltips means that when you hover over a portion of the visual, you see additional information in the form of another visualization.
    - To embed a visualization, take these steps:
        1. Open the Tooltip menu.
        2. Select "Insert" → "Sheets."
        3. Then choose the sheet you'd like to embed.

  ### Annotations
    - An annotation is a comment added to any visualization to describe a notable portion of the visual. Annotations are static tooltips that are part of the visualization — the audience is not able to interact with them.
    - There are three types of annotations, which are used to highlight different portions of the visualization.

        1. Mark: Annotates existing marks in the visualization. For example, when you hover over the visualization, you'll see circles appear. Using the Mark option will point to one of the circles.
        2. Point: Annotates exactly where you click. This means that the accuracy of the location you are highlighting is dependent on your ability to get close with your mouse.
        3. Area: Annotates the entire visualization. This type of annotation doesn't point anywhere — it merely creates a text box for you to place on top of the visual.

    - Suppose the sales team is trying to increase profit and would like to know more about the past performance of the Superstore. They are specifically interested in knowing more about the most profitable month.

      - To add an annotation to the most profitable month, take these steps:
      
        1. Right-click on the most profitable month in the visual.
        2. Select the Annotate menu.
        3. Select the annotation type. In this case, Mark.
        4. Add any relevant information that you would like to be included.
        5. Press "OK" when you're finished.
        6. Resize/reposition the annotation to make sure it's not covering any important information. To do this, first single-click on the annotation to put it into edit mode.

## DASHBOARDS
  - A Tableau dashboard is a consolidated display of many worksheets and related information in a single place.
  - Tableau dashboards, also referred to as the **"core of Tableau,"** are used to compare and view a variety of data simultaneously.
  - How did Tableau Dashboards get named the "core of Tableau"? For starters, many of the more traditional data visualization tools do not have this functionality built into their platform. If they do, it's either complicated to replicate or the analyst is expected to know how to code to produce a similar outcome. Tableau allows you to create dashboards with the same drag-and-drop functionality you've been using thus far in this course. This gives you more time to focus on producing insights and preparing content for stakeholders, as opposed to getting stuck trying to figure out the technicalities of the tool.

### Interactive Dashboards
  - To build an interactive dashboard, you would need to add a dashboard action. Start with a static dashboard, then access the dashboard action menu. Go to the top menu bar, click "Dashboard" → "Actions..." → select "Add Action" and examine the six different types of actions.
      - Filter: Uses the data from one view to filter data in another view.
      - Highlight: Calls attention to marks of interest by coloring specific marks and dimming all others.
      - Go to URL: Creates hyperlinks to external resources, such as a web page, file, or another Tableau worksheet.
      - Go to Sheet: Simplifies navigation to other worksheets, dashboards, or stories.
      - Change Parameter: Users can change parameter values by directly interacting with marks on a viz.
      - Change Set Values: Users can change the values in a set by directly interacting with marks on a viz.

    - Dashboards are made up of a series of visualizations that, when combined, are greater than any single visual on its own.
    - The Dashboard tab is made up of three sections: Device Designer, Sheets, and Objects.
    - Device Designer: Allows you to customize the views of a dashboard.
        Sheets: Allows you to combine visuals with ease.
        Objects: Allows you to add unique features to dashboards and integrate them with other applications.
    - As a data visualization expert, it is your job to make visualizations and dashboards as user-friendly as possible. No matter what background your end user has, they should be able to interact with your dashboards to find insights.
    - The three most commonly used dashboard actions are Filter, Highlight, and Go To URL. Other options are Go To Sheet, Change Parameter, and Change Set Values.
    - The Source Sheets portion of the Action interface can be found on all six types of actions. It includes three settings: Hover, Select, and Menu. The interactive setting Select is the recommended setting for dashboard actions because Hover can be challenging to control and Menu takes too many clicks.
    - The Filter action interface enables you to filter an entire dashboard with one click. This interface can be divided into two parts: Target Sheets and Target Filters. Within Target Sheets, there are three options for how to filter data: Leave the filter, Show all values, and Exclude all values.
        
