---
title: "Nhật ký công việc Tuần 11"
date: 2026-11-23
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

# **Nhật ký công việc Tuần 11: Kiểm chứng tích hợp cuối cùng, Nộp báo cáo & Nghiên cứu mở rộng**

## **1. Mục tiêu tuần**

* Hoàn tất kiểm chứng tích hợp toàn trình trên môi trường AWS của ReLoop.
* Dọn dẹp tài nguyên/ảnh thừa và đối chiếu chi phí AWS thực tế với số credit còn lại.
* Hoàn thiện và nộp báo cáo thực tập cùng trọn bộ tài liệu dự án ReLoop (24–25/11/2026).
* Nghiên cứu các hướng mở rộng kiến trúc và nâng cao bảo mật AWS cho giai đoạn phát triển tiếp theo của ReLoop.

## **2. Lịch trình thực hiện**

| Ngày | Mô tả công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| :--- | :--- | :--- | :--- | :--- |
| **Ngày 1** | Hoàn tất kiểm chứng tích hợp cuối cùng (S3 Presigned URLs, kiểm duyệt Rekognition + Bedrock Guardrail, luồng AI Kimi K3) và dọn sạch ảnh/tài nguyên thừa | 11/23/2026 | 11/23/2026 | [AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/the-pillars-of-the-framework.html) |
| **Ngày 2** | Tổng hợp sơ đồ kiến trúc AWS hoàn chỉnh (`draw.io` + PNG), đối chiếu AWS Billing/Credits và rà soát toàn bộ Worklog, Proposal, Blogs, Events, Workshop, Tự đánh giá & Góp ý | 11/24/2026 | 11/24/2026 | [FCJ Workforce Program](https://cloudjourney.awsstudygroup.com/8-fcjworkforce/) |
| **Ngày 3** | Nộp báo cáo thực tập hoàn chỉnh và bộ tài liệu kỹ thuật dự án ReLoop trên GitHub Pages | 11/25/2026 | 11/25/2026 | [The First Cloud Journey](https://cloudjourney.awsstudygroup.com/) |
| **Ngày 4** | Nghiên cứu hướng mở rộng cho ReLoop: chuyển gửi email Cognito sang Amazon SES (vượt giới hạn mặc định 50 email/ngày) và nâng cấp chat thời gian thực qua API Gateway WebSockets | 11/26/2026 | 11/26/2026 | [Amazon SES Developer Guide](https://docs.aws.amazon.com/ses/latest/dg/Welcome.html) |
| **Ngày 5** | Tìm hiểu tích hợp quét bảo mật Terraform IaC tự động (Shift-Left Security) trong GitHub Actions và kiểm tra trạng thái CloudWatch Logs, Alarm cùng AWS WAF trên môi trường thực tế | 11/27/2026 | 11/27/2026 | [Amazon CloudWatch Alarms](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Alarms.html) |

## **3. Kết quả đạt được**

### **Kiểm chứng cuối cùng & Dọn dẹp tài nguyên**

* Xác minh thông suốt 10 luồng kiến trúc từ CloudFront, WAF, Cognito, API Gateway, Lambda, DynamoDB, S3, Rekognition đến Bedrock Kimi K3.
* Dọn sạch tài nguyên thừa trong mã nguồn và đối chiếu chi phí thực tế nằm gọn trong hạn mức credit AWS.

### **Hoàn thiện & Nộp báo cáo thực tập**

* Hoàn tất xuất bản báo cáo thực tập song ngữ (EN/VI) gồm Worklog 12 tuần, Proposal, 3 bài blog kỹ thuật, 5 sự kiện tham gia, Workshop 12 học phần, Tự đánh giá và Chia sẻ trong mốc 24–25/11/2026.

### **Nghiên cứu hướng mở rộng**

* Ghi nhận các đề xuất mở rộng khả thi cho ReLoop: tích hợp Amazon SES gửi email tùy chỉnh, chat thời gian thực bằng WebSocket thay cho cơ chế polling 5 giây và tự động kiểm tra bảo mật Terraform trong CI/CD.
