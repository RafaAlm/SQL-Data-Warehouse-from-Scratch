# SQL-Data-Warehouse-from-Scratch

Project Overview
This project demonstrates the complete lifecycle of building a SQL Data Warehouse. It follows a modular architecture to transform raw data from multiple sources (CRM and ERP systems) into a polished Star Schema optimized for business intelligence and analytics.

Data Architecture
The project is organized into three logical layers (Medallion Architecture) to ensure data quality and traceability:

Bronze Layer (Source): Raw data ingestion from CRM and ERP systems.

Silver Layer (Integration): Data cleansing, standardization, and deduplication.

Gold Layer (Presentation): Final Dimensional Modeling (Star Schema) for business consumption.

🛠️ Tech Stack & Concepts
Database: SQL Server / PostgreSQL (adjust as needed)

Modeling: Star Schema (Facts & Dimensions)

Engineering: ETL/ELT, Stored Procedures, Data Mapping

Documentation: Data Catalog, Data Flow Diagrams, and Naming Conventions

🚀 Implementation Roadmap
1. Project Initialization
Defined naming conventions for schemas, tables, and columns.

Established a Git-based workflow for database version control.

Setup of the core Database and Schemas environment.

2. Bronze Layer (Staging)
Analyzed source systems (CRM/ERP).

Developed DDL scripts for landing tables.

Built Stored Procedures to automate the loading of raw data.

3. Silver Layer (Cleansing & Transformation)
Performed data profiling to identify inconsistencies.

Cleansed key entities: Customers, Products, and Sales Details.

Handled data quality issues (nulls, formatting, and duplicates) using SQL transformation scripts.

4. Gold Layer (Dimensional Modeling)
Implemented a Star Schema to simplify query logic.

Dimensions: Created dim_customers and dim_products by merging CRM and ERP data.

Fact Table: Built fact_sales to store transactional metrics.

Created a Data Catalog for business user reference.

📂 Project Structure
Plaintext
├── scripts/
│   ├── bronze/         # DDL and Load scripts for Raw Data
│   ├── silver/         # Cleaning and Transformation scripts
│   └── gold/           # Fact and Dimension modeling
├── docs/               # Data Flow Diagrams and Architecture
└── README.md
📈 Key Insights & Results
Integrated Data: Unified customer and product data from siloed CRM and ERP systems.

Performance: Optimized the Gold Layer for sub-second analytical queries.

Automation: Full pipeline execution via Stored Procedures.
