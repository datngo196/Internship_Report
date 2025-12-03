---
title: "Week 8 Worklog"
date: 2025-10-26
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:

- Master advanced IAM concepts: Cross-region access, Role Switching, and Attribute-Based Access Control (ABAC) using Tags.
- Implement restrictive security policies and test IAM User boundaries.
- Deploy comprehensive data security and auditing using KMS, CloudTrail, and Amazon Athena.
- Simulate real-world identity management scenarios with IAM Groups and Admin Roles.

### Tasks to be carried out this week:

| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Complete Lab 28 by creating IAM Policies and Roles, practicing Switch Roles to access resources in different regions (Tokyo/N. Virginia) based on Tag compliance. Perform Lab 30 to create restriction policies and test IAM user limits. <br>  | 10/20/2025 | 10/20/2025      | |
| 3   | - Begin Lab 33 focused on audit and encryption. Create necessary IAM Policies, Roles, Groups, and Users, then initialize a Key Management Service (KMS) key and prepare an S3 bucket for secure data upload. <br>      | 10/21/2025 | 10/21/2025      |  |
| 4   | - Finalize Lab 33 by configuring CloudTrail to log API events, setting up Amazon Athena to query those logs, and testing the sharing of KMS-encrypted data on S3 before cleaning up. <br>  | 10/22/2025 | 10/22/2025      | |
| 5   | - Start Lab 44 to reinforce IAM structural knowledge. Create IAM Groups and Users, and perform detailed permission checks to understand how policies affect user access rights. <br>  | 10/23/2025 | 10/23/2025      |  |
| 6   | - Complete Lab 44 by creating an Admin IAM Role and configuring the Switch Role mechanism for privilege elevation. Review all security concepts learned and perform a full resource cleanup. <br> | 10/24/2025 | 10/24/2025      |  |

### Week 8 Achievements:

- Advanced Identity Management:
  - Successfully implemented Switch Role mechanisms for secure cross-role access.
  - Enforced access controls based on resource tags (ABAC) across different AWS regions.
  - Managed user permissions effectively using Groups and Restriction Policies.
- Security & Compliance:
  - Secured data at rest using AWS KMS encryption.
  - Established an audit trail using AWS CloudTrail and analyzed logs using SQL queries in Amazon Athena.