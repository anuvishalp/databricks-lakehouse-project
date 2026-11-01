
# End-to-End Databricks Lakehouse Project

## Project Overview
This project demonstrates an end-to-end E-commerce Data Engineering
pipeline using Databricks and the Medallion Architecture.

The pipeline transforms raw customer and event CSV files into
cleaned and business-ready Delta tables.

## Architecture
CSV Files -> Bronze -> Silver -> Gold -> Dashboard

## Technologies Used
- Databricks Free Edition
- Apache Spark / PySpark
- Delta Lake
- Python
- SQL / Data Analytics
- Git and GitHub

## Project Structure
- data/: Sample customer and event CSV files
- notebooks/: Bronze, Silver and Gold notebooks
- screenshots/: Dashboard screenshots

## Pipeline Details

### Bronze Layer
- Reads raw CSV files.
- Adds ingestion timestamps.
- Creates bronze_customers and bronze_events Delta tables.

### Silver Layer
- Removes duplicate records.
- Standardizes email addresses.
- Converts timestamps and transaction amounts.
- Separates invalid records.
- Creates silver_customers and silver_events.

### Gold Layer
- Joins customer and event data.
- Calculates daily revenue.
- Analyzes revenue by country.
- Analyzes membership-tier performance.
- Creates overall business KPIs.

## Gold Tables
- gold_daily_sales_summary
- gold_country_sales
- gold_membership_sales
- gold_overall_kpis

## Dashboard
Executive E-Commerce Sales Dashboard:
- Total Revenue
- Total Purchases
- Average Purchase Value
- Daily Revenue Trend
- Revenue by Country
- Revenue by Membership Tier

## How to Run
1. Create a Databricks workspace.
2. Upload the two CSV files.
3. Run 01_bronze_pipeline.
4. Run 02_silver_pipeline.
5. Run 03_gold_pipeline.
6. Create the dashboard using the Gold tables.

## Dataset
The included CSV files are synthetic sample data created
for educational and demonstration purposes.

## Author
GitHub: https://github.com/anuvishalp
