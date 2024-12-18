# Microsoft Fabric Introduction

Microsoft Fabric is a comprehensive analytics platform that enables companies to manage their projects collaboratively with IT staff. Fabric provides an integrated service for data collection, storage, processing, and analysis.

Microsoft Fabric offers companies a wide range of tools covering various services such as information technology, data integration, data warehousing, real-time analytics, data science, and business intelligence. This platform is an ideal solution for organizations looking to make data-driven decisions.

Fabric facilitates collaboration among data workers, simplifying processes and helping companies manage and analyze data effectively.

![image](https://github.com/aysegulyigitbi/Microsoft-Fabric/assets/127193220/96bef429-966f-4be7-a4b3-5703993b2f2c)

For Turkish: https://turkiyeyayini.com/microsoft-fabrice-giri%C5%9F-8941f476c660

## Advantages of Using Microsoft Fabric

### Comprehensive Integrated Analytics
Microsoft Fabric provides access to the most comprehensive analytics in the industry. Users can quickly and easily reuse their data assets.

### Centralized Data Storage
Via OneLake, data storage can be centralized. Instead of dealing with different databases or data warehouses, Fabric allows for more efficient data management.

### AI Integration
Fabric seamlessly integrates AI features, eliminating the need for manual integration. This transforms raw data into actionable insights for business users, making it easy to access insights.

### SaaS-Based Solution
Microsoft Fabric is built on a Software-as-a-Service (SaaS) foundation, offering customized user experiences by integrating components from various services such as Power BI, Azure Synapse Analytics, and Azure Data Factory.

### Centralized Management
Fabric integrates data and services seamlessly, providing centralized management, administration, and discovery. Permissions are applied automatically, and data sensitivity labels are inherited across all components of the package.

## End-to-End Data Analytics with Microsoft Fabric

Microsoft Fabric provides a scalable data analytics solution that eliminates the complexities of complex analytics processes. Fabric can be used as a single product that is easy to understand, easy to set up, and easy to manage. The platform offers an integrated user interface that provides customized, optimized experiences and tools.

In addition to simplifying the user experience, Fabric stores all your data in a single OneLake service. This SaaS is available on all platform analytics engines. Fabric offers advantages such as scalability, cost efficiency, and availability wherever there is an internet connection. Additionally, Microsoft ensures the platform is up-to-date and performs optimally through continuous updates and maintenance.

## OneLake

OneLake is an integrated architecture within Fabric for data workers and organizations collaborating on data projects. OneLake architecture facilitates collaboration among data teams and eliminates the need to transfer and copy data between different systems, saving time. OneCopy, a core component of OneLake, optimizes data management by allowing data to be read from a single copy.

OneLake consolidates data into a single region without the need to transfer or replicate data across different regions and cloud storage locations. This can be thought of like the corporate OneDrive for Office applications; all computing workloads within Fabric are pre-integrated with OneLake. Features such as data warehouse, data engineering (Lakehouse), data integration (pipelines and dataflows), real-time intelligence, and Power BI within Fabric use OneLake as the native store without requiring additional configuration.

![image](https://github.com/aysegulyigitbi/Microsoft-Fabric/assets/127193220/0e5274ba-7571-4311-8a11-151749155d57)

OneLake is built on Azure Data Lake Storage (ADLS) and allows data to be stored in various formats such as Delta, Parquet, CSV, and JSON.

This ensures that all compute engines within Fabric automatically store data in OneLake. All compute engines can directly access data stored in OneLake without the need for moving or copying the data. For tabular data, the analytics engines in Fabric can write data in delta-parquet format, which interacts seamlessly with all engines.

A notable feature of OneLake is its ability to create shortcuts, which are embedded references. These shortcuts allow you to source existing cloud data quickly without the need to copy it, and Fabric experiences always derive data from the same source, keeping it synchronized.

![image](https://github.com/aysegulyigitbi/Microsoft-Fabric/assets/127193220/745f067b-419e-4f08-9cd8-d00585468170)

**Note:** Delta Lake offers robust processing capabilities on data stored in Parquet format. Parquet is a compressed, columnar file format optimized for large-scale data processing. The integration of Delta Lake with Parquet format provides advantages such as reliability, integrity, and transaction history tracking when managing data storage, querying, updating, and processing.

## Fabric Experiences

Fabric offers a set of analytics experiences designed to perform specific tasks and work seamlessly together.

- **Synapse Data Engineering:** Provides data engineering with the Spark platform for large-scale data transformation.
- **Synapse Data Warehouse:** Delivers a data warehouse with industry-leading SQL performance and scalability for data consumption.
- **Synapse Data Science:** Provides data science with Azure Machine Learning and Spark for model training and execution tracking in a scalable environment.
- **Synapse Real-Time Intelligence:** Used to query and analyze large volumes of data in real-time.
- **Data Factory:** Provides data integration by combining Power Query with Azure Data Factory scale for moving and transforming data.
- **Power BI:** Delivers business intelligence to turn data into decisions.

## Reference

Microsoft. (2024). Microsoft Fabric Analytics Engineer Course Materials. https://learn.microsoft.com/en-us/training/courses/dp-600t00
