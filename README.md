# Data Warehouse and Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository! 🚀  
This project demonstrates a comprehensive data warehousing and analytics solution, from building a data warehouse to generating actionable insights. 

---
## 🏗️ Data Architecture

The data architecture for this project follows Medallion Architecture **Bronze**, **Silver**, and **Gold** layers:
![Data Architecture](docs/data_architecture.png)

# Data Warehouse and Analytics Project 🚀

A modern **SQL Server Data Warehouse and Analytics project** built using **Medallion Architecture (Bronze, Silver, Gold)**. The project demonstrates an end-to-end data engineering workflow, from ingesting raw ERP and CRM data to creating a business-ready **Star Schema** for analytics and reporting.

---

## 🏗️ Data Architecture

The project follows the **Medallion Architecture**:

![Data Architecture](docs/data_architecture.png)

### 🥉 Bronze Layer

Stores raw data from the source systems with minimal transformation.

* Ingests ERP and CRM CSV files
* Preserves source data
* Acts as the initial staging layer

### 🥈 Silver Layer

Cleans and transforms the raw data.

* Handles missing and invalid values
* Standardizes data formats
* Removes duplicates
* Applies data quality rules
* Integrates ERP and CRM data

### 🥇 Gold Layer

Contains business-ready data optimized for analytics.

* Fact tables
* Dimension tables
* Star Schema
* Business-friendly data
* Optimized for reporting and analytical queries

---

## 📖 Project Overview

This project demonstrates an end-to-end data warehouse implementation using SQL Server.

### Key Components

1. **Data Architecture**

   * Bronze → Silver → Gold architecture
   * Separation of raw, cleaned, and analytical data

2. **ETL Pipelines**

   * Extract data from ERP and CRM CSV files
   * Load raw data into the Bronze layer
   * Clean and transform data in the Silver layer
   * Create analytical models in the Gold layer

3. **Data Modeling**

   * Fact and dimension tables
   * Star Schema
   * Relationships between business entities

4. **Data Quality**

   * Invalid data handling
   * Duplicate detection
   * Data standardization
   * Data validation

5. **Analytics & Reporting**

   * Customer behavior analysis
   * Product performance analysis
   * Sales trend analysis
   * Business reporting using SQL

---

## 🛠️ Technologies Used

* **SQL Server**
* **SQL**
* **SQL Server Management Studio (SSMS)**
* **ETL / ELT**
* **Medallion Architecture**
* **Star Schema**
* **Data Modeling**
* **Draw.io**
* **Git & GitHub**

---

## 📊 Data Sources

The project integrates data from two source systems.

### ERP

Contains operational business data related to:

* Customers
* Products
* Sales
* Orders

### CRM

Contains customer-related and business information.

The source data is provided as **CSV files** and integrated into a centralized SQL Server Data Warehouse.

---

## 🔄 ETL Workflow

```text
ERP CSV Files ──────┐
                    │
CRM CSV Files ──────┤
                    ▼
              Bronze Layer
                Raw Data
                    │
                    ▼
              Silver Layer
          Cleaned & Transformed
                    │
                    ▼
               Gold Layer
              Star Schema
                    │
                    ▼
          SQL Analytics & Reports
```

---

## ⭐ Data Model

The Gold layer follows a **Star Schema**.

### Fact Tables

Store measurable business events such as:

* Sales
* Orders
* Revenue
* Quantity

### Dimension Tables

Provide descriptive information such as:

* Customers
* Products
* Dates

This structure makes analytical queries easier to write and improves reporting performance.

---

## 📊 SQL Analytics

The project contains multiple SQL scripts for exploring the warehouse and generating business insights.

### Exploration & Analysis

| Script                             | Purpose                                         |
| ---------------------------------- | ----------------------------------------------- |
| `00_init_database.sql`             | Initializes the database                        |
| `01_database_exploration.sql`      | Explores database structure and objects         |
| `02_dimensions_exploration.sql`    | Explores dimension tables                       |
| `03_date_range_exploration.sql`    | Analyzes available date ranges                  |
| `04_measures_exploration.sql`      | Explores key business measures                  |
| `05_magnitude_analysis.sql`        | Performs magnitude analysis                     |
| `06_ranking_analysis.sql`          | Ranks customers/products based on metrics       |
| `07_change_over_time_analysis.sql` | Analyzes trends over time                       |
| `08_cumulative_analysis.sql`       | Performs cumulative analysis                    |
| `09_performance_analysis.sql`      | Analyzes business performance                   |
| `10_data_segmentation.sql`         | Segments customers/products                     |
| `11_part_to_whole_analysis.sql`    | Analyzes contribution to total business metrics |
| `12_report_customers.sql`          | Generates customer analytics report             |
| `13_report_products.sql`           | Generates product analytics report              |

