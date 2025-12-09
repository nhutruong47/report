---
title: "Week 11 Worklog"
date: "2025-11-17"
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Practice building and managing relational databases with Amazon RDS  
* Explore database migration tools and scenarios (Lab 43)  
* Build a simple data lake on AWS using S3, Glue, Athena, and QuickSight  
* Learn to create and operate Amazon DynamoDB, including backups and migrations    

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 1   | - **Lab 05:** Amazon Relational Database Service (Amazon RDS) <br>&emsp;1. Introduction <br>&emsp;2. Prerequisite steps: <br>&emsp;&emsp;- 2.1 Create a VPC <br>&emsp;&emsp;- 2.2 Create EC2 security group <br>&emsp;&emsp;- 2.3 Create RDS security group <br>&emsp;&emsp;- 2.4 Create DB subnet group <br>&emsp;3. Create EC2 instance <br>&emsp;4. Create RDS database instance <br>&emsp;5. Application deployment <br>&emsp;6. Backup and restore <br>&emsp;7. Clean up resources | 17/11/2025 | 17/11/2025 | <https://000005.awsstudygroup.com/> |
| 2   | - **Lab 43:** (DB migration & tools) <br>&emsp;01. EC2 Connect RDP Client <br>&emsp;02. EC2 Connect Fleet Manager <br>&emsp;03. SQLSrv Src Config <br>&emsp;04. Oracle connect SrcDB <br>&emsp;05. Oracle config SrcDB <br>&emsp;06. Drop Constraint <br>&emsp;07. MSSQL to Aurora MySQL target config <br>&emsp;08. MSSQL to Aurora MySQL create project <br>&emsp;09. MSSQL to Aurora MySQL schema conversion <br>&emsp;10. Oracle to MySQL schema conversion (part 1) <br>&emsp;11. Create migration task and endpoint <br>&emsp;12. Inspect S3 <br>&emsp;13. Create serverless migration <br>&emsp;14. Create event notifications <br>&emsp;15. Check logs <br>&emsp;16. Troubleshoot memory pressure scenario <br>&emsp;17. Troubleshoot table error scenario | 18/11/2025 | 18/11/2025 | *Lab 43* |
| 3   | - **Lab 35:** Data Lake on AWS <br>&emsp;1. Introduce Data Lake (Big Data concept) <br>&emsp;2. Preparation steps <br>&emsp;3. Data collection and storage: <br>&emsp;&emsp;- 3.1 Create S3 bucket <br>&emsp;&emsp;- 3.2 Create Kinesis Firehose delivery stream (or similar) <br>&emsp;&emsp;- 3.3 Create sample data <br>&emsp;4. Create data catalog: <br>&emsp;&emsp;- 4.1 Create AWS Glue crawler <br>&emsp;&emsp;- 4.2 Check data/catalog <br>&emsp;5. Data transformation <br>&emsp;6. Analysis and visualization: <br>&emsp;&emsp;- 6.1 Analyze with Athena <br>&emsp;&emsp;- 6.2 Visualize with QuickSight <br>&emsp;7. Clean up resources | 19/11/2025 | 19/11/2025 | <https://000035.awsstudygroup.com/> |
| 4   | - **Practice:** Review Lab 05 & Lab 35 <br>&emsp;+ Practice again creating RDS instances and connecting from EC2 <br>&emsp;+ Review backup and restore steps for RDS <br>&emsp;+ Practice creating S3 buckets, Glue crawlers, and running Athena queries <br>&emsp;+ Write short notes comparing RDS vs data lake (S3 + Glue + Athena) | 20/11/2025 | 20/11/2025 | <https://000005.awsstudygroup.com/>, <https://000035.awsstudygroup.com/> |
| 5 | - **Lab 39:** Learn to build and work with Amazon DynamoDB <br>&emsp;1. LHOL: Hands-on lab for Amazon DynamoDB <br>&emsp;2. Exploring DynamoDB <br>&emsp;3. Exploring the DynamoDB Console <br>&emsp;4. Backups <br>&emsp;5. Cleanup <br>&emsp;6. LADV: Advanced design patterns for Amazon DynamoDB <br>&emsp;7. LMR: Building and deploying global serverless applications with DynamoDB <br>&emsp;8. LEDA: Building a serverless event-driven architecture with DynamoDB | 2025/11/21 | 2025/11/21 | <https://000039.awsstudygroup.com/> |
### 🏆 Week 11 Achievements

* **Amazon RDS basics**
  * Created an RDS database and connected from an EC2 instance
  * Practiced simple application deployment and backup/restore

* **Database migration**
  * Familiarized with migration tools (SQL Server/Oracle → Aurora MySQL)
  * Reviewed logs, inspected S3 data, and handled sample issues

* **Data Lake on AWS**
  * Created an S3 bucket, AWS Glue crawler, and data catalog
  * Queried data with Athena and viewed basic reports in QuickSight

* **Amazon DynamoDB**
  * Created DynamoDB tables and loaded sample data
  * Read and wrote data via CLI and Console; reviewed backup options
