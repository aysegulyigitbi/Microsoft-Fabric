# Using the Copy Data Activity in Microsoft Fabric via Data Factory

The **Copy Data** activity is one of the most frequently used pipeline activities in Data Factory. Many pipelines consist of a single Copy Data activity designed to ingest data from an external source into a lakehouse file or table.

By combining the Copy Data activity with other activities, you can create a repeatable data ingestion process. For example, you might use:
- The **Delete Data** activity to remove existing data,
- The **Copy Data** activity to replace deleted data with data from an external source, and
- The **Notebook** activity running Spark code to transform the data in the file and load it into a table.

## Copy Data Tool

The **Copy Data** tool in Microsoft Fabric simplifies configuring the source and destination when adding the Copy Data activity to a pipeline. It supports a wide variety of source connections, enabling seamless data ingestion from the most commonly used data sources.

![image](https://github.com/user-attachments/assets/36644153-492b-403e-beff-0da303f17b57)


## Use Cases for the Copy Data Activity

The **Copy Data** activity is ideal when you need to copy data between a supported source and destination without applying transformations or when you want to import raw data for later processing in pipeline activities.

If you need to apply transformations during data ingestion or combine data from multiple sources, consider using the **Data Flow** activity to run a **dataflow (Gen2)**. With the Power Query user interface, you can define a dataflow (Gen2) with multiple transformation steps and add it to your pipeline.

## Steps to Use the Copy Data Activity

1. **Navigate to the Data Pipeline**  
   In the **Data Factory** section, select the **Data Pipeline** option.

![image](https://github.com/user-attachments/assets/d7d83095-50b7-43ec-81de-accdc255720a)


2. **Name Your Pipeline**  
   Provide a name for the pipeline you're creating and proceed.

![image](https://github.com/user-attachments/assets/5bb8ab34-9776-481b-8a7a-0a370302254b)

   
3. **Add the Copy Data Activity**  
   On the next screen, click **Pipeline activity** and select the **Copy Data** task for your copy operation.

![image](https://github.com/user-attachments/assets/f7b21d0e-0c96-43b8-8329-9ba657761895)


4. **Define Source and Destination**  
   Specify the source and destination where the data will be copied. Then, click the **Run** button in the upper panel to execute the pipeline.

![image](https://github.com/user-attachments/assets/e32c4257-de75-4b2b-874e-421e7d74fe1e)


5. **Execution Confirmation**  
   The pipeline runs successfully.

![image](https://github.com/user-attachments/assets/3733920b-5bb8-47d6-9013-c64cac81769b)


6. **Verify Data in Lakehouse**  
   Confirm that the data has been successfully transferred to the `sales_copy` table within the lakehouse.

![image](https://github.com/user-attachments/assets/840a14b3-e801-4747-89dd-94bdf4dc3e4c)

