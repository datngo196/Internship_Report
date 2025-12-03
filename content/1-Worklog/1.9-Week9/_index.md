---
title: "Week 9 Worklog"
date: 2025-11-02
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:

- Finalize IAM security best practices by comparing Access Keys vs. IAM Roles.
- Understand AWS Database services (RDS, Aurora, Redshift, ElastiCache) and general database concepts.
- Deploy a 2-tier architecture web application using Amazon EC2 and Amazon RDS.
- Perform database operations including backup, restoration, and connectivity via RDP.

### Tasks to be carried out this week:

| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Complete Lab 44 by implementing conditional switch roles (IP/Time limits). Proceed to Lab 48 to practice generating IAM Access Keys versus using IAM Roles for EC2, understanding why Roles are more secure. <br>  | 10/27/2025 | 10/27/2025      |
| 3   | - Study Module 06 theory videos covering fundamental database concepts (OLTP/OLAP), Amazon RDS & Aurora architectures, and overview of specialized DBs like Redshift and ElastiCache.<br>    | 10/28/2025 | 10/28/2025      |  |
| 4   | - Start Lab 05 (Deploying Web App with RDS) by setting up the network foundation: creating a VPC, configuring EC2 and RDS Security Groups, defining DB Subnet Groups, and launching the EC2 instance. <br> | 10/29/2025 | 10/29/2025      |  |
| 5   | - Continue Lab 05 by provisioning an Amazon RDS database instance, configuring the application on EC2 to connect to the database, and verifying the successful deployment of the web application. <br> | 10/30/2025 | 10/30/2025      |  |
| 6   | - Finalize Lab 05 by performing database backup and restore operations, then clean up all resources. Begin Lab 43 by learning how to connect to Windows instances using an RDP Client. <br> | 10/31/2025 | 10/31/2025      | |

### Week 9 Achievements:

- IAM Security Mastery:
  - Implemented advanced conditional access policies (Date/IP based).
  - Demonstrated the security benefits of using IAM Roles over long-term Access Keys.
- Database Implementation:
  - Grasped the differences between various AWS database offerings (Relational vs. Key-value vs. Warehousing).
  - Successfully deployed a managed Relational Database (RDS) inside a VPC.
- Application Deployment:
  - Connected a web application hosted on EC2 to a backend RDS instance.
  - Performed critical database maintenance tasks like snapshots and restoration.
