Azure E-Commerce Data Pipeline

## What This Project Does
Automated cloud data pipeline that ingests e-commerce data from 
Azure Blob Storage into Azure SQL Database using Azure Data Factory.

## Architecture
CSV Files → Azure Blob Storage → Azure Data Factory → Azure SQL Database

## Tables Loaded
- dbo.orders (89,316 rows)
- dbo.payments (89,316 rows)
- dbo.customers (89,316 rows)

## Tech Stack
- Azure Data Factory (ADF)
- Azure Blob Storage
- Azure SQL Database
- SQL (Query Editor)

## Business Insights Generated
- Total revenue by payment type
- Order status distribution
- Top 10 cities by customer count

## Pipeline Details
- 3 Copy Activities running in parallel
- Auto table creation in Azure SQL
- Source: Azure Blob Storage (raw-data container)
- Sink: Azure SQL Database (dbo schema)
