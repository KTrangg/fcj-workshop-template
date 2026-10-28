---
title: "Worklog Tuần 6"
date: 2026-10-23
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

* Tham gia giai đoạn khảo sát và viết proposal của dự án ở vai trò Frontend.
* Chọn cách host frontend trên AWS và hiểu các yêu cầu đi kèm (HTTPS, cache, routing của SPA, URL API).
* Kiểm tra frontend vẫn build và chạy test được sau khi đổi tên SEAL → FCAJ.
* Hiểu luồng chấm điểm bằng AI để giao diện hiển thị đúng từng trạng thái job.
* Chuẩn bị đầu vào cho phần frontend trong proposal (kiến trúc, chi phí).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Dự án được đổi tên thành FCAJ Hackathon (cập nhật README) <br> - So sánh các phương án host frontend trên AWS: giữ container trên EC2 (hiện tại), S3 + CloudFront, AWS Amplify Hosting | 19/10/2026 | 19/10/2026 | [Rename commit](https://github.com/nhatnhm1405/fcaj-hackathon-system/commit/087fb7e9372c8d07b167772c764f96e4b0d51a11); [Amplify Hosting](https://docs.aws.amazon.com/amplify/latest/userguide/welcome.html); [Hosting a static website on S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html) |
| 3 | - Tìm hiểu S3 + CloudFront cho single-page app: bucket private với Origin Access Control, custom error response trả về `index.html`, invalidation cache sau mỗi lần deploy <br> - Ghi chú `VITE_API_URL` phải được truyền trong bước build của CI vì giá trị này bị đóng gói lúc build | 20/10/2026 | 20/10/2026 | [Restrict access to an S3 origin (OAC)](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-restricting-access-to-s3.html); [Custom error responses](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/GeneratingCustomErrorResponses.html); [Invalidating files](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Invalidation.html) |
| 4 | - PR #10 (`feature/technical-rename-fcaj`) được merge vào `main` <br> - Pull `main` mới nhất và kiểm tra frontend trên máy: `npm ci`, `npm run build`, `npm test` (Vitest) | 21/10/2026 | 21/10/2026 | [Merge commit PR #10](https://github.com/nhatnhm1405/fcaj-hackathon-system/commit/93c3cbab5b7e42cc4a19e2e7b6eeaf45913d91b4); [Vitest](https://vitest.dev/guide/) |
| 5 | - Tìm hiểu luồng mục tiêu: Frontend → Backend → RDS/S3 → AI job → SQS → worker → kết quả → Backend → Frontend <br> - Liệt kê các trạng thái job giao diện cần hiển thị (chờ, đang xử lý, thành công, thất bại) và dữ liệu API frontend cần từ Backend 1 | 22/10/2026 | 22/10/2026 | [Amazon SQS](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/welcome.html); [Project repository](https://github.com/nhatnhm1405/fcaj-hackathon-system) |
| 6 | - Chuẩn bị đầu vào chi phí cho frontend (dung lượng S3, số request và data transfer của CloudFront) cho phần ước tính trong proposal <br> - Tổng hợp đề xuất frontend: phương án hosting, các điểm CORS và cookie đăng nhập cần kiểm tra với backend | 23/10/2026 | 23/10/2026 | [AWS Pricing Calculator](https://calculator.aws/); [CloudFront pricing](https://aws.amazon.com/cloudfront/pricing/) |

### Kết quả đạt được tuần 6:

* Chọn S3 + CloudFront làm phương án host frontend và nắm các yêu cầu: bucket private với OAC, fallback `index.html` cho SPA, invalidation cache.
* Hiểu URL API được đóng gói lúc build, nên pipeline CI phải build frontend với `VITE_API_URL` đúng cho từng môi trường.
* Xác nhận frontend build và chạy test được sau khi PR #10 đổi tên được merge.
* Hiểu luồng AI job qua SQS và liệt kê các trạng thái giao diện cùng dữ liệu API cần có.
* Chuẩn bị đầu vào frontend cho proposal và ước tính chi phí, sẵn sàng cho task frontend tiếp theo ở [Issue #12](https://github.com/nhatnhm1405/fcaj-hackathon-system/issues/12).

<!-- [CẦN XÁC NHẬN: kiểm tra thứ 4 (bạn có chạy build/test trên máy không?) và thêm link ghi chú hoặc phần proposal của bạn, rồi xóa dòng này.] -->
