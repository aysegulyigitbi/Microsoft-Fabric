# End-to-End Data Analysis with Apache Spark in Microsoft Fabric

In this article, we will explain step by step how to perform data analysis in Microsoft Fabric using Apache Spark. Apache Spark is an open-source engine used for distributed data processing, providing broad language support for analyzing large datasets. These steps include data cleaning, manipulation, statistical analysis, and data visualization.

## 1. Creating a Workspace
First, you need to create a workspace in Microsoft Fabric:
1. Go to the Microsoft Fabric homepage.
2. From the left menu, select "Workspaces."
3. Create a new workspace. In the advanced section, choose a licensing mode that includes Fabric capacity (Trial, Premium, or Fabric).

## 2. Creating a Lakehouse and Uploading Files
After creating a workspace, create a Lakehouse for the data files you will analyze:
1. On the Synapse Data Engineering homepage, create a new Lakehouse.
2. Download and extract the data files from this [link](#).
3. Upload the extracted `orders` folder to the Lakehouse.

![image](https://github.com/user-attachments/assets/db77e4db-7ef1-4ff3-a5f8-7791ba50b4c5)


## 3. Creating a Notebook
Create a notebook for data work using Apache Spark:
1. While viewing the Lakehouse content, select **New notebook** from the **Open notebook** menu.

![image](https://github.com/user-attachments/assets/fa41648a-dc13-4caf-888b-d9f720f0b44c)


## 4. Loading Data into a DataFrame
Follow these steps to load data into a Spark DataFrame:
1. Select the `2019.csv` file from the Lakehouse and choose **Load data > Spark**.

![image](https://github.com/user-attachments/assets/acdf313a-1213-4ca4-a2b2-a2a3d7aeb0e2)


2. Run the code that is automatically generated in the notebook cell.

![image](https://github.com/user-attachments/assets/529f58e4-e76e-46cd-88d9-160f010989d2)


3. Use the following code to correctly define column names and data types:

![image](https://github.com/user-attachments/assets/0a32e107-eeec-480f-a93d-9148cde42fc0)


4. Change the file path to load data from all years:

![image](https://github.com/user-attachments/assets/51baa2a0-94ff-4f8b-b764-685163a0f3c3)


## 5. Exploring Data in the DataFrame
To explore the data in the DataFrame, perform the following operations:
1. Add a new cell and write the following code:

![image](https://github.com/user-attachments/assets/2477ddc7-4cd4-4e8a-9a57-b9e3805735c1)


2. Filter by products:

![image](https://github.com/user-attachments/assets/74d17622-4144-416d-a7f8-a3dc770dce3b)


3. Perform data grouping and aggregation:

![image](https://github.com/user-attachments/assets/6c813e2a-0517-4eea-9c6d-0d3b52cac9be)


## 6. Transforming and Saving Data
Follow these steps to transform and save the data:
1. Add new columns and rearrange the data:

![image](https://github.com/user-attachments/assets/a9b9ffc7-ddad-46fc-b1e3-ce385890631c)


2. Save the data in Parquet format:

![image](https://github.com/user-attachments/assets/9a3eaf0c-504b-4ea5-bc2a-76b5702bb4b4)


3. Save the data in partitions:

![image](https://github.com/user-attachments/assets/4358c7f7-91f6-443c-96f9-a762b91c1b03)


## 7. Working with SQL
You can perform SQL queries using the Spark metastore:
1. Save the DataFrame as a table:

![image](https://github.com/user-attachments/assets/adfe92d4-f0f4-4b54-88e3-7b4810a9744a)


2. Run SQL queries:

![image](https://github.com/user-attachments/assets/c800ce5e-6b21-442f-b166-f58018b274fa)


## 8. Data Visualization
You can use the `matplotlib` library to visualize the data:
1. Display annual revenue in a bar chart:

![image](https://github.com/user-attachments/assets/0de519b1-f673-400f-9ce1-993ae6973872)


