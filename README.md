# Stock-Market-Analysis

## Project Overview

This project focuses on executing an End-To-End Data Engineering Pipeline on Real-Time Stock Market Data using various technologies such as Apache Kafka, AWS services, and Python. The primary goal is to stream, store, process, and analyze real-time stock market data effectively and efficiently.

## Architecture

The project architecture comprises the following components:

- **Data Ingestion**: Real-time stock market data is ingested using Apache Kafka.
- **Data Storage**: The ingested data is stored in Amazon S3 (Simple Storage Service).
- **Data Processing**: AWS Glue and AWS Athena are used for data processing and querying.
- **Data Visualization**: Processed data can be visualized using various BI tools Quicksight, Tableau, PowerBI.

## Technologies Used

### Programming Language
- **Python**: The primary programming language used for scripting and automation.

### Amazon Web Services (AWS)
- **S3 (Simple Storage Service)**: Used for storing raw and processed data.
- **Athena**: Utilized for querying data stored in S3 using SQL.
- **Glue Crawler**: Automatically catalogs the data in S3 for use in Athena.
- **Glue Catalog**: Metadata repository for data stored in S3, managed by Glue Crawler.
- **EC2 (Elastic Compute Cloud)**: Instances used for running Kafka brokers and other services.

### Other Technologies
- **Apache Kafka**: Distributed event streaming platform used for real-time data ingestion and processing.

## Project Workflow

1. **Setup Kafka Cluster on EC2**:
   - Launch EC2 instances.
   - Install and configure Apache Kafka.

2. **Data Ingestion with Kafka**:
   - Write Python scripts to produce real-time stock market data to Kafka topics.
   - Consume data from Kafka topics for further processing.

3. **Storing Data in S3**:
   - Configure AWS S3 buckets.
   - Write data from Kafka consumers to S3 in a structured format.

4. **Data Processing with AWS Glue**:
   - Set up Glue Crawler to catalog data stored in S3.
   - Use AWS Glue jobs for ETL (Extract, Transform, Load) operations.

5. **Querying Data with Athena**:
   - Use Athena to run SQL queries on the data cataloged by Glue.
   - Analyze and derive insights from the queried data.

