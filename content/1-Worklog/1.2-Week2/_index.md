---
title: "Week 2 Worklog"
date: 2026-09-25
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Week 2 Objectives:

* Understand how a VPC is divided into subnets with CIDR blocks and how route tables send traffic.
* Tell the difference between Security Groups (stateful) and Network ACLs (stateless).
* Build a VPC with public and private subnets in two Availability Zones and connect to EC2 instances in both.
* Know the options for connecting networks: VPC Peering, Transit Gateway, Site-to-Site VPN, Direct Connect, and the role of Elastic Load Balancing.
* Configure inbound and outbound Route 53 Resolver endpoints for a Hybrid DNS lab.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Studied VPC, CIDR, subnets, route tables, Internet Gateway and NAT Gateway <br> - Compared Security Groups and Network ACLs <br> - Overview of VPC Peering, Transit Gateway, VPN, Direct Connect and ELB | 09/21/2026 | 09/21/2026 | [Module 02-01](https://www.youtube.com/watch?v=O9Ac_vGHquM), [02-02](https://www.youtube.com/watch?v=BPuD1l2hEQ4), [02-03](https://www.youtube.com/watch?v=CXU8D3kyxIc); [VPC CIDR blocks](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-cidr-blocks.html) |
| 3 | - **Lab 03 (part 1):** create the VPC, subnets, route tables and Internet Gateway; associate subnets with route tables <br> - Used the VPC Resource Map to check the layout | 09/22/2026 | 09/22/2026 | [FCJ Lab03](https://000003.awsstudygroup.com/); [Module 02 playlist](https://www.youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i); [Subnet sizing](https://docs.aws.amazon.com/vpc/latest/userguide/subnet-sizing.html) |
| 4 | - **Lab 03 (part 2):** create Security Groups, launch EC2 in the public and private subnets <br> - Added a NAT Gateway for outbound Internet from the private subnet <br> - Connected to the private instance through an EC2 Instance Connect Endpoint | 09/23/2026 | 09/23/2026 | [FCJ Lab03](https://000003.awsstudygroup.com/); [Security Groups](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-security-groups.html), [Network ACLs](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html); [EC2 Instance Connect Endpoint](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/connect-with-ec2-instance-connect-endpoint.html) |
| 5 | - **Lab 10 (part 1):** deploy the network and RDGW with CloudFormation <br> - Set up AWS Managed Microsoft AD to act as the on-premises DNS | 09/24/2026 | 09/24/2026 | [FCJ Lab10](https://000010.awsstudygroup.com/); [Launch CloudFormation](https://000010.awsstudygroup.com/2-prerequiste/2.2-launchcloudformation/), [Set up Managed AD](https://000010.awsstudygroup.com/4-setupad/) |
| 6 | - **Lab 10 (part 2):** create an outbound endpoint, a forwarding rule for `onprem.example.com` and an inbound endpoint <br> - Tested DNS resolution, then cleaned up endpoints, rules, the directory and the stack | 09/25/2026 | 09/25/2026 | [Outbound queries](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/resolver-forwarding-outbound-queries.html), [Inbound queries](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/resolver-forwarding-inbound-queries.html); [FCJ Lab10 cleanup](https://000010.awsstudygroup.com/6-cleanup/) |

### Week 2 Achievements:

* Completed Module 02 theory, Lab 03 and Lab 10.
* Built a working VPC with public and private subnets across two AZs, Internet Gateway, NAT Gateway and Security Groups.
* Managed a private EC2 instance without giving it a public IP.
* Set up and tested Hybrid DNS with Route 53 Resolver inbound/outbound endpoints.
* Cleaned up in the right order (endpoints and rules → directory → CloudFormation stack) so no hidden cost was left.
