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

### 4. How to connect to data in Power BI? How to use the content pack to connect to google analytics? Mention the steps.

To **Connect to a Data source**, click on **"Get Data"** option in Home Tab. Select the respective Data source. There are multiple sources of data to connect with, i.e, to Database or Cloud or Local File etc., Given below is the screenshot of Getting Data from a web source.
![image](https://user-images.githubusercontent.com/89411580/151568693-aa9aa1b0-65cd-4a89-987a-afa2da6663a2.png)

**_Using Content Pack to Connect to Google Analytics_**

- In the left navigation pane, click Get Data.
![image](https://user-images.githubusercontent.com/89411580/151586830-ee8e90ab-4a00-4d81-807d-fa70abdef74a.png)

- In the Services box, click Get.
![image](https://user-images.githubusercontent.com/89411580/151586877-29c11014-9a05-4239-a194-d758c1a1ff3c.png)

- From the menu of online services, select Google Analytics, and then click Connect.
![image](https://user-images.githubusercontent.com/89411580/151586933-5fc5b3ce-d862-4bc5-a57f-c867e0f1eb47.png)

- Enter the Google Analytics account, property, and view that you want to connect to. Then sign in with your Google Analytics credentials.
![image](https://user-images.githubusercontent.com/89411580/151586952-45f320b4-c0c0-4d44-884e-b122224aadfe.png)

- To permit Power BI to connect to Google Analytics, click Accept.
![image](https://user-images.githubusercontent.com/89411580/151587019-ec1b9683-9fce-4dff-97c0-5abf010bc940.png)

- When the import process completes, you will see a new dashboard, report, and model in the Navigation Pane. Select the dashboard to view your imported data.
![image](https://user-images.githubusercontent.com/89411580/151587065-21d08758-485a-4968-b610-5a80681023ad.png)

Reference : https://powerbi.microsoft.com/en-us/blog/power-bi-google-analytics-power-analytics/
