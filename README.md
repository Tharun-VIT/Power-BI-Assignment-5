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
