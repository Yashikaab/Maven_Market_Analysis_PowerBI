# Maven_Market_Analysis_PowerBI

This is my First PowerBI Project.
Here i have worked on a multi-national grocery chain with locations in Canada, Mexico and the United States.

The steps i have followed to build this Interactive Reports are as described below:

Step 1: **Connecting and shaping the data**
      - I have Loaded the data from 6 different CSV files coming from different systems like Calendar, Customers, Products, Regions, Sales, Returns.
      - Then i have transformed the Raw data suitable for Analysis ( Changing Table names, Data types, adding few columns like splitting full names to different columns, and creating few conditional columns which will help me in Analysis.
      - After working on the Raw data and after cleaning all the data i have loaded in to Data Model.

Step 2: **Creating the Data Model**
      - First i have identified which are my Lookup tables and which are Fact/Data tables.
      - Then i have connected the tables using valid Primary and Foriegn Keys.
      - I have made sure that all the relationships are one-to-many cardinality, with primary keys (1) on the lookup side and foreign keys (*) on the data side.
      - Filters are all one-way (no two-way filters).
      - Filter context flows "downstream" from lookup tables to data tables.
      - Data tables are connected via shared lookup tables (not directly to each other).

Step 3: **Adding DAX Measures**
      - I have created few measures to work on Calendar Tables ( like Weekend, Month, Year, Start of Month, End of Month etc)
      - I also created few Calulative measures using CALCULATE, RELATE, % calculations etc, Total Cost, Total Revenue, Total Profit etc)

Step 4: **Building the Report**
      - In Report view, i have added KPI card to show Total Transactions, with Start of Month as the trend axis and Last Month Transactions as the target goal.
      - Have added a Map visual to show Total Transactions by store city and a Treemap visual to break down Total Transactions by store country.
      - I have also added a Matrix visual to show Total Transactions, Total Profit, Profit Margin, and Return Rate by Product_Brand.
      - Added a Column Chart to show Total Revenue every month.
      - Added a Gauge Chart to show Total Revenue against Revenue Target.
