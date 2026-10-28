---
title: "Buildrathon Kickoff: Code the Future with CMC Global"
date: 2026-09-26
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

### Thông tin sự kiện

- **Ngày:** 26/09/2026
- **Giờ bắt đầu:** 09:00 (UTC+7)
- **Địa điểm:** Bitexco Financial Tower, TP. Hồ Chí Minh
- **Vai trò:** Người tham dự
- **Trang sự kiện:** [Buildrathon Kickoff: Code the Future with CMC Global](https://luma.com/8fe9vvps)

### Mục tiêu của sự kiện

- Giới thiệu chương trình Buildrathon và những gì người tham gia cần xây dựng.
- Cho thấy kiến thức cloud và AI được dùng trong sản phẩm thực tế qua một ví dụ từ doanh nghiệp.
- Tạo cơ hội để thực tập sinh FCAJ gặp và hỏi trực tiếp diễn giả.

### Diễn giả

| Thứ tự | Diễn giả | Chức danh | Phần chia sẻ tại sự kiện |
| --- | --- | --- | --- |
| 1 | [Nguyễn Gia Hưng](https://www.linkedin.com/in/jotaguy/) | Head of Solutions Architect, AWS Vietnam and Cambodia | Mở đầu sự kiện, giới thiệu Buildrathon và định hướng của chương trình trong First Cloud AI Journey. |
| 2 | [Bùi Trường Nhật](https://www.linkedin.com/in/dominicbui0000/) | Tech Lead, CMC Global | Trình bày kiến trúc một Slack bot tích hợp AI do CMC Global xây dựng và trả lời câu hỏi. |

Sự kiện đi từ "tại sao" (chương trình và mục tiêu) đến "làm như thế nào" (một hệ thống thực tế của đội kỹ sư), nên phần chia sẻ thứ hai dễ theo dõi hơn.

### Nội dung nổi bật

#### 1. Buildrathon và First Cloud AI Journey

Phần mở đầu giải thích Buildrathon là gì, vì sao nằm trong chương trình thực tập và người tham gia nên hướng tới kết quả như thế nào. Slide cũng trình bày dòng thời gian của AWS tại Việt Nam, từ những khách hàng đầu tiên đến Local Zone, chia thành ba hướng: nhân lực trong nước, hạ tầng và kỹ năng tương lai. Điều này giúp tôi nhìn kỳ thực tập như một phần của kế hoạch dài hạn phát triển kỹ năng cloud và AI tại Việt Nam.

#### 2. Ví dụ thực tế: Market Slack Bot

Phần chia sẻ của CMC Global trình bày một Slack bot được đội phát triển xây dựng từng bước. Thông điệp chính trên slide là mỗi thành phần tồn tại vì nó giải quyết một vấn đề thật mà đội đã gặp.

| Thành phần | Vai trò |
| --- | --- |
| Slack + Socket Mode (WebSocket) | Nhận mention, tin nhắn trực tiếp và tin nhắn trong các thread đang hoạt động. |
| Response gate | Quyết định bot có nên trả lời một tin nhắn hay không trước khi gọi AI. |
| Claude Code | Tạo câu trả lời và trả về dữ liệu có cấu trúc (JSON). |
| `SOUL.md` + Memory | Định nghĩa giọng điệu, phạm vi của bot và lưu ngữ cảnh của từng thread. |
| bot-schedule, Internal API, Cron + database | Chạy các lượt đã lên lịch, job do ứng dụng quản lý và lưu bộ nhớ, job định kỳ. |

#### 3. Xây dựng từng bước

Diễn giả chia sẻ rằng bot bắt đầu từ một nhu cầu duy nhất (phân loại yêu cầu) rồi mở rộng dần. Thành phần mới chỉ được thêm khi xuất hiện nhu cầu thật, thay vì thiết kế mọi thứ ngay từ đầu.

### Bài học rút ra

- Một tính năng AI không chỉ là gọi model: còn cần cách nhận request, quyết định khi nào phản hồi, lưu ngữ cảnh và chạy tác vụ định kỳ.
- Bắt đầu nhỏ và chỉ thêm thành phần khi cần giúp hệ thống dễ hiểu và dễ bảo trì hơn.
- Thấy được kế hoạch dài hạn của AWS tại Việt Nam giúp tôi hiểu rõ hơn ý nghĩa của những kỹ năng đang học trong chương trình.

### Định hướng áp dụng

Dự án của nhóm, FCAJ Hackathon System, cũng có một thành phần AI chấm bài chạy nền. Từ buổi chia sẻ này, tôi muốn áp dụng cho phần Frontend: mỗi phần chỉ làm một việc rõ ràng, cho người dùng thấy yêu cầu của họ đang ở trạng thái nào, và chỉ thêm tính năng khi nhóm thực sự cần.

### Trải nghiệm tham dự

Đây là sự kiện đầu tiên tôi tham gia trong kỳ thực tập. Được nghe Solutions Architect của AWS và Tech Lead của CMC Global trong cùng một buổi sáng giúp tôi nối mục đích của chương trình với cách kỹ sư xây dựng sản phẩm AI thực tế. Sau phần chia sẻ, tôi chụp ảnh cùng diễn giả và các bạn thực tập sinh FCAJ.

### Hình ảnh sự kiện

![Phần mở đầu giới thiệu AWS First Cloud AI Journey.](/images/4-EventParticipated/4.1-Event1/opening-presentation.jpg)

*Phần mở đầu giới thiệu First Cloud AI Journey và Buildrathon.*

![Slide trình bày quá trình đầu tư của AWS tại Việt Nam từ 2015 đến 2026.](/images/4-EventParticipated/4.1-Event1/aws-vietnam-timeline.jpg)

*Dòng thời gian đầu tư của AWS tại Việt Nam: nhân lực, hạ tầng, kỹ năng và nhân tài tương lai.*

![Tech Lead của CMC Global trình bày kiến trúc Market Slack Bot.](/images/4-EventParticipated/4.1-Event1/cmc-global-talk.jpg)

*Phần chia sẻ của CMC Global về việc xây dựng Slack bot tích hợp AI.*

![Cận cảnh slide kiến trúc Market Slack Bot.](/images/4-EventParticipated/4.1-Event1/slack-bot-architecture.jpg)

*Toàn bộ kiến trúc của Market Slack Bot.*

![Chụp ảnh cùng diễn giả và các thực tập sinh FCAJ tại Buildrathon Kickoff.](/images/4-EventParticipated/4.1-Event1/buildrathon-kickoff.jpg)

*Ảnh chụp cùng diễn giả và các bạn thực tập sinh FCAJ sau sự kiện.*
