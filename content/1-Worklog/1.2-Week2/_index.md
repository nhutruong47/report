---
title: "Week 2 Worklog"
date: "2025-09-15"
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Week 2 Objectives:

* Set up Hybrid DNS with Route 53 Resolver.
* Set up VPC peering

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 1   | - Deploy Amazon EC2 instances and core networking <br>&emsp;+ Create EC2 server and test connectivity <br>&emsp;+ Configure NAT Gateway and use Reachability Analyzer <br>&emsp;+ Create EC2 Instance Connect Endpoint and use Systems Manager Session Manager <br>&emsp;+ Enable CloudWatch monitoring and alerts <br>&emsp;+ Set up Site-to-Site VPN (create VGW, CGW, VPN connection) and configure customer gateway <br>&emsp;+ Modify VPN tunnels, explore alternative VPN setups, and troubleshoot VPN issues | 15/09/2025 | 15/09/2025 | <https://000003.awsstudygroup.com/> |
| 2   | - Build VPN connection using Strongswan and Transit Gateway <br>&emsp;+ Create Transit Gateway and attachments <br>&emsp;+ Configure route tables and customer gateway <br>&emsp;+ Clean up resources after testing <br>&emsp;+ Set up Hybrid DNS with Route 53 Resolver and review Route 53 basics |16/09/2025 | 16/09/2025      | <https://000003.awsstudygroup.com/> <br> <https://000004.awsstudygroup.com/>|
| 3   | - Prepare Amazon Route 53 and related infrastructure <br>&emsp;+ Generate key pairs and initialize CloudFormation templates <br>&emsp;+ Configure security groups and connect to RDGW <br>&emsp;+ Deploy Microsoft AD and set up DNS <br>&emsp;+ Create Route 53 outbound/inbound endpoints and resolver rules <br>&emsp;+ Test DNS resolution and clean up resources | 17/09/2025 | 17/09/2025 | <https://000004.awsstudygroup.com/> |
| 4   | - Set up VPC peering and cross-VPC connectivity <br>&emsp;+ Review prerequisites and initialize CloudFormation templates <br>&emsp;+ Create security groups and EC2 instances as needed <br>&emsp;+ Update Network ACLs, configure route tables and enable cross-peer DNS <br>&emsp;+ Cleanup resources after validation | 18/09/2025 | 18/09/2025 | <https://000019.awsstudygroup.com/> |
| 5   | - Hands-on practices: <br>&emsp;+ Create and configure EC2 server <br>&emsp;+ Test connectivity to EC2 instances <br>&emsp;+ Set up Hybrid DNS with Route 53 Resolver <br>&emsp;+ Explore Amazon Route 53 features <br>&emsp;+ Generate key pairs and validate readiness for Route 53 | 19/09/2025 | 19/09/2025 | |
### 🏆 **Week 2 Achievements**

**1. EC2 Deployment & Core Networking**

- Deployed Amazon EC2 instances and validated connectivity.
- Configured NAT Gateway and used Reachability Analyzer to verify routing.
- Enabled EC2 Instance Connect and Systems Manager Session Manager for access; set up CloudWatch monitoring and alerts.

**2. Site-to-Site VPN**

- Established Site-to-Site VPN components (Virtual Private Gateway, Customer Gateway and VPN connection).
- Modified and tested VPN tunnels; applied troubleshooting steps to resolve connectivity issues.

**3. Transit Gateway & StrongSwan VPN**

- Built VPN using StrongSwan with Transit Gateway; created TGW and attachments.
- Configured route tables and customer gateway settings; validated cross-VPC routing.

**4. Route 53 & Microsoft AD**

- Deployed Microsoft AD and configured Route 53: created inbound/outbound endpoints and resolver rules.
- Tested DNS resolution across environments and verified connectivity.

**5. VPC Peering & Hands-on Practice**

- Implemented VPC peering and configured cross-peer DNS; validated networking and DNS across peered VPCs.
- Completed hands-on tasks: EC2 setup, connectivity testing, Hybrid DNS configuration, and key-pair validation.
