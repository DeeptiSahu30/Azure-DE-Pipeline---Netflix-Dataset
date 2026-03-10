## 📌 Project Overview

This project demonstrates an **end-to-end Azure Data Engineering pipeline** that ingests Netflix dataset files, processes them using **Azure Databricks**, 
and builds analytical tables using **Medallion Architecture (Bronze, Silver, Gold)**.
The pipeline includes **data ingestion, transformation, data quality checks, and analytics-ready tables** for reporting.

---

## Workflow Diagram
<img width="1536" height="1024" alt="Workflow" src="https://github.com/user-attachments/assets/36f52818-361b-4649-a1cb-09227cf6ba4c" />


## ⚙️ Technologies Used

* Azure Data Factory
* Azure Data Lake Storage Gen2
* Azure Databricks
* Delta Live Tables
* Unity Catalog
* PySpark
* Databricks Workflows
* Power BI

---


### Pipeline Flow

1. **Data Source** - Netflix dataset stored in GitHub and Azure Data Lake.

2. **Data Ingestion** - Azure Data Factory pipelines ingest raw data into ADLS.

3. **Raw Layer (Bronze)** - Databricks Autoloader ingests raw files into Delta tables.

4. **Cleaned Layer (Silver)** - PySpark transformations clean and standardize data.

5. **Business Layer (Gold)** - Delta Live Tables build aggregated analytical tables.

6. **Analytics** - Data is queried via Databricks SQL Warehouse and visualized in Power BI dashboards.

---


## 🧱 Medallion Architecture

### Bronze Layer

* Raw data ingestion using **Databricks Autoloader**
* Data stored as **Delta tables**

### Silver Layer

* Data cleaning
* Type casting
* Handling null values
* Data standardization

### Gold Layer

* Aggregated tables
* Business-level metrics
* Optimized for analytics

---

## 👨‍💻 Author

**Deepti Sahu**

Aspiring Data Engineer | Azure | Databricks | PySpark
