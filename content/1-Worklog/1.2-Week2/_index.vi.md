---
title: "Worklog Tuần 2"
date: 2026-09-25
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:

* Hiểu cách chia VPC thành các subnet bằng CIDR và cách route table định tuyến lưu lượng.
* Phân biệt Security Group (stateful) và Network ACL (stateless).
* Dựng VPC có public subnet và private subnet trên hai Availability Zone, kết nối được tới EC2 ở cả hai loại subnet.
* Nắm các phương án kết nối mạng: VPC Peering, Transit Gateway, Site-to-Site VPN, Direct Connect và vai trò của Elastic Load Balancing.
* Cấu hình inbound và outbound endpoint của Route 53 Resolver cho lab Hybrid DNS.
* Tham dự sự kiện Buildrathon Kickoff để tìm hiểu chương trình Buildrathon.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Học VPC, CIDR, subnet, route table, Internet Gateway và NAT Gateway <br> - So sánh Security Group và Network ACL <br> - Tổng quan VPC Peering, Transit Gateway, VPN, Direct Connect và ELB | 21/09/2026 | 21/09/2026 | [Module 02-01](https://www.youtube.com/watch?v=O9Ac_vGHquM), [02-02](https://www.youtube.com/watch?v=BPuD1l2hEQ4), [02-03](https://www.youtube.com/watch?v=CXU8D3kyxIc); [VPC CIDR blocks](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-cidr-blocks.html) |
| 3 | - **Lab 03 (phần 1):** tạo VPC, subnet, route table và Internet Gateway; gán subnet vào route table <br> - Dùng VPC Resource Map để kiểm tra cấu trúc | 22/09/2026 | 22/09/2026 | [FCJ Lab03](https://000003.awsstudygroup.com/); [Module 02 playlist](https://www.youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i); [Subnet sizing](https://docs.aws.amazon.com/vpc/latest/userguide/subnet-sizing.html) |
| 4 | - **Lab 03 (phần 2):** tạo Security Group, chạy EC2 ở public subnet và private subnet <br> - Thêm NAT Gateway cho private subnet ra Internet <br> - Kết nối EC2 private qua EC2 Instance Connect Endpoint | 23/09/2026 | 23/09/2026 | [FCJ Lab03](https://000003.awsstudygroup.com/); [Security Groups](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-security-groups.html), [Network ACLs](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html); [EC2 Instance Connect Endpoint](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/connect-with-ec2-instance-connect-endpoint.html) |
| 5 | - **Lab 10 (phần 1):** triển khai network và RDGW bằng CloudFormation <br> - Dựng AWS Managed Microsoft AD đóng vai DNS on-premises | 24/09/2026 | 24/09/2026 | [FCJ Lab10](https://000010.awsstudygroup.com/); [Launch CloudFormation](https://000010.awsstudygroup.com/2-prerequiste/2.2-launchcloudformation/), [Set up Managed AD](https://000010.awsstudygroup.com/4-setupad/) |
| 6 | - **Lab 10 (phần 2):** tạo outbound endpoint, forwarding rule cho `onprem.example.com` và inbound endpoint <br> - Kiểm tra phân giải DNS, sau đó dọn endpoint, rule, directory và stack | 25/09/2026 | 25/09/2026 | [Outbound queries](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/resolver-forwarding-outbound-queries.html), [Inbound queries](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/resolver-forwarding-inbound-queries.html); [FCJ Lab10 cleanup](https://000010.awsstudygroup.com/6-cleanup/) |
| 7 | - Tham dự **Buildrathon Kickoff: Code the Future with CMC Global** tại Bitexco Financial Tower <br> - Nghe giới thiệu chương trình Buildrathon và bài chia sẻ kỹ thuật về kiến trúc một Slack bot tích hợp AI | 26/09/2026 | 26/09/2026 | [Sự kiện 1]({{< relref "/4-EventParticipated/4.1-Event1" >}}); [Trang sự kiện](https://luma.com/8fe9vvps) |

### Kết quả đạt được tuần 2:

* Hoàn thành lý thuyết Module 02, Lab 03 và Lab 10.
* Tham dự Buildrathon Kickoff (Sự kiện 1) và hiểu mục đích của chương trình Buildrathon.
* Dựng được VPC chạy thực tế với public/private subnet trên hai AZ, Internet Gateway, NAT Gateway và Security Group.
* Quản lý được EC2 private mà không cần gán public IP.
* Cấu hình và kiểm tra Hybrid DNS bằng inbound/outbound endpoint của Route 53 Resolver.
* Dọn dẹp đúng thứ tự (endpoint và rule → directory → CloudFormation stack) để không phát sinh chi phí ẩn.
