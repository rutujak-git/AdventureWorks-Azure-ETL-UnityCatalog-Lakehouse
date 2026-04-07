# AdventureWorks-Azure-ETL-UnityCatalog-Lakehouse
End-to-end Azure Data Engineering project from scratch using AdventureWorks2022 dataset, implementing full ETL pipeline with SSMS,Azure SQL DB, ADF, ADLS Gen2, Databricks (Unity Catalog), and Power BI dashboards.

# End-to-End Data Engineering Pipeline using Azure & Databricks

## 📌 Overview
I have created this project from scratch and published it on my YouTube Channel : www.youtube.com/@DataToCrunch .
This project demonstrates a real-world **Azure Data Engineering pipeline** built from scratch using the AdventureWorks2022 dataset. 

<img width="1649" height="922" alt="image" src="https://github.com/user-attachments/assets/cb61f250-0233-4bcb-bdb6-55f87d2fc870" />


The pipeline simulates enterprise ingestion and processing patterns through a **Medallion Architecture** (Bronze, Silver, Gold), ensuring clean, governed, and analytics-ready data for business intelligence.

---

## 🏗️ Architecture

AdventureWorks2022 → On-Prem SQL Server → Azure SQL DB → Azure Data Factory → ADLS Gen2 (Bronze) → Databricks (Silver & Gold) → Power BI

<img width="2126" height="1307" alt="image" src="https://github.com/user-attachments/assets/b94b896e-1f28-4223-b15a-058196ea7342" />


---

## ⚙️ Tech Stack

- SSMS
- Azure SQL Database
- Azure Data Factory (ADF)
- Azure Data Lake Storage Gen2 (ADLS)
- Azure Databricks + Unity Catalog
- Delta Lake
- Power BI
- GitHub

---

## 🔄 Pipeline Flow

### 🔹 Data Source
- Dataset: AdventureWorks2022  
- Stored in SSMS
- Pulled into Azure SQL Database from SSMS

### 🔹 Ingestion (ADF)
- Azure Data Factory pipelines move raw data from SQL DB to ADLS Bronze layer
- Handles orchestration and data movement

### 🔹 Bronze Layer
- Raw, unprocessed data in Delta format
- Append-only ingestion for traceability

### 🔹 Silver Layer
- Data cleaning and transformations
- Schema enforcement and data validation

### 🔹 Gold Layer
- Business-level aggregations
- Analytics-ready datasets

### 🔹 Visualization
- Power BI dashboards connected to Gold layer

---

## 🚀 Key Features

- End-to-end Azure & Databricks data pipeline  
- Medallion architecture (Bronze → Silver → Gold)  
- Secure governance via Unity Catalog  
- Delta Lake for reliable data storage  
- Scalable and modular design  
- Orchestration with ADF  

---

## ▶️ How to Run

1. Provision Azure resources:
   - Azure SQL DB(stores data from SSMS), ADLS Gen2, Databricks Workspace (Unity Catalog), Power BI
2. Configure ADF pipelines to move data from SQL DB to ADLS Bronze
3. Load raw data into Bronze layer
4. Run Databricks notebooks for:
   - Silver transformations (data cleaning)
   - Gold aggregations (analytics-ready datasets)
5. Connect Power BI to Gold layer dashboards

---

## 🎥 YouTube Walkthrough
https://youtu.be/Mzxn0eGKfso?si=hYrdH0qsXuAeTq6R

---

## 📌 Dataset

https://www.kaggle.com/datasets/algorismus/adventure-works-in-excel-tables?select=Product.csv
