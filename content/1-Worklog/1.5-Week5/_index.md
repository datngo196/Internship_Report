---
title: "Week 5 Worklog"
date: 2025-10-05
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

- Master advanced Amazon S3 features (Storage Classes, Lifecycle, Access Points) and Glacier.
- Understand Hybrid Cloud solutions using AWS Storage Gateway and the Snow Family.
- Learn to migrate on-premises Virtual Machines to AWS (VM Import/Export).
- Deploy and manage Windows File Server file systems (FSx) with Multi-AZ configurations.

### Tasks to be carried out this week:

| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Watch Module 04 theory videos covering S3 Storage Classes, Access Points, Static Website Hosting, CORS, and the Snow Family, then start Lab 13 by creating S3 buckets and deploying backup infrastructure. <br>            | 09/29/2025 | 09/29/2025      |
| 3   | - Complete Lab 13 by setting up notifications and testing the restore process, then begin Lab 14 by preparing VMWare Workstation and exporting a virtual machine from on-premises environment.<br>                       | 09/30/2025 | 09/30/2025      |  |
| 4   | - Continue Lab 14 by uploading the VM to AWS, importing it as an AMI, and launching an instance; proceed to Lab 24 to initialize a Storage Gateway service. <br>  | 10/01/2025 | 10/01/2025      |  |
| 5   | - Finalize Lab 24 by creating File Shares and mounting them on a local machine, then start Lab 25 to create SSD and HDD Multi-AZ file systems (FSx for Windows File Server). <br>                              | 10/02/2025 | 10/02/2025      |  |
| 6   | - Complete the setup of Multi-AZ file systems in Lab 25, review all storage concepts learned during the week, and perform a thorough cleanup of all created resources (S3, Gateways, File Systems). <br>  | 10/03/2025 | 10/03/2025      |  |

### Week 5 Achievements:

- Advanced Storage:
  - Deepened understanding of S3 performance, security (CORS/ACL), and archival strategies with Glacier.
  - Explored the AWS Snow Family for offline data transfer.
- Backup & Migration:
  - Successfully configured AWS Backup notifications and tested data restoration.
  - Performed a "Lift and Shift" migration by importing a VMWare virtual machine into AWS EC2.
- Hybrid & File Systems:
  - Bridged on-premise and cloud storage using AWS Storage Gateway.
  - Deployed highly available Windows File Systems (FSx) with Multi-AZ SSD/HDD configurations.
