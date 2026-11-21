---
title: "Nhật ký công việc Tuần 10"
date: 2026-11-07
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

# **Nhật ký công việc Tuần 10: Rà soát kiến trúc AWS của ReLoop & Kiểm chứng tích hợp dịch vụ**

## **1. Mục tiêu tuần**

* Rà soát tổng thể kiến trúc AWS của hệ thống ReLoop.
* Kiểm chứng các luồng giao tiếp giữa dịch vụ và ranh giới kiến trúc.
* Xem xét chi tiết phần xác thực, lưu trữ, backend và tích hợp AI.
* Nâng cao độ chính xác và tính rõ ràng của tài liệu kiến trúc AWS.

## **2. Lịch trình thực hiện**

| Ngày | Mô tả công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| :--- | :--- | :--- | :--- | :--- |
| **Ngày 1** | Bắt đầu rà soát sơ đồ kiến trúc AWS của ReLoop và xác định các tương tác dịch vụ chính | 11/16/2026 | 11/16/2026 | [Modernize Applications on AWS](https://cloudjourney.awsstudygroup.com/4-modernize/) |
| **Ngày 2** | Rà soát CloudFront origins, S3 Origin Access Control (OAC) và định tuyến yêu cầu qua API Gateway | 11/17/2026 | 11/17/2026 | [CloudFront Origin Access Control](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-restricting-access-to-s3.html) |
| **Ngày 3** | Kiểm tra xác thực Cognito, phân quyền JWT Authorizer và Lambda trigger khởi tạo hồ sơ người dùng | 11/18/2026 | 11/18/2026 | [API Gateway JWT Authorizer](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-jwt-authorizer.html) |
| **Ngày 4** | Rà soát luồng S3 Presigned URL, truy xuất dữ liệu DynamoDB và tích hợp các dịch vụ AI | 11/19/2026 | 11/19/2026 | [S3 Presigned URLs](https://docs.aws.amazon.com/AmazonS3/latest/userguide/using-presigned-url.html) |
| **Ngày 5** | Tinh chỉnh sơ đồ kiến trúc và rà soát kết nối EventBridge, xử lý AI cùng hệ thống giám sát | 11/20/2026 | 11/20/2026 | [Kimi K3 – Amazon Bedrock](https://docs.aws.amazon.com/bedrock/latest/userguide/model-card-moonshot-ai-kimi-k3.html) |

## **3. Kết quả đạt được**

### **Hiểu biết kiến trúc**

* Triển khai rà soát chi tiết kiến trúc ReLoop từ ngày 16/11/2026, làm rõ mối quan hệ giữa CloudFront, API Gateway và backend.
* Kiểm tra luồng xác thực Amazon Cognito – JWT và sự tách biệt giữa bucket web tĩnh với bucket ảnh thiết bị.

### **Phân tích kỹ thuật**

* Rà soát cơ chế Presigned URL cho tải lên/tải xuống trực tiếp trình duyệt – S3 và thao tác đọc/ghi DynamoDB.
* Xem xét vai trò của Amazon Rekognition (kiểm duyệt ảnh, OCR), Amazon Bedrock Kimi K3 & Guardrails, lịch trình EventBridge và giám sát CloudWatch.

### **Tài liệu & Sản phẩm**

* Tinh chỉnh sơ đồ kiến trúc AWS của ReLoop, chuẩn hóa nhãn và chiều luồng giao tiếp dịch vụ để đưa vào tài liệu đồ án cuối kỳ.
