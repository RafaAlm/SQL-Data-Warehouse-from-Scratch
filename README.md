#  SQL Data Warehouse from Scratch
### *End-to-End Data Engineering Pipeline*

---

## 📝 Project Overview
This project demonstrates the complete lifecycle of building a robust **SQL Data Warehouse**. It implements a modular architecture to transform raw data from disparate sources (CRM and ERP systems) into a polished **Star Schema** optimized for high-performance business intelligence and analytics.

---

## 📐 Data Architecture
The project follows the **Medallion Architecture** to ensure data quality, traceability, and a clear separation of concerns:

| Layer | Name | Purpose |
| :--- | :--- | :--- |
| 🥉 | **Bronze** | Raw data ingestion from CRM and ERP systems (Staging). |
| 🥈 | **Silver** | Data cleansing, standardization, and deduplication. |
| 🥇 | **Gold** | Final Dimensional Modeling (**Star Schema**) for business consumption. |

---

## 🛠️ Tech Stack & Concepts
* **Database:** SQL Server / PostgreSQL (Core Engine)
* **Modeling:** Star Schema (Fact & Dimension Tables)
* **Engineering:** ETL/ELT Pipelines, Stored Procedures, Data Mapping
* **Documentation:** Data Catalog, Flow Diagrams, and Naming Conventions

---

## 🚀 Implementation Roadmap

### 1️⃣ Project Initialization
* Defined professional **Naming Conventions** for schemas, tables, and columns.
* Established a **Git-based workflow** for database version control.
* Environment setup including Database and Schema structures.

### 2️⃣ Bronze Layer (Staging)
* Detailed analysis of source systems (CRM & ERP).
* Developed **DDL scripts** for landing tables to mirror source data.
* Built **Stored Procedures** to automate the batch loading of raw data.

### 3️⃣ Silver Layer (Cleansing & Transformation)
* **Data Profiling:** Identified inconsistencies, nulls, and duplicates.
* **Entity Cleansing:** Refined `Customers`, `Products`, and `Sales Details`.
* **Standardization:** Unified date formats and currency units using SQL transformation scripts.

### 4️⃣ Gold Layer (Dimensional Modeling)
* Implemented a **Star Schema** to simplify query logic and improve performance.
* **Dimensions:** Created `dim_customers` and `dim_products` by merging data across systems.
* **Fact Table:** Built `fact_sales` to store business metrics and transactional keys.
* **Data Catalog:** Comprehensive documentation for end-user reference.

---

## 📂 Project Structure
```text
.
├── scripts/
│   ├── bronze/         # DDL and Load scripts for Raw Data
│   ├── silver/         # Cleaning and Transformation logic
│   └── gold/           # Fact and Dimension modeling (Star Schema)
├── docs/               # Architecture Diagrams and Data Flow
└── README.md           # Project documentation
