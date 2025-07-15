# AWS VPC Peering Lab

This lab demonstrates how to establish VPC Peering between two Amazon VPCs to enable private communication between instances.

---

## Overview

Two VPCs were created with non-overlapping CIDR blocks:

- **VPC-A:** `10.0.0.0/16`
- **VPC-B:** `192.168.0.0/16`

Each VPC contains:

- 1 public subnet
- 1 EC2 instance (Amazon Linux 2)

---

## Key Steps

1. Created **VPC-A** and **VPC-B**
2. Created public subnets and attached **Internet Gateways**
3. Launched EC2 instances in each VPC
4. Created and accepted a **VPC Peering Connection**
5. Updated **route tables** to allow cross-VPC routing
6. Configured **security groups** to allow ICMP and SSH between the VPCs
7. Verified connectivity using `ping`

---

## Screenshot of Success

![Ping Test](<img width="822" height="511" alt="ping success" src="https://github.com/user-attachments/assets/600f3c6b-496b-4513-87d8-af86f8f2370d" />)

The ping test confirms that the EC2 instance in VPC-A can reach the EC2 in VPC-B.

---

## Skills Practiced

- VPC Peering
- Route Table configuration
- Security group rules
- Cross-VPC EC2 communication
- Basic network troubleshooting
