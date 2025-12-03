---
title: "Week 10 Worklog"
date: 2025-11-09
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:

- Perform heterogeneous database migrations (SQL Server/Oracle to Aurora MySQL) using AWS SCT and DMS.
- Troubleshoot complex migration scenarios involving schema conversion, memory pressure, and table errors.
- Build a Serverless Data Analytics pipeline using Amazon Kinesis, Glue, and Athena.
- Visualize business intelligence data using Amazon QuickSight.

### Tasks to be carried out this week:

| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Begin Lab 43 by connecting via EC2 Fleet Manager, configuring Source databases (SQL Server/Oracle), handling constraints, and preparing the Target Aurora MySQL environment. <br>  | 11/03/2025 | 11/03/2025      |
| 3   | - Continue Lab 43 by using the Schema Conversion Tool (SCT) to convert schemas, creating Migration Tasks and Endpoints, and launching a Serverless Migration process. <br>    | 11/04/2025 | 11/04/2025      |  |
| 4   | - Finalize Lab 43 by monitoring logs, troubleshooting specific test scenarios (Memory Pressure, Table Errors), validating the migrated data, and cleaning up migration resources. <br> | 11/05/2025 | 11/05/2025      |  |
| 5   | - Start Module 07 (Lab 35) by setting up the ingestion layer: creating an S3 Bucket, configuring a Kinesis Data Firehose Delivery Stream, and generating sample data for analysis. <br>   | 11/06/2025 | 11/06/2025      | |
| 6   | - Complete Lab 35 by configuring an AWS Glue Crawler to catalog data, performing SQL analysis with Amazon Athena, creating visualizations in QuickSight, and cleaning up resources. <br> | 11/07/2025 | 11/07/2025      |  |

### Week 10 Achievements:

- Database Migration:
  - Successfully migrated data from heterogeneous sources (SQL Server, Oracle) to AWS Aurora MySQL.
  - Mastered the AWS Schema Conversion Tool (SCT) and Database Migration Service (DMS).
  - Gained experience in troubleshooting migration failures (memory issues, mapping errors).
- Data Analytics Pipeline:
  - Built a complete serverless data pipeline: Ingestion (Kinesis) -> Storage (S3) -> Catalog (Glue).
  - Analyzed large datasets using SQL queries in Amazon Athena without managing servers.
- Business Intelligence:
  - Connected Amazon QuickSight to the data source to create interactive visual reports.