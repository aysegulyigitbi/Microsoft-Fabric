# End-to-End Business Intelligence Application with Microsoft Fabric

Traditionally, large-scale data analytics solutions have been built around data warehouses. Data is stored in relational tables and queried using SQL. However, the emergence of big data, low-cost storage, and cloud-based distributed computing technologies has led to a new approach called Data Lakehouse. The Data Lakehouse stores data as files without a fixed schema. In this approach, data is stored as files in a data lakehouse.

## Creating a Lakehouse in Microsoft Fabric

In Microsoft Fabric, the Lakehouse provides highly scalable file storage on OneLake, built on Azure Data Lake Store Gen2. This storage includes a metastore for relational objects such as tables and views and uses the Delta Lake-based open-source table format. This allows you to define the schema of tables in the Lakehouse and query them using SQL.

![image](https://github.com/user-attachments/assets/129f1d70-bb6a-4c0b-8d19-f073aa523181)


### 1) Creating a Workspace

Before working with data in Fabric, create a workspace where the Fabric trial version is enabled. Select Workspaces from the left menu bar and create a new workspace by selecting a licensing mode that includes Fabric capacity.

### 2) Creating a Lakehouse

After creating the workspace, create a data lakehouse to store your data files.

**Note:**

- **Tables:** Includes tables that can be queried using SQL. Tables in Microsoft Fabric Lakehouse are based on the open-source Delta Lake file format, commonly used in Apache Spark.
- **Files:** Includes data files not associated with delta tables managed in the Lakehouse’s OneLake storage. You can also create shortcuts to reference externally stored data in this folder.

![image](https://github.com/user-attachments/assets/621243ea-979e-40c9-b99d-839b1c106f4f)


### 3) Uploading Files

Fabric offers various methods for loading data into a Lakehouse. These include pipelines that copy data from external sources and visual tools based on Power Query. However, one of the simplest ways to load a small amount of data is to upload a file or folder from your local computer. Create a new subfolder in the Files folder.

![image](https://github.com/user-attachments/assets/c68de14b-a52a-482e-9dec-fd57fb2afb14)


**Upload the CSV file to the Data folder.**

![image](https://github.com/user-attachments/assets/9372abd1-c1ca-4ec9-9782-2a88808fcf49)

After the file is uploaded, select the Files/data folder and verify that the `sales.csv` file is uploaded.

### 4) Loading File Data into a Table

The sales data you uploaded is in a file and can be directly executed using Apache Spark code. However, loading data from a file into a table is more suitable for querying using SQL.

**To view the CSV file, select the Files/Data folder and choose "Load to Tables" from the CSV file menu.**

![image](https://github.com/user-attachments/assets/8a2dd765-b977-417d-8f7d-432e72c06bb4)


Confirm the table loading process.

### 5) Querying Tables with SQL

When you create a Lakehouse and define tables within it, a SQL endpoint is automatically created where the tables can be queried using SQL `SELECT` statements.

**Switch from the Lakehouse page to the SQL analytics endpoint at the top right.**

![image](https://github.com/user-attachments/assets/50bec27a-2750-4314-a3b3-ab90310c152c)


Use the "New SQL query" button to open a new query editor and enter an SQL query. Use the "Run" button to execute the query and see the results.

![image](https://github.com/user-attachments/assets/4c2f5c12-bf8a-4451-874d-a67302ea36ba)


### 6) Creating a Visual Query

While many people are familiar with SQL, data analysts with Power BI experience can use their Power Query skills to create visual queries.

![image](https://github.com/user-attachments/assets/565ea916-cc9b-4f2c-9909-bf2f85e2f2a0)


**Select the "New visual query" button in the toolbar.**

Drag your table into the new visual query editor pane.

![image](https://github.com/user-attachments/assets/d330ad77-bc9d-4978-9551-1edc0d4df098)


Everything you can do in Power Query can be directly reflected in the corresponding interface.

- **Select Column:**

![image](https://github.com/user-attachments/assets/38e489fe-fd96-47dd-b834-46e4c1f671f0)


- **Group:** In the Transform menu, select the "Group by" option to configure the desired grouping.

![image](https://github.com/user-attachments/assets/2f38ae2d-0c21-4be1-b39c-469076946832)


### 7) Creating a Report

Tables in the Lakehouse are automatically added to the default semantic model for reporting with Power BI.

![image](https://github.com/user-attachments/assets/aaf0ccdc-bd24-4a22-9110-8e38bb98bd71)


**Select the Model tab at the bottom of the SQL Endpoint page. The data model schema related to the semantic model is displayed.**

In the ribbon, select the "Reporting" tab and then choose "New report." In the Power BI interface, you can add desired visuals and perform analyses.

![image](https://github.com/user-attachments/assets/503fc421-0c1b-4dec-a30f-61c2b82d294e)

