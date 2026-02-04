# End-to-End Lakehouse Architecture

This repository contains a full Bronze–Silver–Gold Lakehouse implementation using Databricks for a retail company. It includes datasets, notebooks, scripts, and documentation that illustrate the entire value stream—from data ingestion and transformation to analytics-ready data products.

---

## 1. Challenges

• Multiples data sources

• Finance and operations don’t report the same numbers

• Reports are produced too late

• Operations data are difficult to use / not easily actionable

• IT is constantly in firefighting mode

• 80% time on data prep

• Slow query performance

• No self service capability

---

## 2. Solution

The solution approach consists of designing and implementing a complete Lakehouse architecture following the Medallion pattern—ingesting raw data, transforming it with PySpark, and aggregating it into a star schema to enable fast, self-service analytics.

### 🥉 Bronze Layer
- Raw data ingestion  
- Schema inference and storage as Delta tables  

### 🥈 Silver Layer
- Data cleaning and standardization  
- Type casting and validation  

### 🥇 Gold Layer
- Dimensional Data Model (Business Transformation)
- Ready for BI and analysis

---

## 3. Solution architecture

<img width="1230" height="760" alt="Screenshot 2026-02-04 134222" src="https://github.com/user-attachments/assets/74801d4b-73f8-4430-a34c-93bd9d9f8847" />

---

## 4. Technologies Used

- Databricks  
- Apache Spark  
- PySpark  
- Spark SQL  
- Delta Lake  
- Unity Catalog

---

## 5. Results & Impacts

• 80% Times saving
(analysts now focus on insights instead of SQL gymnastics)

• Self-service Enabled
(Business users create theirs own reports from the star schema)

• 10x Query time performance

• Isolated analytics workload
(Analytics workload runs on Lakehouse, not on operational system)

• Accurate numbers, faster closing cycles

• Governance embedded from day one

• Aligned decision-making enabled by a single source of truth