---

## 📂 Repository Structure

```text
Data-Warehouse-and-Analytics/
│
├── datasets/
│   └── Raw ERP and CRM CSV files
│
├── docs/
│   ├── etl.drawio
│   ├── data_architecture.drawio
│   ├── data_architecture.png
│   ├── data_catalog.md
│   ├── data_flow.drawio
│   ├── data_models.drawio
│   ├── naming-conventions.md
│   └── requirements.md
│
├── scripts/
│   │
│   ├── bronze/
│   │   └── Bronze layer ETL scripts
│   │
│   ├── silver/
│   │   └── Silver layer transformation scripts
│   │
│   ├── gold/
│   │   └── Gold layer modeling scripts
│   │
│   ├── 00_init_database.sql
│   ├── 01_database_exploration.sql
│   ├── 02_dimensions_exploration.sql
│   ├── 03_date_range_exploration.sql
│   ├── 04_measures_exploration.sql
│   ├── 05_magnitude_analysis.sql
│   ├── 06_ranking_analysis.sql
│   ├── 07_change_over_time_analysis.sql
│   ├── 08_cumulative_analysis.sql
│   ├── 09_performance_analysis.sql
│   ├── 10_data_segmentation.sql
│   ├── 11_part_to_whole_analysis.sql
│   ├── 12_report_customers.sql
│   └── 13_report_products.sql
│
├── tests/
│   └── Data quality and validation scripts
│
├── README.md
├── LICENSE
├── .gitignore
├── requirements.txt
└── FUNDING.yml
```

---

## 🧪 Data Quality

The project includes data quality checks to improve the reliability of analytical data.

Examples include:

* Duplicate detection
* Missing-value handling
* Invalid-value handling
* Data type validation
* Data standardization
* Referential integrity checks

---

## 📈 Business Analytics

The warehouse supports analysis in three major areas.

### Customer Behavior

* Customer purchasing patterns
* Customer segmentation
* Customer sales performance
* Customer contribution to revenue

### Product Performance

* Product sales performance
* Quantity sold
* Top-performing products
* Product contribution to revenue

### Sales Trends

* Revenue trends
* Sales over time
* Order trends
* Cumulative sales
* Business performance

---

## 🎯 Project Objectives

The main objectives are to:

* Build a centralized SQL Server Data Warehouse
* Integrate ERP and CRM data
* Implement Bronze, Silver, and Gold layers
* Apply data cleansing and transformation
* Build a Star Schema
* Perform SQL-based analytics
* Generate meaningful business insights
* Create reusable analytical reports

---

## 🚀 How to Run

### 1. Install SQL Server

Install SQL Server and SQL Server Management Studio (SSMS).

### 2. Clone the Repository

```bash
git clone https://github.com/UtkarshReddyNathala/Data-Warehouse-and-Analytics.git
```

### 3. Load the Source Data

Place the ERP and CRM CSV files inside the `datasets/` directory.

### 4. Initialize the Database

Run:

```text
scripts/00_init_database.sql
```

### 5. Run the ETL Pipeline

Execute the SQL scripts in the following order:

```text
Bronze
  ↓
Silver
  ↓
Gold
```

### 6. Run Analytics

Execute the analysis scripts from:

```text
scripts/01_database_exploration.sql
```

through:

```text
scripts/13_report_products.sql
```

to explore the warehouse and generate analytical reports.

---

## 🧪 Testing

The `tests/` directory contains scripts used to validate data quality and ensure that the warehouse produces reliable results.

---

## 📚 Skills Demonstrated

This project demonstrates practical experience in:

* SQL Development
* Data Engineering
* ETL Pipelines
* Data Warehousing
* Data Modeling
* Medallion Architecture
* Star Schema
* Data Quality
* SQL Analytics
* Business Intelligence
* Analytical Reporting

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Utkarsh Reddy Nathala**

GitHub: https://github.com/UtkarshReddyNathala
