# amazon-athena-s3-sql-lab
Query and analyze CSV data in Amazon S3 using Amazon Athena and SQL
# Amazon Athena S3 SQL Lab

## Lab Overview

This lab demonstrates how to query and analyze data stored in an Amazon S3 bucket using **Amazon Athena** and **SQL**.

You will learn how to:
- Upload a CSV file to Amazon S3
- Configure Amazon Athena
- Create an external table
- Execute SQL queries for data analysis

---

## Introduction: What is Amazon Athena?

Amazon Athena is a serverless query service offered by Amazon Web Services (AWS) that allows you to analyze data stored in Amazon S3 using standard SQL.

Athena is built on **Presto**, an open-source distributed SQL query engine, and supports data formats such as:
- CSV
- JSON
- ORC
- Avro
- Apache Parquet

Athena operates on a **pay-per-query** pricing model, meaning you only pay for the data scanned by your queries. It automatically scales and integrates with **AWS Glue Data Catalog** for metadata management.

---

## Prerequisites

- AWS Account
- Access to:
  - Amazon S3
  - Amazon Athena
  - AWS Glue
- Basic knowledge of SQL

---

## Repository Contents

| Folder/File | Description |
|------------|-------------|
| `data/` | Sample CSV dataset |
| `athena/` | SQL scripts for table creation and querying |
| `docs/` | Step-by-step lab guide |

---

## Getting Started

Follow the instructions in `docs/lab_guide.md` to complete the lab.
# Amazon Athena Lab Guide

## Step 1: Upload Data to Amazon S3
1. Create an S3 bucket
2. Create a folder named `e.g data, food, transportation`
3. Upload `sales_data.csv` into the folder

---

## Step 2: Configure Amazon Athena
1. Open Amazon Athena in AWS Console
2. Set query result location:
   s3://<your-bucket-name>/athena-results/

---

## Step 3: Create the Athena Table
1. Open the Athena Query Editor
2. Select the default database or create a new one
3. Paste the contents of `create_table.sql`
4. Update the S3 bucket path
5. Run the query

---

## Step 4: Execute SQL Queries
1. Open `queries.sql`
2. Run queries one by one
3. Review the results in the Athena console

---

## License

This project is licensed under the MIT License.
