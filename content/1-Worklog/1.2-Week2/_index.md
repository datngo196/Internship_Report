---
title: "Week 2 Worklog"
date: 2025-09-14
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---


### Week 2 Objectives:

- Delve into critical networking services on the AWS platform.
- Set up and configure a secure Virtual Private Cloud (VPC) environment, including the creation of Public and Private Subnets distributed across multiple Availability Zones (AZs) to ensure a high-availability architecture.
- Master the Internet connectivity mechanism for resources within the VPC, differentiating the roles of the Internet Gateway (IGW) and the NAT Gateway.
- Understand and implement AWS network security layers: Network Access Control Lists (NACLs) at the Subnet level and Security Groups (SGs) at the Elastic Network Interface (ENI) level.
- Research large-scale networking solutions between multiple VPCs, specifically VPC Peering and Transit Gateway.
- Familiarize with the types of Elastic Load Balancers (ELB), focusing on Layer 7 routing capabilities (ALB) and Layer 4 extreme performance (NLB).

### Tasks to be carried out this week:

| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Set up Basic VPC Architecture (Multi-AZ): Create a VPC with a specified CIDR range. Create at least 4 Subnets (Public/Private across 2 different AZs) to ensure a high-availability architecture. Understand the rule of 5 IP addresses reserved by AWS in each Subnet.<br>                                                                                                | 09/08/2025 | 09/08/2025      |
| 3   | - Configure Internet Gateway (IGW): Create and attach an IGW to the VPC. Create a Custom Route Table for Public Subnets. Route Internet traffic (0.0.0.0/0) via the IGW. Associate this Route Table with the Public Subnets. <br> | 09/09/2025 | 09/09/2025      | 
| 4   | - Deploy NAT Gateway: Differentiate NAT Gateway and NAT Instance. Allocate an Elastic IP. Deploy the NAT Gateway in a Public Subnet. Configure the Route Table for Private Subnets, routing Internet traffic (0.0.0.0/0) through the NAT Gateway, allowing outbound access only. <br> | 09/10/2025 | 09/10/2025      | 
| 5   | - Configure Security and Deploy EC2: Study and differentiate Security Groups (stateful, ENI level, ALLOW only) and NACLs (stateless, Subnet level, ALLOW/DENY). Create Security Groups for public and private hosts. Deploy EC2 in Public and Private Subnets. Test connectivity between Subnets and to the Internet (using a Bastion Host/Jump Host concept to SSH into Private EC2). <br>  | 09/11/2025 | 09/11/2025      | 
| 6   | - Connectivity and ELB: Learn about VPC Peering (1:1 connection, no transitive routing support) and Transit Gateway (Central Hub for connecting a large number of VPCs). Explore Elastic Load Balancing (ELB), focusing on ALB (Layer 7, path-based routing) and NLB (Layer 4, extreme performance, static IP support). <br>             | 09/12/2025 | 09/12/2025      | 
### Week 2 Achievements:

- Established a Complete VPC: Successfully created a VPC and divided Subnets into Public/Private tiers across multiple Availability Zones (AZs), ensuring a high-availability architecture.
- Mastered Internet Outbound/Inbound Mechanism: Configured IGW to allow Public Internet access for Public Subnets.
- Secured Internet Access for Private Subnets: Deployed a NAT Gateway (placed in a Public Subnet) and configured the corresponding Route Table, allowing instances in the Private Subnet to access the Internet outbound only.
- Applied Network Layer Security:
  - Differentiated and configured Security Groups (Stateful, applied at ENI) and NACLs (Stateless, applied at Subnet).
  - Successfully deployed EC2 Instances in both Public and Private Subnets and verified internal and external connectivity using jump hosts (Bastion Host)
- Researched Large-Scale Connectivity: Understood the functional difference between VPC Peering (1:1) and the scalable Transit Gateway (Hub-and-spoke).
- Familiarized with Elastic Load Balancer types (ALB for Layer 7 routing, NLB for Layer 4 extreme performance) and core features
