---
title: "Week 3 Worklog"
date: 2026-10-02
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:

* Connect two VPCs with VPC Peering and know which conditions must be met for traffic to flow.
* Connect several VPCs through a Transit Gateway and understand attachments, association and propagation.
* Choose an EC2 instance type and understand AMIs, key pairs, snapshots, EBS and instance store.
* Use User Data and instance metadata, and understand how EC2 Auto Scaling keeps an application available.
* Get an overview of other compute and file storage services: EFS, FSx, Lightsail and AWS Application Migration Service (MGN).

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - **Lab 19:** prepare two VPCs, configure Security Groups and Network ACLs, create a peering connection <br> - Added routes on both sides, enabled cross-VPC DNS resolution, tested by private IP, cleaned up | 09/28/2026 | 09/28/2026 | [FCJ Lab19](https://000019.awsstudygroup.com/); [VPC peering basics](https://docs.aws.amazon.com/vpc/latest/peering/vpc-peering-basics.html), [Peering DNS](https://docs.aws.amazon.com/vpc/latest/peering/vpc-peering-dns.html) |
| 3 | - **Lab 20:** connect four VPCs through a Transit Gateway <br> - Configured attachments, TGW route tables, association and propagation; updated VPC route tables <br> - Checked paths with Reachability Analyzer, then cleaned up | 09/29/2026 | 09/29/2026 | [FCJ Lab20](https://000020.awsstudygroup.com/); [How Transit Gateway works](https://docs.aws.amazon.com/vpc/latest/tgw/how-transit-gateways-work.html), [Reachability Analyzer](https://docs.aws.amazon.com/vpc/latest/reachability/how-reachability-analyzer-works.html) |
| 4 | - Studied EC2 instance families and sizing, AMIs, key pairs and backups <br> - Compared Amazon EBS and instance store | 09/30/2026 | 09/30/2026 | [Compute VM](https://www.youtube.com/watch?v=-t5h4N6vfBs), [AMI / Backup / Key Pair](https://www.youtube.com/watch?v=yAR6QRT3N1k), [EBS](https://www.youtube.com/watch?v=hKr_TfGP7NY), [Instance store](https://www.youtube.com/watch?v=6IHNDJ85aoQ); [EC2 instance types](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-types.html) |
| 5 | - Studied EC2 User Data and instance metadata <br> - Learned how EC2 Auto Scaling uses launch templates, desired/min/max capacity and scaling policies | 10/01/2026 | 10/01/2026 | [User Data](https://www.youtube.com/watch?v=_v_43Wi7zjo), [Metadata](https://www.youtube.com/watch?v=Ew3QRaKJQSA), [EC2 Auto Scaling](https://www.youtube.com/watch?v=bbLcPitXJSY); [EC2 User Data](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/user-data.html) |
| 6 | - Overview of EFS, FSx, Lightsail and AWS MGN <br> - Reviewed the week and summarized Modules 02–03 | 10/02/2026 | 10/02/2026 | [Compute services overview](https://www.youtube.com/watch?v=hFVYG8WqfU0); [Amazon EFS](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html), [Amazon Lightsail](https://docs.aws.amazon.com/lightsail/latest/userguide/what-is-amazon-lightsail.html) |

### Week 3 Achievements:

* Completed Lab 19 (VPC Peering) and Lab 20 (Transit Gateway), plus the EC2 lectures of Module 03.
* Can choose between VPC Peering and Transit Gateway based on the number of VPCs and routing needs.
* Understand the EC2 building blocks needed to run a backend server: instance type, AMI, key pair, EBS volume, User Data.
* Understand how Auto Scaling and launch templates keep an application running when an instance fails.
