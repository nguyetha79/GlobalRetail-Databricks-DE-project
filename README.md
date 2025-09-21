# Global Retail Databricks Data Engineering Project

## 1. Case Study Overview
The case study focuses on GlobalRetail, a multinational retail corporation with over 11,000 stores and a robust e-commerce platform, generating massive amounts of data daily.

## 2. Data Management Goals
- Consolidate **global data sources**.  
- Accelerate **data processing and analysis**.  
- Improve **decision-making capabilities**.  
- Enable **real-time, company-wide analytics**.  

## 3. Data Sources
- **Customer Data**  
  - Format: `.csv` files  
  - Source: CRM system  
  - Volume: ~500 million records  

- **Product Catalog**  
  - Format: `.json` files  
  - Source: Inventory management system  
  - Volume: ~0.5 million SKUs  

- **Transaction History**  
  - Format: Parquet files  
  - Source: Point-of-sale & e-commerce platform  
  - Volume: ~10 billion transactions annually
 
| Data Sources | Quantity | Format |
|----------|----------|----------|
| Customer Data (CRM)    | 500M records   | `.csv`   |
| Product Catalog   | 1M SKUs   | `JSON` |
| Transaction History   | 10B annual transactions   | `parquet`  |

## 4. Expected Outcomes
-	Reduce processing time
-	Improve inventory forecasting accuracy by 25%
-	Boost repeat purchases by 15%
-	Enable real-time financial reporting across all regions

## 5. Challenges
-	Data quality and inconsistanies
-	Varying format across 27 countries
-	Complex ETL process

## 6. Solution
Implement a **modern data lakehouse architecture** using **Databricks** with a **multi-layer design (Bronze, Silver, Gold)** to ingest, process, and unify data for analytics and reporting.  

## 7. Solution Components

### 🔹 Data Lakehouse Concept
Combines the **flexibility & scalability** of data lakes with the **data management & transaction capabilities** of data warehouses.  

### 🔹 Three-Layer Architecture
- **🟤 Bronze Layer:** Raw data ingestion, maintaining data as received for **auditability**.  
- **⚪ Silver Layer:** Clean and conform data, applying **data quality rules** and managing **schema evolution**.  
- **🟡 Gold Layer:** Business-level aggregates, optimized for **query performance** and connected to **Power BI** for visualization.  

### 🔹 Benefits
- **Scalability** for handling historical data.  
- **Flexibility** for diverse data formats.  
- **Governance** with data lineage, security, and quality controls.  
- **Cost**

## 8.	High-Level Architecture Diagram
![architecture](https://github.com/nguyetha79/GlobalRetail-Databricks-DE-project/blob/main/High-Level%20Architecture%20Diagram.png)

## 9.	Key components
- Databricks Workspace
-	Databricks File System (DBFS)
-	Databricks Clusters
-	Databricks Notebooks
-	Delta Lake
-	Databricks Jobs
