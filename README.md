# Dataframe Operations with Apache Spark - Microsoft Fabric

Apache Spark is an open-source, fast, and general-purpose cluster computing system developed for big data processing. Terms like Dataframe, Spark SQL, and PySpark belong to the Apache Spark ecosystem.

## Working with Spark Dataframe and Data Structure

Spark uses a data structure called a Resilient Distributed Dataset (RDD). The most commonly used data structure for working with structured data is the Dataframe, which is part of the Spark SQL library. Dataframes are similar to the data frames in the Pandas library but are optimized for Spark's distributed processing environment.

### 1. Creating a New Notebook

In the workspace, click the **"New"** button and select **"Notebook."** Give the notebook a name and choose **PySpark** as the Spark language.

![image](https://github.com/user-attachments/assets/d27d8e39-b4b2-413e-8793-eadc04a221ea)


### 2. Loading Data into a Dataframe

In this example, a comma-separated text file named `Products.csv` containing product data is used. Press `shift+enter` or click the **"Run"** button next to the cell to execute the code.

![image](https://github.com/user-attachments/assets/0e93bc6d-2db9-4418-a199-3920b4b46118)

### 3. Specifying a Schema Explicitly

If the data file does not contain column names, you can specify an explicit schema.

![image](https://github.com/user-attachments/assets/60107efe-6fce-4e77-ae0b-f7cac893b6e7)

### 4. Filtering and Grouping the Dataframe

The following code selects and displays the ProductID and ListPrice columns.

![image](https://github.com/user-attachments/assets/00154d69-606c-4ae5-8c72-2b9af42fd94f)

### 5. Saving the Dataframe

Using Spark, you can transform raw data and save the results. To save the dataframe in Parquet format, run the following code.
This code saves the bikes_df dataframe in Parquet format to the Files/product_data folder.

![image](https://github.com/user-attachments/assets/5e740607-e7a1-434c-81ce-cc18e5d1a916)

### 6. Partitioning the Output File
To improve performance, you can partition the data using the partitionBy method.
The code below saves the bikes_df dataframe by partitioning it based on category.

![image](https://github.com/user-attachments/assets/2e1723c5-23a0-409c-827a-230a14a9da9d)
