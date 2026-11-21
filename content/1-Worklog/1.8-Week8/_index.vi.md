---
title: "Nhật ký công việc Tuần 8"
date: 2026-11-07
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

# **Nhật ký công việc Tuần 8: Kiểm kê hạ tầng AWS, Aurora Serverless v2 & Bảo mật ứng dụng Web**

## **1. Mục tiêu tuần**

* Rà soát các tài nguyên AWS đang sử dụng trong môi trường phát triển ReLoop.
* Hiểu rõ mối liên kết giữa CloudFront, S3 và API Gateway.
* Nghiên cứu Amazon Aurora Serverless v2 và bài toán tối ưu chi phí cơ sở dữ liệu.
* Tìm hiểu các cơ chế bảo mật và bảo vệ ứng dụng web.

## **2. Lịch trình thực hiện**

| Ngày | Mô tả công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| :--- | :--- | :--- | :--- | :--- |
| **Ngày 1** | Rà soát kiến trúc Serverless và cách tích hợp lưu trữ, cơ sở dữ liệu cùng dịch vụ backend trên AWS | 11/02/2026 | 11/02/2026 | [Modernize Applications on AWS](https://cloudjourney.awsstudygroup.com/4-modernize/) |
| **Ngày 2** | Rà soát danh mục hạ tầng AWS gồm CloudFront distributions, S3 buckets và tài nguyên API Gateway | 11/03/2026 | 11/03/2026 | [CloudFront Distribution Documentation](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html) |
| **Ngày 3** | Thu thập và tổng hợp thông tin tài nguyên AWS cho môi trường phát triển ReLoop | 11/04/2026 | 11/04/2026 | [AWS Management Console Documentation](https://docs.aws.amazon.com/console/) |
| **Ngày 4** | Nghiên cứu Amazon Aurora Serverless v2 và xuất bản bài blog kỹ thuật về tính năng tự động tạm dừng & khởi động lại ([Blog 3](../../3-blogsposted/3.3-blog3/)) | 11/05/2026 | 11/05/2026 | [Aurora Serverless v2 – Automatic Pause and Resume](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/aurora-serverless-v2-auto-pause.html) |
| **Ngày 5** | Tìm hiểu cơ chế bảo vệ ứng dụng web và quan sát hành vi AWS WAF trong quá trình kiểm thử môi trường phát triển | 11/06/2026 | 11/06/2026 | [Securing Applications with AWS WAF](https://cloudjourney.awsstudygroup.com/3-optimize/) |

## **3. Kết quả đạt được**

### **Rà soát hạ tầng AWS**

* Thu thập bảng kiểm kê tài nguyên AWS vào ngày 04/11/2026 tại region `ap-southeast-1`.
* Rà soát CloudFront distributions cùng các origin tương ứng, nhận diện S3 bucket web hosting, bucket ảnh thiết bị và bucket Terraform state.
* Kiểm tra mối liên kết định tuyến giữa CloudFront và API Gateway.

### **Nghiên cứu Cơ sở dữ liệu & Tối ưu chi phí**

* Nghiên cứu Amazon Aurora Serverless v2, cơ chế tự động co giãn capacity và cấu hình 0 ACU (automatic pause & resume) cho workload gián đoạn cùng các giới hạn đi kèm.

### **Nghiên cứu Bảo mật & Kỹ năng thực hành**

* Tìm hiểu cơ chế bảo vệ ứng dụng web và vai trò của AWS WAF trong việc lọc các yêu cầu HTTP độc hại.
* Nâng cao kỹ năng kiểm kê hạ tầng và lập tài liệu kiến trúc.

### **Sản phẩm kỹ thuật**

* Xuất bản bài blog kỹ thuật về Aurora Serverless v2 vào ngày 05/11/2026 và chuẩn hóa thông tin hạ tầng cho các đợt rà soát kiến trúc kế tiếp.

**Minh chứng bài Blog:** [Bài đăng Aurora Serverless v2 trên AWS Study Group (Facebook)](https://www.facebook.com/photo/?fbid=2576398179507823&set=gm.2326664424765183&idorvanity=660548818043427) | [Xem Blog 3](../../3-blogsposted/3.3-blog3/)
