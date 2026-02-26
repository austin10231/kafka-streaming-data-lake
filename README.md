# Stock Market Real-Time Kafka Streaming Project

## Overview

This project implements an end-to-end real-time stock market data streaming pipeline using Apache Kafka deployed on AWS EC2. 

Simulated stock tick data is produced in Python and streamed into Kafka topics. A consumer service processes the streaming data and writes structured outputs into Amazon S3. AWS Glue Crawler is used to automatically detect schema and register metadata in the Glue Data Catalog, enabling SQL-based querying via Amazon Athena.

The system demonstrates real-time data ingestion, cloud storage integration, and serverless analytics on AWS.

---

## Architecture

Producer → Kafka (EC2) → Consumer → Amazon S3 → Glue Crawler → Glue Data Catalog → Athena

---

## Tech Stack

- Apache Kafka (EC2)
- Python (kafka-python, boto3)
- Amazon EC2
- Amazon S3
- AWS Glue Crawler
- AWS Glue Data Catalog
- Amazon Athena

---

## Key Highlights

- Built and configured Kafka cluster on AWS EC2
- Implemented Python producer for simulated stock streaming
- Developed Kafka consumer that persists streaming data into S3
- Automated schema discovery using AWS Glue Crawler
- Queried streaming outputs using Athena SQL
- Designed end-to-end cloud-based streaming architecture

---

## Use Case

This architecture reflects real-world streaming data pipelines used in financial analytics, real-time monitoring, and large-scale event processing systems.

## Future Improvements

- Real-time aggregation with Spark Streaming / Flink
- Batch compaction using Parquet format
- CI/CD deployment for infrastructure automation
