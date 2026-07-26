# Netflix_Azure_Data_Engineering_Project

## 📌 Overview
This project demonstrates an end-to-end data engineering pipeline using Azure services.

## 🏗️ Architecture
![Architecture](images/architecture.png)

## ⚙️ Tech Stack
- Azure Data Factory
- Azure Databricks
- Delta Live Tables
- Azure Data Lake Gen2
- Azure Synapse Analytics
- Power BI

## 🔄 Pipeline Flow
1. Data Ingestion using ADF
2. Raw Data stored in Data Lake (Bronze)
3. Transformation using Databricks (Silver)
4. Star Schema modeling (Gold)
5. Data loaded into Azure Synapse
6. Reporting using Power BI

## 📊 Key Features
- Incremental Data Loading
- Medallion Architecture (Bronze, Silver, Gold)
- Star Schema Design
- Scalable ETL Pipeline




## 🚀 How to Run
1. Set up Azure resources
2. Configure ADF pipeline
3. Run Databricks notebooks
4. Query data in Synapse
