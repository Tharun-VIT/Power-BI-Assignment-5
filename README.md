# Power-BI-Assignment-5

### 1. Explain DAX

DAX is the formula language associated with the Data Model of Microsoft Excel Power Pivot and with Microsoft Power BI. It is used to calculate values, create calculated columns, filter query and many other tasks through Expressions or formulas. DAX formulas enable you to perform data modeling, data analysis, and use the results for reporting and decision making. DAX is a very important skill for Analyst to work with Power BI. 

A sample DAX Expression.

Total Sales in East = ADDCOLUMNS ( 
   Products,"East_Sales", SUMX (RELATEDTABLE(East_Sales), 
      IF([Product] = East_Sales[Product], East_Sales[Sales Amount],0) 
   ) 
)

### 2. Explain datasets, reports, and dashboards and how they relate to each other?

**Dataset** is a collection of raw data from one or multiple data sources which the Analyst uses to clean, Analyze, Visualize, get insight and create reports and Dashboards. It is a raw form of data which contains attributes which when processed might help in understanding the task and draw conclusions. There are multiple types of Dataset such as Table, Links, Trees, Network, Geo-spatial etc.,

**Reports** is a page or series of pages which contains multiple tiles depicting some values or graphs in form of visualizations which are colourful and interactive. It can convey the performance of Business. If streaming data is supplied, dynamic changes are reflected in Visualizations in reports. Multiple reports are created for different areas of Business and the reports are watched closely by stakeholders.

**Dashboards** are also a form of reports. The unique thing is it a summarized form of report. It contains the same elements as reports have. But the important key information alone is added to dashboard from multiple reports. For example, we may create multiple indivudual reports on Facebook, Instragram, LinkedIn data how people interact with our Business page. A Dashboard for same case might try to depict "How to Digital media covers audience and accounts for Business?" which may contain some tile or visuals from the reports created individually on Facebook, Instagram or LinkedIn data.

**Relation** between these three is in hierarchical Manner. From processed Dataset we create multiple reports and from multiple reports, we create unique Dashboards. Ofcourse both reports and Dashboards are accessible to stakeholders. Dataset is processed is Power BI desktop and Reports and Dashboards are accessed by stakeholders through Power BI service/Mobile.

### 3. How reports can be created in power BI, explain two ways with Navigation of each.

There are 3 primary sections in home page which is used to create contents in Reports
- **Canvas** - The center blank white is the canvas where visuals will appear
- **Fields Pane** - Contains queries and columns of the dataset 
- **Visualization Pane** - To edit and format visualizations

Reports can be created in two ways
- Select the fields first then visualizations after
- Select the type of visual first then the fields after

**METHOD 1**

 **step 1** - Select 2 columns from Field Pane to visualize the data in 2D chart.
 **step 2** - When clicking them, a suitable visual will appear in the canvas area.
 **step 3** - Drag them and position them properly. Use formatting options in Visualization Pane for Customization.
 **step 4** - If you want to change the type of graph, select the chart tile in canvas and click the required type of graph in Visualization Pane.

**METHOD 2**

**step 1** - Select the chart type. An empty tile will appear in Canvas.
**step 2** - Click and drag the Columns to Fields and Values field in Visualization pane.
**step 3** - If we want to categorize the 2D plot with category as 3rd Dimension, the drop the column in Legend Field
**step 4** - Use formatting options in Visualization Pane for Customization.

Click File-->Save and type the name of the report. Now once we save our Report in Power BI desktop, it is time to publish it in Power BI service. Click on "Publish" option in Home Tab. Type the Name of report and select the workspace on which you want to publish the report. Now we have created a report for the stakeholders in workspace.
