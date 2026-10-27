---
title: "Week 4 Worklog"
date: 2026-10-09
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:

* Compare block, file and object storage and choose the right S3 storage class and lifecycle policy.
* Host a static website on Amazon S3 and serve it through Amazon CloudFront without making the bucket public.
* Practise S3 Versioning, moving objects and Cross-Region Replication (CRR).
* Use S3 File Gateway to give a client an SMB file share backed by S3.
* Build a backup plan with AWS Backup and verify that a restore actually works.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Studied block/file/object storage, S3 Access Points, storage classes, lifecycle policies and CORS <br> - Learned disaster recovery strategies and the meaning of RTO / RPO | 10/05/2026 | 10/05/2026 | Module 04: [Storage overview](https://www.youtube.com/watch?v=hsCfP0IxoaM), [S3 & storage classes](https://www.youtube.com/watch?v=_yunukwcAwc), [Static website & CORS](https://www.youtube.com/watch?v=mPBjB6Ltl_Q), [Data transfer & Backup](https://www.youtube.com/watch?v=YXn8Q_Hpsu4) |
| 3 | - **Lab 57 (part 1):** create a bucket, upload website files, enable static website hosting <br> - Configured public access and object permissions as required by the lab, tested the website endpoint | 10/06/2026 | 10/06/2026 | FCJ Lab57: [Create bucket](https://000057.awsstudygroup.com/2-prerequiste/2.1-creates3bucket/), [Static website](https://000057.awsstudygroup.com/3-staticwebsite/), [Block public access](https://000057.awsstudygroup.com/4-blockpublicaccess/), [Test website](https://000057.awsstudygroup.com/6-testwebsite/) |
| 4 | - **Lab 57 (part 2):** turned Block Public Access back on, created a CloudFront distribution with the S3 origin and a bucket policy <br> - Practised Versioning, moving objects and CRR, then cleaned up | 10/07/2026 | 10/07/2026 | FCJ Lab57: [Configure CloudFront](https://000057.awsstudygroup.com/7-cloudfront/7.2-configure_amazon_cloudfront/), [Versioning](https://000057.awsstudygroup.com/8-versioning/), [Replication](https://000057.awsstudygroup.com/10-s3ccr/), [Cleanup](https://000057.awsstudygroup.com/11-cleanup/) |
| 5 | - **Lab 24:** deploy S3 File Gateway on EC2, create an SMB file share, mount it from a Windows client <br> - Checked that files written to the share appear in S3, then cleaned up | 10/08/2026 | 10/08/2026 | [FCJ Lab24](https://000024.awsstudygroup.com/); [Mount file share](https://000024.awsstudygroup.com/2-useawsstoragegw/2.3-mountfileshare/), [Cleanup](https://000024.awsstudygroup.com/3-cleanup/) |
| 6 | - **Lab 13:** deploy the lab infrastructure, create a backup plan, vault and resource assignment <br> - Enabled vault notifications with SNS via AWS CLI, ran an on-demand backup and tested restore, then cleaned up | 10/09/2026 | 10/09/2026 | FCJ Lab13: [Introduction](https://000013.awsstudygroup.com/1-introduce/), [Backup plan](https://000013.awsstudygroup.com/3-createbackupplan/), [Notifications](https://000013.awsstudygroup.com/4-enablenoti/), [Test restore](https://000013.awsstudygroup.com/5-testrestore/), [Cleanup](https://000013.awsstudygroup.com/6-cleanup/) |

### Week 4 Achievements:

* Completed Module 04 theory and Lab 57, Lab 24 and Lab 13.
* Deployed a static website on S3 and distributed it through CloudFront with a private bucket.
* Practised S3 Versioning and Cross-Region Replication and know what each one protects against.
* Built and tested a full backup → notification → restore flow with AWS Backup.
* Finished the AWS foundations phase (Module 01–04) and am ready to join the team project.
