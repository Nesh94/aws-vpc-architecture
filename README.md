# AWS VPC Architecture Project

## Overview
This project demonstrates a custom AWS VPC architecture with public and private
subnet segmentation, controlled internet access via NAT Gateway, and secure
instance management via AWS Systems Manager.

## Architecture Diagram
![VPC Architecture](./diagram/vpc-architecture.png)

## Components
- Custom VPC (10.0.0.0/16)
- 1 Public Subnet, 1 Private Subnet
- Internet Gateway
- NAT Gateway
- Explicit public & private route tables
- Custom Network ACLs (NACLs)

## Configuration Screenshots
See `/screenshots` — includes VPC, subnets, route tables, NAT gateway,
and connectivity tests (SSH failure vs. SSM success).

## Connectivity Verification
See `connectivity-verification-theory.md` for the full write-up on how
traffic flows through this architecture and why access is controlled as designed.
