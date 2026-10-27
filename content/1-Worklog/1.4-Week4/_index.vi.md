---
title: "Worklog Tuần 4"
date: 2026-10-09
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

* So sánh block, file và object storage; chọn đúng S3 storage class và lifecycle policy.
* Host website tĩnh trên Amazon S3 và phân phối qua Amazon CloudFront mà không cần public bucket.
* Thực hành S3 Versioning, di chuyển object và Cross-Region Replication (CRR).
* Dùng S3 File Gateway để cung cấp SMB file share lưu trên S3 cho máy client.
* Tạo backup plan với AWS Backup và kiểm chứng việc restore thực sự hoạt động.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Học block/file/object storage, S3 Access Point, storage class, lifecycle policy và CORS <br> - Tìm hiểu các chiến lược disaster recovery và ý nghĩa RTO / RPO | 05/10/2026 | 05/10/2026 | Module 04: [Storage overview](https://www.youtube.com/watch?v=hsCfP0IxoaM), [S3 & storage classes](https://www.youtube.com/watch?v=_yunukwcAwc), [Static website & CORS](https://www.youtube.com/watch?v=mPBjB6Ltl_Q), [Data transfer & Backup](https://www.youtube.com/watch?v=YXn8Q_Hpsu4) |
| 3 | - **Lab 57 (phần 1):** tạo bucket, upload file website, bật static website hosting <br> - Cấu hình public access và quyền object theo yêu cầu lab, kiểm tra website endpoint | 06/10/2026 | 06/10/2026 | FCJ Lab57: [Create bucket](https://000057.awsstudygroup.com/2-prerequiste/2.1-creates3bucket/), [Static website](https://000057.awsstudygroup.com/3-staticwebsite/), [Block public access](https://000057.awsstudygroup.com/4-blockpublicaccess/), [Test website](https://000057.awsstudygroup.com/6-testwebsite/) |
| 4 | - **Lab 57 (phần 2):** bật lại Block Public Access, tạo CloudFront distribution với S3 origin và bucket policy <br> - Thực hành Versioning, di chuyển object và CRR, sau đó dọn dẹp | 07/10/2026 | 07/10/2026 | FCJ Lab57: [Configure CloudFront](https://000057.awsstudygroup.com/7-cloudfront/7.2-configure_amazon_cloudfront/), [Versioning](https://000057.awsstudygroup.com/8-versioning/), [Replication](https://000057.awsstudygroup.com/10-s3ccr/), [Cleanup](https://000057.awsstudygroup.com/11-cleanup/) |
| 5 | - **Lab 24:** triển khai S3 File Gateway trên EC2, tạo SMB file share, mount từ máy Windows <br> - Kiểm tra file ghi vào share xuất hiện trên S3, sau đó dọn dẹp | 08/10/2026 | 08/10/2026 | [FCJ Lab24](https://000024.awsstudygroup.com/); [Mount file share](https://000024.awsstudygroup.com/2-useawsstoragegw/2.3-mountfileshare/), [Cleanup](https://000024.awsstudygroup.com/3-cleanup/) |
| 6 | - **Lab 13:** triển khai hạ tầng lab, tạo backup plan, vault và resource assignment <br> - Bật thông báo vault qua SNS bằng AWS CLI, chạy on-demand backup và test restore, sau đó dọn dẹp | 09/10/2026 | 09/10/2026 | FCJ Lab13: [Introduction](https://000013.awsstudygroup.com/1-introduce/), [Backup plan](https://000013.awsstudygroup.com/3-createbackupplan/), [Notifications](https://000013.awsstudygroup.com/4-enablenoti/), [Test restore](https://000013.awsstudygroup.com/5-testrestore/), [Cleanup](https://000013.awsstudygroup.com/6-cleanup/) |

### Kết quả đạt được tuần 4:

* Hoàn thành lý thuyết Module 04 cùng Lab 57, Lab 24 và Lab 13.
* Triển khai website tĩnh trên S3 và phân phối qua CloudFront với bucket private.
* Thực hành S3 Versioning, Cross-Region Replication và hiểu mỗi cơ chế bảo vệ trước rủi ro nào.
* Dựng và kiểm tra trọn luồng backup → thông báo → restore với AWS Backup.
* Hoàn tất giai đoạn nền tảng AWS (Module 01–04), sẵn sàng tham gia dự án nhóm.
