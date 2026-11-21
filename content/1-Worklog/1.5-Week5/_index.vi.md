---
title: "Nhật ký công việc Tuần 5"
date: 2026-11-07
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

# **Nhật ký công việc Tuần 5: Phân tích yêu cầu ReLoop & Lập kế hoạch kiến trúc AWS**

## **1. Mục tiêu tuần**

* Làm rõ các yêu cầu nghiệp vụ và chức năng của dự án ReLoop.
* Xác định các vai trò người dùng chính và luồng xử lý của ứng dụng.
* Nghiên cứu các dịch vụ AWS phù hợp cho lưu trữ frontend, xác thực và xử lý backend.
* Định hình kiến trúc đám mây ban đầu cho hệ thống.

## **2. Lịch trình thực hiện**

| Ngày | Mô tả công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| :--- | :--- | :--- | :--- | :--- |
| **Ngày 1** | Phân tích yêu cầu ReLoop, xác định các đối tượng tham gia chính và mục tiêu ứng dụng | 10/12/2026 | 10/12/2026 | [Modernize Applications on AWS](https://cloudjourney.awsstudygroup.com/4-modernize/) |
| **Ngày 2** | Phác thảo luồng gửi thông tin thiết bị, tải ảnh lên và đăng ký đối tác | 10/13/2026 | 10/13/2026 | [Serverless Application Architecture](https://cloudjourney.awsstudygroup.com/4-modernize/) |
| **Ngày 3** | Nghiên cứu Amazon S3 và CloudFront cho lưu trữ website tĩnh và phân phối hình ảnh | 10/14/2026 | 10/14/2026 | [CloudFront OAC – AWS Documentation](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-restricting-access-to-s3.html) |
| **Ngày 4** | Tìm hiểu Amazon Cognito, API Gateway và AWS Lambda cho xác thực người dùng và xử lý backend | 10/15/2026 | 10/15/2026 | [Serverless Authentication with Amazon Cognito](https://cloudjourney.awsstudygroup.com/4-modernize/) |
| **Ngày 5** | Hệ thống hóa bảng ánh xạ dịch vụ AWS ban đầu và ghi chú kiến trúc ReLoop | 10/16/2026 | 10/16/2026 | [Serverless Backend with Lambda, S3 and DynamoDB](https://cloudjourney.awsstudygroup.com/4-modernize/) |

## **3. Kết quả đạt được**

### **Phân tích yêu cầu**

* Định hình rõ hướng chức năng ban đầu của nền tảng ReLoop.
* Xác định hai nhóm người dùng chính là chủ sở hữu thiết bị và các đối tác đã đăng ký.
* Phác thảo các luồng nghiệp vụ cơ bản cho việc đăng thiết bị và báo giá từ đối tác.

### **Nghiên cứu kiến trúc AWS**

* Nghiên cứu Amazon S3 cho tài nguyên frontend và lưu trữ ảnh thiết bị.
* Tìm hiểu Amazon CloudFront cho phân phối nội dung, Amazon Cognito cho xác thực người dùng.
* Đánh giá API Gateway, AWS Lambda cho tầng xử lý backend và Amazon DynamoDB cho cơ sở dữ liệu.

### **Lập kế hoạch kỹ thuật**

* Nâng cao hiểu biết về kiến trúc ứng dụng Serverless.
* Hoàn thiện ánh xạ ban đầu giữa các chức năng ứng dụng với dịch vụ AWS tương ứng làm cơ sở triển khai.
