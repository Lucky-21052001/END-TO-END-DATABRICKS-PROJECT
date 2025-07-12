![Screenshot (166)](https://github.com/user-attachments/assets/a0c49050-8a1a-4c1d-90df-bca4aa0ba8e2)

✈️ Flight Analytics Pipeline – End-to-End Lakehouse Project with Delta Live Tables & dbt
📌 Overview
This project demonstrates a complete end-to-end data engineering pipeline for flight data analytics using Databricks Delta Live Tables (DLT) and dbt. It follows the medallion architecture (bronze, silver, gold) to build a reliable and governed lakehouse system. The goal is to showcase scalable ingestion, reusable transformation logic, automated data quality enforcement, and curated insights ready for reporting and analysis.

🏗️ Architecture: Medallion Lakehouse
Bronze Layer (Raw Ingestion): Ingest raw flight-related data using Databricks Auto Loader with schema inference.

Silver Layer (Transformed): Clean, validate, and enrich data using PySpark transformations and Delta Live Tables.

Gold Layer (Curated): Create analytical fact and dimension tables using dbt for consumption by BI tools.

⚙️ Key Components & Features
1. Auto Loader with Delta Live Tables

        Automatically ingests data from cloud storage.

        Handles schema evolution and scalable streaming ingestion into the bronze layer.

2. Parameterized PySpark Functions

        Dynamically generate dimension tables (e.g., airports, airlines).

        Improve code reusability and maintainability across ETL pipelines.

3. Delta Live Tables with Data Quality Expectations

        Apply rules like expect_all_or_drop and expect_or_drop.

        Enforce schema consistency and drop invalid records.

4. Governance with Unity Catalog

        Manage table access, metadata, and lineage with Unity Catalog integration.

        Centralized governance across layers.

5. Analytical Modeling with dbt

        Build reusable models for KPIs like average delay, route frequency, etc.

        Generate materialized views and document models for analytics teams.

🧰 Tech Stack Used
1. Databricks – Spark-based transformation and orchestration

2. Azure Data Lake Gen2 – Scalable data storage

3. dbt – SQL modeling, documentation, and testing

4. PySpark – Data transformation logic

5. Unity Catalog – Data governance and access control


