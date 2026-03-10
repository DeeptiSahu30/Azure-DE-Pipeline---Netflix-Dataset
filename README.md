## 📌 Project Overview

This project demonstrates an **end-to-end Azure Data Engineering pipeline** that ingests Netflix dataset files, processes them using **Azure Databricks**, 
and builds analytical tables using **Medallion Architecture (Bronze, Silver, Gold)**.
The pipeline includes **data ingestion, transformation, data quality checks, and analytics-ready tables** for reporting.

---

## Workflow Diagram 
<img width="1536" height="1024" alt="ChatGPT Image Mar 10, 2026, 08_55_35 PM" src="https://github.com/user-attachments/assets/2d5cfcfc-84a6-48c1-9d2d-e8addb107fb8" />

---
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
3. **Bronze Layer** - Databricks Autoloader ingests raw files into Delta tables.
4. **Silver Layer** - PySpark transformations clean and standardize data.
5. **Gold Layer** - Delta Live Tables build aggregated analytical tables.
6. **Analytics** - Data is queried via Databricks and visualized in Power BI dashboards.

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
