---
title: "Worklog Tuần 3"
date: 2026-10-02
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:

* Kết nối hai VPC bằng VPC Peering và nắm các điều kiện để lưu lượng đi được.
* Kết nối nhiều VPC qua Transit Gateway, hiểu attachment, association và propagation.
* Chọn được loại EC2 instance; hiểu AMI, key pair, snapshot, EBS và instance store.
* Sử dụng User Data, instance metadata và hiểu cách EC2 Auto Scaling giữ ứng dụng luôn sẵn sàng.
* Có cái nhìn tổng quan về các dịch vụ compute và lưu trữ file khác: EFS, FSx, Lightsail và AWS Application Migration Service (MGN).
* Tham dự watch party AWS Cloud and AI Day Hanoi để tìm hiểu cách cloud và AI được ứng dụng thực tế.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - **Lab 19:** chuẩn bị hai VPC, cấu hình Security Group và Network ACL, tạo peering connection <br> - Thêm route ở cả hai phía, bật phân giải DNS giữa hai VPC, kiểm tra bằng private IP, dọn dẹp | 28/09/2026 | 28/09/2026 | [FCJ Lab19](https://000019.awsstudygroup.com/); [VPC peering basics](https://docs.aws.amazon.com/vpc/latest/peering/vpc-peering-basics.html), [Peering DNS](https://docs.aws.amazon.com/vpc/latest/peering/vpc-peering-dns.html) |
| 3 | - Tham dự **AWS Cloud and AI Day Hanoi 2026** qua buổi watch party tại TP.HCM (tầng 26, Bitexco Financial Tower) <br> - Theo dõi keynote truyền trực tiếp từ Hà Nội: ứng dụng cloud và AI tại Việt Nam, đưa AI vào quy trình doanh nghiệp (Techcombank), nền tảng kỹ thuật phía sau dịch vụ cloud (Werner Vogels), kiểm chứng phần mềm phát triển với AI (Katalon) | 29/09/2026 | 29/09/2026 | [Sự kiện 2]({{< relref "/4-EventParticipated/4.2-Event2" >}}); [AWS Cloud and AI Day Hanoi](https://aws.amazon.com/events/cloud-day-hanoi/) |
| 4 | - **Lab 20:** kết nối bốn VPC qua Transit Gateway <br> - Cấu hình attachment, TGW route table, association và propagation; cập nhật route table của VPC <br> - Kiểm tra đường đi bằng Reachability Analyzer rồi dọn dẹp | 30/09/2026 | 30/09/2026 | [FCJ Lab20](https://000020.awsstudygroup.com/); [How Transit Gateway works](https://docs.aws.amazon.com/vpc/latest/tgw/how-transit-gateways-work.html), [Reachability Analyzer](https://docs.aws.amazon.com/vpc/latest/reachability/how-reachability-analyzer-works.html) |
| 5 | - Học về họ và kích thước EC2 instance, AMI, key pair và sao lưu; so sánh Amazon EBS và instance store <br> - Học EC2 User Data và instance metadata | 01/10/2026 | 01/10/2026 | [Compute VM](https://www.youtube.com/watch?v=-t5h4N6vfBs), [AMI / Backup / Key Pair](https://www.youtube.com/watch?v=yAR6QRT3N1k), [EBS](https://www.youtube.com/watch?v=hKr_TfGP7NY), [Instance store](https://www.youtube.com/watch?v=6IHNDJ85aoQ); [EC2 instance types](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-types.html); [User Data](https://www.youtube.com/watch?v=_v_43Wi7zjo), [Metadata](https://www.youtube.com/watch?v=Ew3QRaKJQSA); [EC2 User Data](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/user-data.html) |
| 6 | - Tìm hiểu EC2 Auto Scaling: launch template, desired/min/max capacity và scaling policy <br> - Tổng quan EFS, FSx, Lightsail và AWS MGN; ôn tập Module 02-03 | 02/10/2026 | 02/10/2026 | [EC2 Auto Scaling](https://www.youtube.com/watch?v=bbLcPitXJSY); [Compute services overview](https://www.youtube.com/watch?v=hFVYG8WqfU0); [Amazon EFS](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html), [Amazon Lightsail](https://docs.aws.amazon.com/lightsail/latest/userguide/what-is-amazon-lightsail.html) |

### Kết quả đạt được tuần 3:

* Hoàn thành Lab 19 (VPC Peering), Lab 20 (Transit Gateway) và phần bài giảng EC2 của Module 03.
* Chọn được giữa VPC Peering và Transit Gateway dựa trên số lượng VPC và nhu cầu định tuyến.
* Nắm các thành phần EC2 cần để chạy một backend server: instance type, AMI, key pair, EBS volume, User Data.
* Hiểu cách Auto Scaling và launch template giữ ứng dụng chạy khi một instance gặp sự cố.
* Tham dự AWS Cloud and AI Day Hanoi (Sự kiện 2): AI cần đi kèm kiểm soát quyền truy cập, bằng chứng kiểm thử và trách nhiệm của con người, không chỉ tăng tốc phát triển.
