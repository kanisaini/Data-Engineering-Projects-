# 🏅 Azure Data Engineering Project – Tokyo Olympic Data Pipeline

## 📌 Overview

This project demonstrates an end-to-end Azure Data Engineering pipeline built using the Tokyo Olympic dataset. The goal was to design a scalable, cloud-native data architecture to ingest, transform, and analyze data using modern Azure services.

## 🏗️ Architecture

The pipeline follows a modern data engineering workflow:

### HTTP Source → Azure Data Factory → Azure Data Lake Storage Gen2 → Azure Databricks (PySpark) → ADLS Gen2 → Azure Synapse Analytics

![Sales Dashboard](https://github.com/kanisaini/Data-Engineering-Projects-/blob/main/Tokyo%20Olympics%20Data%20Engineering%20Project/Architecture%20diagram.png)

## 🔄 Project Workflow
### 🔹 Data Ingestion – Azure Data Factory
Ingested Tokyo Olympic dataset from an HTTP source
Used Azure Data Factory (ADF) for orchestration
Implemented Copy Activity to move raw data into ADLS Gen2
Enabled scalable and monitored data movement
### 🔹 Data Transformation – Azure Databricks
Performed data cleaning and transformations using PySpark
Processed data stored in ADLS Gen2
Wrote transformed data back to storage
### 🔹 Data Analytics – Azure Synapse Analytics
Connected Synapse to transformed data in ADLS Gen2
Created external tables
Used Serverless SQL Pool for querying data without infrastructure setup
Performed aggregation and analysis on Olympic datasets
🚀 Key Learnings
Built a complete end-to-end data pipeline on Azure
Understood how ADF orchestrates workflows efficiently
Gained hands-on experience with Databricks & PySpark
Learned how to query data directly from storage using Synapse Serverless SQL
Explored integration between multiple Azure services
💡 Engineering Insights
✔️ What Worked Well
ADF Copy Activity simplified data ingestion
Seamless integration across Azure services
Synapse Serverless SQL enabled fast data exploration
⚖️ Trade-offs
Dataset was small → Databricks introduced unnecessary cost
Simpler transformations could be handled within ADF

👉 Lesson: Always choose the right tool based on workload

🔧 Improvements for Future
Convert data from CSV → Parquet for better performance
Implement full Medallion Architecture (Bronze → Silver → Gold)
Optimize pipeline for cost and scalability
🛠️ Tech Stack
Azure Data Factory
Azure Data Lake Storage Gen2
Azure Databricks
PySpark
Azure Synapse Analytics
Serverless SQL Pool
SQL
📈 Conclusion

This project highlights how to design a modern data pipeline using Azure services. It reinforces the importance of balancing performance, cost, and simplicity when building scalable data solutions.
