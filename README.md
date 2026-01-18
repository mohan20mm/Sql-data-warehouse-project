📊 Data Warehouse Project – Medallion Architecture (Bronze, Silver, Gold)

### 🔍 Project Overview

This project demonstrates the design and implementation of a **modern data warehouse** using the **Medallion Architecture**, structured into **Bronze**, **Silver**, and **Gold** layers. The objective is to build a scalable, maintainable, and analytics-ready data platform that transforms raw source data into trusted business insights.

The project follows industry best practices in **data engineering**, **ETL development**, and **dimensional modeling**, making it suitable for real-world enterprise use cases as well as professional portfolios.

---
<img width="1598" height="912" alt="data_architecture" src="https://github.com/user-attachments/assets/cc1b93e3-fd03-4d88-9bc0-0d2cd1ec3a92" />

---

### 🏗️ Data Architecture – Medallion Framework

The data warehouse is organized into three logical layers, each serving a distinct purpose:

#### 🟤 Bronze Layer – Raw Data Ingestion

* Stores raw data ingested directly from source systems (CSV files, external feeds, etc.)
* Minimal to no transformations applied
* Preserves original data structure for traceability and auditing
* Serves as the system of record for downstream processing

#### ⚪ Silver Layer – Cleansed & Transformed Data

* Performs data cleansing, standardization, and validation
* Applies business rules and data quality checks
* Resolves data type issues, duplicates, and inconsistencies
* Prepares structured datasets optimized for analytical modeling

#### 🟡 Gold Layer – Business-Ready Data

* Represents the final **analytical layer**
* Implements **Star Schema** design with **Fact** and **Dimension** tables
* Aggregated, enriched, and optimized for high-performance queries
* Designed to support reporting, dashboards, and decision-making

---

### 🔄 ETL Pipelines

The project includes end-to-end **ETL pipelines** that:

* Extract data from external source systems
* Load raw data into the Bronze layer
* Transform and cleanse data into the Silver layer
* Model and publish analytics-ready datasets in the Gold layer

ETL logic is implemented using **SQL-based transformations**, ensuring transparency, maintainability, and performance.

---

### 📐 Data Modeling

* Fact tables capture measurable business events
* Dimension tables provide descriptive business context
* Schema design is optimized for analytical workloads and BI tools

---

### 📈 Analytics & Reporting

* Gold-layer views and tables are directly queryable
* Designed to support:

  * Ad-hoc analysis
  * SQL-based reporting
  * BI dashboards
* Enables fast, reliable access to trusted business metrics

---

### 🎯 Skills & Expertise Demonstrated

This repository showcases hands-on expertise in:

* **SQL Development**
* **Data Engineering**
* **ETL Pipeline Design**
* **Modern Data Architecture**
* **Medallion Architecture Implementation**
* **Dimensional Data Modeling**
* **Analytics & Reporting**

---

### 👨‍💼 Ideal For

This project is an excellent resource for:

* Data Engineers
* Data Architects
* ETL Developers
* SQL Developers
* Data Analysts
* Students building real-world data engineering portfolios

---
🛠️ Important Links & Tools:
---

* [Datasets](https://github.com/mohan20mm/Sql-data-warehouse-project/tree/71b960912210dabc26469f5ecb195f75c788cc8e/datasets): Access to the project dataset (csv files).
* [SQL Server Express](https://www.microsoft.com/en-in/sql-server/sql-server-downloads): Lightweight server for hosting your SQL database.
* [SQL Server Management Studio](https://learn.microsoft.com/en-us/ssms/install/install): GUI for managing and interacting with databases.
* [Notion](https://www.notion.so/Data-Warehouse-Project-284130c3c44280deaf77e62c98af7be1?source=copy_link): Get the Project Template from Notion
* [Draw.io](https://www.drawio.com/): Design data architecture, models, flows, and diagrams.
* [GIT Repository](https://github.com/git/git): Set up a GitHub account and repository to manage, version, and collaborate on your code efficiently.
---
\🚀 Project Requirements
Building the Data Warehouse (Data Engineering)
Objective
Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical reporting and informed decision-making.

Specifications
* Data Sources: Import data from two source systems (ERP and CRM) provided as CSV files.
* Data Quality: Cleanse and resolve data quality issues prior to analysis.
* Integration: Combine both sources into a single, user-friendly data model designed for analytical queries.
* Scope: Focus on the latest dataset only; historization of data is not required.
* Documentation: Provide clear documentation of the data model to support both business stakeholders and analytics teams
---
📂 Repository Structure
--
data-warehouse-project/
│
├── datasets/                           # Raw datasets used for the project (ERP and CRM data)
│
├── docs/                               # Project documentation and architecture details
│   ├── etl.drawio                      # Draw.io file shows all different techniquies and methods of ETL
│   ├── data_architecture.drawio        # Draw.io file shows the project's architecture
│   ├── data_catalog.md                 # Catalog of datasets, including field descriptions and metadata
│   ├── data_flow.drawio                # Draw.io file for the data flow diagram
│   ├── data_models.drawio              # Draw.io file for data models (star schema)
│   ├── naming-conventions.md           # Consistent naming guidelines for tables, columns, and files
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Scripts for extracting and loading raw data
│   ├── silver/                         # Scripts for cleaning and transforming data
│   ├── gold/                           # Scripts for creating analytical models
│
├── tests/                              # Test scripts and quality files
│
├── README.md                           # Project overview and instructions
├── LICENSE                             # License information for the repository

---
This implementation reflects real enterprise data warehouse patterns and demonstrates the ability to design, build, and maintain a scalable analytics platform from raw data to business insights.
