---
title: "Nhật ký công việc Tuần 9"
date: 2026-11-07
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

# **Nhật ký công việc Tuần 9: Tích hợp Serverless, Kiến trúc hướng sự kiện & Buổi chia sẻ Cloud Mastery**

## **1. Mục tiêu tuần**

* Khám phá các mẫu tích hợp ứng dụng Serverless.
* Hiểu cơ chế xử lý webhook tin cậy và phòng chống trùng lặp sự kiện (idempotency).
* Nghiên cứu dịch vụ hàng đợi, nhắn tin và kiến trúc hướng sự kiện trên AWS.
* Tiếp tục xây dựng ghi chú nghiên cứu và tài liệu chia sẻ kỹ thuật.
* Tham dự buổi chia sẻ **Cloud Mastery – Buổi chia sẻ về Cloud cho sinh viên** tại Văn phòng AWS Việt Nam.

## **2. Lịch trình thực hiện**

| Ngày | Mô tả công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| :--- | :--- | :--- | :--- | :--- |
| **Ngày 1** | Rà soát các mô hình tích hợp API Gateway và Lambda cho ứng dụng Serverless | 11/09/2026 | 11/09/2026 | [Serverless API Development](https://cloudjourney.awsstudygroup.com/4-modernize/) |
| **Ngày 2** | Nghiên cứu tính lũy đẳng (webhook idempotency) và xử lý yêu cầu trùng lặp ở tầng backend | 11/10/2026 | 11/10/2026 | [AWS Lambda Asynchronous Invocation](https://docs.aws.amazon.com/lambda/latest/dg/invocation-async-error-handling.html) |
| **Ngày 3** | Học về nhắn tin bất đồng bộ với Amazon SQS, Amazon SNS và dead-letter queues (DLQ) | 11/11/2026 | 11/11/2026 | [Event Processing with SQS and SNS](https://cloudjourney.awsstudygroup.com/4-modernize/) |
| **Ngày 4** | Tìm hiểu AWS Step Functions và mô hình bù trừ (compensation) cho quy trình nhiều bước | 11/12/2026 | 11/12/2026 | [Getting Started with AWS Step Functions](https://cloudjourney.awsstudygroup.com/4-modernize/) |
| **Ngày 5** | Tổng hợp ghi chú nghiên cứu kỹ thuật và ôn tập các chủ đề kỹ thuật AWS mở rộng | 11/13/2026 | 11/13/2026 | [AWS Cloud Day Developer Lounge – AWS Study Group](https://www.youtube.com/watch?v=62YaE5kac3s) |
| **Ngày 6 (T7)** | **Sự kiện:** Tham dự [Sự kiện 5: Cloud Mastery – Buổi chia sẻ về Cloud cho sinh viên](../../4-eventparticipated/4.5-event5/) tại Văn phòng AWS Việt Nam (Bitexco Financial Tower) | 11/14/2026 | 11/14/2026 | [Báo cáo Sự kiện 5](../../4-eventparticipated/4.5-event5/) |

## **3. Kết quả đạt được**

### **Cơ sở lý thuyết**

* Củng cố hiểu biết về mô hình tích hợp API Gateway – Lambda và vai trò của xử lý bất đồng bộ trong hệ thống phân tán.
* Nắm vững cơ chế idempotency chống xử lý trùng lặp, vai trò của SQS, SNS, DLQ và điều phối luồng đa bước bằng AWS Step Functions.

### **Nghiên cứu kỹ thuật**

* Tìm hiểu cách dùng bản ghi idempotency để kiểm soát yêu cầu lặp lại và mẫu Saga compensation trong luồng giao dịch phân tán.

### **Tài liệu & Hoạt động cộng đồng**

* Hệ thống hóa tài liệu nghiên cứu chia sẻ kiến thức AWS gắn liền với các bài toán kỹ thuật thực tế.
* Tham dự sự kiện **Cloud Mastery** ngày 14/11/2026, tham gia phiên hỏi đáp định hướng nghề nghiệp Cloud và trò chơi Quiz.com ôn tập cuối buổi.
