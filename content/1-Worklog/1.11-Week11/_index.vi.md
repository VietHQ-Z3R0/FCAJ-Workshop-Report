---
title: "Nhật ký công việc Tuần 11"
date: 2026-11-07
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

# **Nhật ký công việc Tuần 11: Rà soát tích hợp dự án ReLoop & Kiểm chứng cuối cùng**

**Trạng thái:** *Dự kiến – Sẽ cập nhật theo kết quả thực tế sau khi hoàn thành tuần.*

## **1. Mục tiêu tuần**

* Hoàn tất các đầu việc phát triển và tích hợp còn lại của ReLoop.
* Rà soát luồng tải ảnh, kiểm duyệt nội dung và xử lý AI.
* Kiểm chứng các tương tác giữa các dịch vụ AWS hiện có.
* Chuẩn bị tài liệu dự án cuối kỳ cùng các minh chứng kỹ thuật.
* Hướng tới hoàn thiện dự án vào khoảng 28–30/11/2026.

## **2. Lịch trình thực hiện**

| Ngày | Mô tả công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| :--- | :--- | :--- | :--- | :--- |
| **Ngày 1** | Rà soát các đầu việc còn lại của dự án và xác minh trạng thái triển khai hiện tại của ReLoop | 11/23/2026 | 11/23/2026 | [Modernize Applications on AWS](https://cloudjourney.awsstudygroup.com/4-modernize/) |
| **Ngày 2** | Rà soát luồng tải ảnh lên S3, xử lý Presigned URL và các giới hạn truy cập hình ảnh | 11/24/2026 | 11/24/2026 | [S3 Presigned URLs](https://docs.aws.amazon.com/AmazonS3/latest/userguide/using-presigned-url.html) |
| **Ngày 3** | Rà soát luồng kiểm duyệt ảnh và OCR sử dụng Amazon Rekognition và Bedrock Guardrails | 11/25/2026 | 11/25/2026 | [Amazon Rekognition Moderation](https://docs.aws.amazon.com/rekognition/latest/dg/moderation-api.html) |
| **Ngày 4** | Kiểm tra tính năng tạo tin đăng hỗ trợ AI, xử lý bất đồng bộ và lưu trữ kết quả | 11/26/2026 | 11/26/2026 | [Amazon Bedrock Kimi K3](https://docs.aws.amazon.com/bedrock/latest/userguide/model-card-moonshot-ai-kimi-k3.html) |
| **Ngày 5** | Thực hiện rà soát kiến trúc cuối cùng và chuẩn bị các sản phẩm bàn giao còn lại của dự án | 11/27/2026 | 11/27/2026 | [AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/the-pillars-of-the-framework.html) |

## **3. Kết quả dự kiến**

### **Rà soát tích hợp dự án**

* Hoàn tất kiểm tra các luồng nghiệp vụ chính của ứng dụng ReLoop và mối liên kết giữa frontend, backend, xác thực và lưu trữ.
* Rà soát quy trình kiểm duyệt ảnh, xử lý tin đăng bằng AI và khắc phục các lỗi tích hợp còn tồn đọng.

### **Rà soát Bảo mật & Độ tin cậy**

* Kiểm tra phân quyền IAM, giới hạn truy cập S3, xử lý bất đồng bộ, chống trùng lặp sự kiện, lịch hết hạn và giám sát CloudWatch.

### **Chuẩn bị hoàn thiện dự án**

* Tổng hợp sơ đồ kiến trúc hoàn chỉnh, ảnh chụp minh chứng kỹ thuật và hoàn thiện tài liệu dự án theo mốc 28–30/11/2026.
