---
title: "Week 3 Worklog"
date: 2025-09-21
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:

- Successfully build the Hybrid DNS network architecture to integrate the On-Premise DNS system (simulated by AWS Managed Microsoft Active Directory) with Amazon Route 53 DNS service.
- Successfully configure Inbound Endpoint, Outbound Endpoint, and Resolver Rules for bidirectional DNS query routing.

### Tasks to be carried out this week:

| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Preparation and Network Infrastructure Initialization: Review Route 53 Resolver features. Create an EC2 Key Pair (e.g., hr-dns-key) for secure Remote Desktop access. Initialize the CloudFormation Template (e.g., hr-dns-vpc-stack) to deploy the foundational high-availability and secure network infrastructure (VPC, Subnets, Gateways). <br> | 09/15/2025 | 09/15/2025      |
| 3   | - Infrastructure Finalization & RDGW Connection: Monitor CloudFormation stack completion. Reconfigure the VPC Security Group (SG): remove unused ports (3391, 443) and retain ICMP and RDP (3389). Connect to the Remote Desktop Gateway (RDGW) Host by downloading the RDP file, uploading the Key Pair to decrypt, and retrieving the Administrator password. <br>   | 09/16/2025 | 09/16/2025      | 
| 4   | - Route 53 Outbound Endpoint Setup: Create the Route 53 Outbound Endpoint to allow Route 53 Resolver to forward DNS queries externally (to AD). Select the correct VPC and corresponding Security Group. Configure automatic IP addresses in two different Availability Zones. Wait for the endpoint status to become operational. <br> | 09/17/2025 | 09/17/2025      | 
| 5   | - Resolver Rules and Inbound Endpoint Setup: Create a Resolver Rule (type Forward) to forward DNS queries for the specific domain (e.g., onprem.example.com) to the AWS Managed Microsoft AD DNS IP addresses. Create the Route 53 Inbound Endpoint to allow the On-Premise DNS system (AD) to query the Route 53 Resolver, configuring it within private subnets. <br>  | 09/18/2025 | 09/18/2025      | 
| 6   | - Testing and Resource Cleanup: Test results using the nslookup onprem.example.com command on the RDGW host. Verify that the query is resolved via the VPC DNS Resolver IP (VPC CIDR + 2, e.g., 10.0.0.2). Clean up resources: Delete Inbound/Outbound Endpoints. Disassociate the VPC from the Resolver Rule before deleting the Rule. Delete AWS Managed Microsoft Active Directory, and finally, delete the CloudFormation Stacks. <br>                                         | 09/19/2025 | 09/19/2025      | 

### Week 3 Achievements:

- Successfully implemented the Hybrid DNS architecture using Route 53 Resolver.
- Configured the Outbound Endpoint to allow Route 53 Resolver to forward DNS queries externally (to AWS Managed AD).
- Created the Inbound Endpoint enabling the On-Premise DNS system (AD) to query the Route 53 Resolver.
- Resolver Rules (Forward type) were successfully established to route queries for onprem.example.com to the AWS Managed Microsoft AD DNS IP addresses.
- Testing using nslookup on the RDGW host confirmed successful bidirectional DNS resolution.
- Verified that queries were resolved via the VPC DNS Resolver IP (e.g., 10.0.0.2, defined as VPC CIDR + 2).
- Completed comprehensive resource cleanup to prevent unexpected costs.