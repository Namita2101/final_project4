Medallion Architecture in Microsoft Fabric 🚀

This project implements the Medallion Architecture in Microsoft Fabric, leveraging PySpark and data pipelines. The architecture has three stages: Bronze, Silver, and Gold.


Stage 1: Bronze - Raw Data (Lakehouse) 📥
Goal: Store raw, unprocessed data in the Bronze Lakehouse.

Actions:

Ingest data without transformations ❌


Stage 2: Silver - Cleaned Data (Lakehouse) 🧹
Goal: Clean and preprocess the data in the Silver Lakehouse.

Actions:

Remove duplicates 

Handle null values 

Cast data types for consistency 

Store cleaned data in Silver Lakehouse 🏠


Stage 3: Gold - Transformed Data (Warehouse) 💎
Goal: Apply business logic, aggregation, and transformations in the Gold Warehouse for reporting.

Actions:

Copy Data: Transfer data from Silver Lakehouse to Gold Warehouse 🔄

SQL Transformations: Perform joins, apply business logic, and aggregate data using SQL 

Audit Log: Record each transformation in the audit log for tracking changes 

Automation: Trigger transformations automatically after the data copy via a Stored Procedure ⚙️

This project efficiently processes data in stages, ensuring clean, transformed, and business-ready datasets for final analysis and reporting. 🎯

Note: The project_files_warehouse_queries consists of all the queries(transformation, business logic and also of table that can be used in Power BI.
