---
title: "Event 1"
date: 2026-09-26
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

# Bài thu hoạch “Buildrathon Kickoff: Code the Future with CMC Global”

### Thông Tin Sự Kiện

- **Thời gian:** 09:00 ngày 26/09/2026
- **Địa điểm:** Bitexco Financial Tower, TP. Hồ Chí Minh
- **Vai trò:** Người tham dự
- **Trang sự kiện:** [Buildrathon Kickoff: Code the Future with CMC Global](https://luma.com/8fe9vvps)

### Mục Đích Của Sự Kiện

- Giới thiệu chương trình Buildrathon, mục tiêu và những gì người tham gia cần xây dựng.
- Kết nối kiến thức cloud và AI với ví dụ thực tế từ các kỹ sư trong ngành.
- Tạo cơ hội để thực tập sinh FCAJ trao đổi trực tiếp với diễn giả.

### Danh Sách Diễn Giả

- **Nguyễn Gia Hưng** – Head of Solutions Architect, AWS Vietnam and Cambodia
- **Bùi Trường Nhật** – Tech Lead, CMC Global

### Nội Dung Nổi Bật

#### Giới thiệu chương trình Buildrathon

- Phần mở đầu giải thích mục đích của Buildrathon và vị trí của nó trong First Cloud AI Journey.
- Slide trình bày bối cảnh của AWS tại Việt Nam: đầu tư vào nhân lực, hạ tầng và kỹ năng tương lai.

#### Ví dụ kiến trúc: Slack bot tích hợp AI

Bài chia sẻ kỹ thuật trình bày kiến trúc một Slack bot gồm nhiều thành phần kết nối với nhau:

- **Slack + Socket Mode (WebSocket):** nhận mention, tin nhắn trực tiếp và trả lời trong thread.
- **Response gate:** quyết định bot có nên trả lời và trả lời lúc nào trước khi gọi AI.
- **Xử lý AI (Claude Code):** tạo câu trả lời dưới dạng dữ liệu có cấu trúc.
- **Cấu hình và bộ nhớ:** file định nghĩa giọng điệu, phạm vi của bot và ngữ cảnh của thread.
- **Bộ lập lịch, internal API và database:** chạy tác vụ định kỳ và lưu dữ liệu cho bộ nhớ, job.

### Những Gì Học Được

- Một ứng dụng AI không chỉ là gọi model: còn cần xử lý request, kiểm soát phản hồi, ngữ cảnh và tác vụ định kỳ.
- Chia hệ thống thành các thành phần rõ ràng giúp dễ giải thích, kiểm thử và mở rộng.
- Những sự kiện như vậy giúp tôi nối kiến thức trong các module FCJ với cách kỹ sư xây dựng sản phẩm thật.

### Ứng Dụng Vào Công Việc

- FCAJ Hackathon System của nhóm cũng có thành phần AI (AI judge worker). Ý tưởng "gate" trước khi gọi AI và luồng job rõ ràng hữu ích khi thiết kế cách frontend hiển thị từng trạng thái job.
- Khi vẽ kiến trúc cho dự án, tôi sẽ tách phần nhận request, xử lý và lưu trữ giống cách diễn giả trình bày.

### Trải nghiệm trong event

Đây là sự kiện đầu tiên tôi tham gia trong kỳ thực tập. Nghe Solutions Architect của AWS và Tech Lead của CMC Global chia sẻ giúp tôi hiểu Buildrathon cần gì và một tính năng AI được ghép vào hệ thống thực tế như thế nào. Đây cũng là dịp gặp trực tiếp diễn giả và các bạn thực tập sinh khác.

#### Hình ảnh tham gia sự kiện

![Chụp ảnh cùng diễn giả và các thực tập sinh FCAJ tại Buildrathon Kickoff](/images/4-EventParticipated/4.1-Event1/buildrathon-kickoff.jpg)

*Ảnh chụp cùng diễn giả và các thực tập sinh FCAJ tại Buildrathon Kickoff, Bitexco Financial Tower.*
