---
title: "Worklog Tuần 5"
date: 2026-10-16
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:

* Tham gia team FCAJ Hackathon System, thống nhất bài toán, người dùng mục tiêu và mục tiêu của workshop.
* Được cấp quyền vào repository của nhóm và hiểu cách tổ chức của hệ thống SEAL Hackathon hiện có.
* Tham gia đổi tên dự án từ SEAL sang FCAJ (Issue #1).
* Hiểu stack frontend hiện tại cùng cách build và triển khai.
* Học Shared Responsibility Model, IAM role và tối ưu chi phí để chuẩn bị cho thiết kế trên AWS.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Brainstorm cùng nhóm: bài toán, người dùng (ban tổ chức, thí sinh, giám khảo) và mục tiêu workshop <br> - Học Shared Responsibility Model | 12/10/2026 | 12/10/2026 | [Shared Responsibility Model](https://www.youtube.com/watch?v=tsobAlSg19g); [AWS Well-Architected](https://docs.aws.amazon.com/wellarchitected/latest/framework/the-pillars-of-the-framework.html) |
| 3 | - Trưởng nhóm tạo repository dự án từ mã nguồn SEAL; tôi clone về và tìm hiểu cấu trúc: `back-end/seal-api` (Spring Boot), `front-end/seal-web`, `docker-compose.yml`, `Caddyfile`, `docs/` <br> - Học IAM policy và role | 13/10/2026 | 13/10/2026 | [Initial commit](https://github.com/nhatnhm1405/fcaj-hackathon-system/commit/35479425a228928d66fa4c73528955925f44f725); [IAM](https://www.youtube.com/watch?v=N_vlJGAqZxo), [Create IAM Role](https://www.youtube.com/watch?v=pJWANviu8QM) |
| 4 | - Được giao [Issue #1: Rename files, packages](https://github.com/nhatnhm1405/fcaj-hackathon-system/issues/1) (SEAL → FCAJ) cùng trưởng nhóm và Backend 2 <br> - Liệt kê các phần frontend bị ảnh hưởng khi đổi tên (thư mục `seal-web`, tên ứng dụng, nội dung hiển thị) | 14/10/2026 | 14/10/2026 | [Issue #1](https://github.com/nhatnhm1405/fcaj-hackathon-system/issues/1); [Refactor commit](https://github.com/nhatnhm1405/fcaj-hackathon-system/commit/3c0de1e3ee9f053c43bf58a355164f0e1ad039c2) |
| 5 | - Tìm hiểu stack frontend: React 18 + TypeScript + Vite 6, Tailwind CSS 4, MUI / Radix UI, React Router, kiểm thử bằng Vitest và Playwright <br> - Tìm hiểu cách truyền địa chỉ API lúc build (build argument `VITE_API_URL`) và cách Caddy phục vụ bản build trong Docker <br> - Học tối ưu chi phí | 15/10/2026 | 15/10/2026 | [Project repository](https://github.com/nhatnhm1405/fcaj-hackathon-system); [Vite env variables](https://vite.dev/guide/env-and-mode); [Cost Optimization](https://www.youtube.com/watch?v=IY61YlmXQe8) |
| 6 | - Tìm hiểu cách triển khai hiện tại: Docker Compose (MySQL, backend, frontend, Caddy) và workflow GitHub Actions chạy Vitest + JUnit rồi deploy lên EC2 qua SSH <br> - Ghi lại những gì frontend cần khi chuyển lên AWS: hosting tĩnh, HTTPS, URL API theo từng môi trường | 16/10/2026 | 16/10/2026 | [docker-compose.yml](https://github.com/nhatnhm1405/fcaj-hackathon-system/blob/main/docker-compose.yml); [deploy.yml](https://github.com/nhatnhm1405/fcaj-hackathon-system/blob/main/.github/workflows/deploy.yml) |

### Kết quả đạt được tuần 5:

* Tham gia nhóm và thống nhất bài toán, người dùng và mục tiêu workshop.
* Hiểu cấu trúc repository và vai trò từng phần (backend, frontend, Docker Compose, Caddy, docs).
* Tham gia Issue #1 (đổi tên SEAL → FCAJ) và xác định các phần frontend bị ảnh hưởng.
* Nắm stack frontend (React + TypeScript + Vite + Tailwind) và hiểu `VITE_API_URL` được cố định lúc build, nên mỗi môi trường cần một bản build riêng.
* Hiểu pipeline hiện tại (test → deploy lên EC2 bằng Docker Compose) làm điểm xuất phát cho thiết kế trên AWS.
* Củng cố kiến thức về Shared Responsibility Model, IAM role và tối ưu chi phí.

<!-- [CẦN XÁC NHẬN: kiểm tra lại ngày họp nhóm rồi xóa dòng này.] -->
