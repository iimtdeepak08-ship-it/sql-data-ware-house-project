# SQL Data Warehouse Project

## 📌 Project Overview

This project focuses on developing a **modern SQL Server–based data warehouse** to consolidate sales data from multiple source systems and enable **analytical reporting and informed decision-making**.

The solution emphasizes clean data modeling, data quality handling, and business-ready analytics using SQL.

---

## ✅ Specifications

* **Data Sources**: Import data from two source systems (**ERP** and **CRM**) provided as CSV files.
* **Data Quality**: Cleanse and resolve data quality issues prior to analysis (null handling, deduplication, standardization).
* **Integration**: Combine both sources into a single, user-friendly analytical data model.
* **Scope**: Focus on the **latest dataset only**; historization is not required.
* **Documentation**: Provide clear documentation of the data model for business stakeholders and analytics teams.

---

## 🏗️ Architecture

The data warehouse follows a **star schema** approach:

* **Fact Tables** → Store transactional / measurable data
* **Dimension Tables** → Store descriptive attributes

Example layers:

* Staging Layer
* Data Warehouse Layer
* Reporting / Analytics Layer

---

## 🗂️ Database Structure

The warehouse is modeled using a **star schema** for efficient analytics.

### Dimension Tables

* `dim_customer`
* `dim_product`
* `dim_date`

### Fact Tables

* `fact_sales`

Each table uses appropriate data types, primary keys, and foreign key relationships to support analytical queries.

---

## 🧱 Technologies Used

* **SQL Server (SSMS)**
* **T-SQL**
* **draw.io** (for ER & architecture diagrams)

---

## ⚙️ Setup Instructions

1. Install **SQL Server** and **SQL Server Management Studio (SSMS)**
2. Create a database:

   ```sql
   CREATE DATABASE sql_data_warehouse;
   ```
3. Switch to the database:

   ```sql
   USE sql_data_warehouse;
   ```
4. Execute table creation scripts
5. Load sample data using INSERT statements

---

## 📊 BI: Analytics & Reporting (Data Analytics)

### Objective

Develop SQL-based analytics to deliver insights into:

* **Customer Behavior**
* **Product Performance**
* **Sales Trends**

These insights empower stakeholders with key business metrics for strategic decision-making.

### Example Analyses

* Total and average sales by product
* Top customers by revenue
* Monthly and daily sales trends
* Ranking products using window functions

---

## 🎯 Learning Outcomes

By completing this project, you will learn:

* How data warehouses are structured
* Difference between OLTP and OLAP
* Fact vs Dimension tables
* Writing analytical SQL queries
* Interview-ready SQL concepts

---

## 🧠 Interview Relevance

This project helps answer questions like:

* How do you design a data warehouse?
* What is a star schema?
* How do fact and dimension tables differ?
* How do you optimize SQL queries for analytics?

---

## 📈 Future Enhancements

* Add ETL pipelines
* Integrate with Power BI / Tableau
* Add incremental data loading
* Implement indexing and partitioning

---

## 👤 Author

**Deepak Singh**
Software Developer | Aspiring Data Engineer

---

## 📜 License

This project is licensed under the **MIT License**. You are free to use, modify, and distribute this project with proper attribution.

---

## ⭐ Notes

This project is created for **learning, hands-on practice, and interview preparation**. The structure and documentation are inspired by real-world data engineering use cases.

Happy Learning 🚀
