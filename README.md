# Azure-Data-Engineering-Project
# End-to-End Azure Data Engineering Project

This repository contains an end-to-end data engineering project on Azure, involving data ingestion, transformation, analytics, and visualization.

## Project Overview
This project demonstrates how to build a data pipeline using:
- **Azure Data Factory (ADF)** for data ingestion
- **Azure Data Lake** for structured storage
- **Azure Databricks** for transformations
- **Azure Synapse Analytics** for querying and reporting
- **Power BI** for visualization

## Steps
## Datasource:
https://github.com/anshlambaoldgit/Adventure-Works-Data-Engineering-Project/tree/main/Data


### 1. **Setup & Configuration**
- Create an Azure **Resource Group** and **Data Lake** (with hierarchical namespaces).
- Create **Containers** in Data Lake: `bronze`, `silver`, `gold`.

### 2. **Data Ingestion (Azure Data Factory)**
- Create **Linked Services** (connections to data sources and sinks).
- Create **Datasets** for source (GitHub) and sink (Azure Data Lake).
- Develop a **Pipeline** to load data into the `bronze` layer.
- Use **dynamic parameters** to pull multiple datasets efficiently.
- Perform **lookup operations** using `git.json`.


![Screenshot 2025-03-04 232627](https://github.com/user-attachments/assets/a6228ad3-ddea-47f6-b302-c6b5a6616f12)

### 3. **Data Transformation (Azure Databricks)**
- Register Databricks as a **service principal** for Data Lake access.
- Obtain and configure **secrets** for authentication.
- Assign **Storage Blob Contributor** role for read/write access.
- Use Databricks notebooks and pyspark to transform data (`silver` layer).
- Perform data visualization in Databricks.

![Screenshot 2025-03-08 160022](https://github.com/user-attachments/assets/1c0d089a-9409-4d5a-8aef-8755696b1281)



### 4. **Data Analytics (Azure Synapse)**
- Create **Synapse Analytics Workspace** and connect to Data Lake.
- Use **OPENROWSET** to query data from the `silver` layer.
- Create **Views** and **External Tables** for efficient querying.
- Define **Master Key** for secure access.

![Screenshot 2025-03-08 155857](https://github.com/user-attachments/assets/e8138283-80cd-45e5-b208-7503c57f1548)



### 5. **Reporting & Visualization (Power BI)**
- Connect **Synapse Analytics** to Power BI using SQL endpoints.
- Load transformed data into Power BI for dashboards.


![Screenshot 2025-03-08 153656](https://github.com/user-attachments/assets/b7cf89ed-ef1b-4d11-89e7-9d6a24a61cf0)

## Key Features:  
✔️ Scalable **ETL pipelines** in **ADF**  

✔️ Serverless querying with **Synapse Analytics**

✔️ Integration with **Power BI** for visualization  



