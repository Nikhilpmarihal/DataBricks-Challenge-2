# DataBricks-Challenge-2

🚀 Day 1 – Delta Conversion & Optimization

Databricks 14 Days AI Challenge – Phase 1: Better Data Engineering

📌 Objective

Establish a strong foundation in Lakehouse data engineering by converting raw CSV e-commerce data into Delta Lake format, creating a managed Delta table, simulating the small file problem, and applying optimization techniques to improve storage layout and query performance.

🏗️ Architecture Context

This notebook implements the Bronze Layer of a Medallion Architecture:

Raw CSV  →  Delta Lake (Bronze)  →  Optimized Delta Table

Key platform: Databricks
Storage format: Delta Lake

📂 Dataset

Source: Kaggle – Ecommerce Behavior Data (Oct 2019)

Approximate Size:

~4.2 million rows

~1.1 GB

Columns:

| Column Name   | Description                            |
| ------------- | -------------------------------------- |
| event_time    | Timestamp of event                     |
| event_type    | view, cart, purchase, remove_from_cart |
| product_id    | Product identifier                     |
| category_id   | Category identifier                    |
| category_code | Category hierarchy                     |
| brand         | Product brand                          |
| price         | Product price                          |
| user_id       | User identifier                        |
| user_session  | Session UUID                           |

🛠️ Tools & Technologies

Databricks Community Edition

PySpark

Delta Lake

SQL

🔄 Steps Implemented
1. Load Raw CSV

2. Create Database

3. Write Data as Delta

4. Create Managed Delta Table

5. Simulate Small File Problem

6. Optimize Delta Table

7. Performance Validation

📈 Results

Successfully converted raw CSV into Delta Lake format

Created managed Delta table

Observed increase in number of files after small-file simulation

OPTIMIZE reduced file count and improved query execution time

Validated performance improvement using runtime benchmarking

🎯 Key Learnings

Difference between Parquet and Delta Lake

Impact of small files on performance

How OPTIMIZE compacts files

Importance of measuring performance rather than assuming improvements

Foundations of Lakehouse-based data engineering
