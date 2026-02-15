## AWS VPC Networking Lab
Project Overview

This project demonstrates the manual creation of a custom Virtual Private Cloud (VPC) in AWS, including public and private subnets,
internet gateway configuration, route tables, and subnet associations.
The goal was to understand how AWS networking components work together to enable internet connectivity and traffic control.

## Architecture Components
- custom vpc (10.0.0.0/16)
- private subnet 1 (10.0.1.0/24)
- private subnet 2 (10.0.2.0/24)
- public subnet 1 (10.0.3.0/24)
- public subnet 2 (10.0.4.0/24)
- internet gateway
- custom routing tables
- subnet associations with the vpc and internet gateway


## Step 1 – Create Custom VPC
A custom VPC was created with CIDR (classless inter domain routing address) block 10.0.0.0/16.

## Step 2 – Create Public and Private Subnets
-Four subnets were created in different availability zones.
Public subnet for internet-facing resources
Private subnet for internal resources

## Step 3 – Attach Internet Gateway
An Internet Gateway was created and attached to the VPC to allow outbound internet access.

## Step 4 – Configure Route Table
A custom route table was created with a default route:
0.0.0.0/0 → Internet Gateway

## Step 5 – Associate Route Table with Public Subnet
The route table was associated with the public subnet to enable internet connectivity.

## Key Learnings
-Difference between public and private subnets
-Role of Internet Gateway
-Importance of route tables
-How traffic flows within a VPC

