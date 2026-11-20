---
title: "Blog 2"
date: 2026-10-28
weight: 2
chapter: false
pre: " <b> 3.2. </b> "
---

# AWS SAVINGS PLANS: TỐI ƯU CHI PHÍ COMPUTE BẰNG CAM KẾT SỬ DỤNG DÀI HẠN

## Tổng quan

Trong nhiều môi trường cloud, workload compute có thể chạy liên tục hoặc có mô hình sử dụng tương đối ổn định. Nếu toàn bộ nhu cầu nền này đều được tính theo mức giá On-Demand, việc tối ưu chi phí sẽ gặp nhiều hạn chế. AWS Savings Plans cung cấp mô hình định giá với mức giá thấp hơn khi người dùng cam kết một lượng compute usage đủ điều kiện ổn định, được tính bằng chi phí mỗi giờ, trong thời hạn một hoặc ba năm.

Savings Plans không yêu cầu ứng dụng phải duy trì cố định một số lượng instance tại mọi thời điểm. Thay vào đó, AWS tự động áp dụng ưu đãi cho mức sử dụng đủ điều kiện, tùy theo loại plan và các điều khoản của plan. Điều này phù hợp với workload có mức sử dụng nền ổn định nhưng vẫn cần khả năng mở rộng khi nhu cầu thay đổi.

## Các điểm chính cần nắm

* Savings Plan dựa trên cam kết chi tiêu cố định theo giờ trong thời hạn một hoặc ba năm.
* **Compute Savings Plans** linh hoạt trên các mức sử dụng Amazon EC2 đủ điều kiện, không phụ thuộc instance family, size, hệ điều hành, tenancy hay AWS Region; đồng thời áp dụng cho mức sử dụng AWS Fargate và AWS Lambda đủ điều kiện.
* **EC2 Instance Savings Plans** cung cấp mức giá ưu đãi cho EC2 trong instance family và AWS Region đã chọn, đồng thời vẫn linh hoạt về size, hệ điều hành và tenancy trong phạm vi của plan.
* AWS tự động áp dụng ưu đãi Savings Plans cho mức sử dụng đủ điều kiện. Phần sử dụng vượt quá mức cam kết sẽ được tính theo mức giá On-Demand tương ứng.
* Các tùy chọn thanh toán bao gồm No Upfront, Partial Upfront và All Upfront, tùy plan và lựa chọn mua được cung cấp.
* AWS Cost Explorer cung cấp đề xuất và báo cáo để đánh giá mức cam kết, utilization và coverage.

## Ví dụ sử dụng

Giả sử một ứng dụng có workload compute chạy xuyên suốt tháng với mức sử dụng nền tương đối ổn định, nhưng đôi khi tăng cao do lưu lượng truy cập đột biến. Nhóm vận hành có thể xem lịch sử sử dụng và đề xuất từ Cost Explorer để ước lượng mức cam kết phù hợp với một phần nhu cầu nền có thể dự đoán. Ứng dụng vẫn có thể mở rộng tài nguyên khi nhu cầu tăng, trong khi phần sử dụng được Savings Plan bao phủ sẽ nhận mức giá ưu đãi tương ứng.

Mức cam kết cần được lựa chọn cẩn thận. Nếu mức sử dụng đủ điều kiện thường xuyên thấp hơn mức đã cam kết, một phần cam kết theo giờ có thể không được sử dụng hết. Vì vậy, cần xem xét lịch sử usage, dự kiến tăng trưởng, thay đổi workload và mức độ linh hoạt của plan trước khi mua.

## Những điểm cần lưu ý

Savings Plans giảm mức giá cho các dịch vụ và loại usage đủ điều kiện, không tự động giảm mọi khoản phí AWS. Trước khi mua, cần xác nhận dịch vụ và usage type nào được plan đã chọn bao phủ, so sánh thời hạn một năm và ba năm, đồng thời đánh giá utilization và coverage dự kiến. Cam kết thận trọng dựa trên nhu cầu nền ổn định thường dễ quản lý hơn việc cam kết theo mức tải đỉnh chỉ xuất hiện trong thời gian ngắn.

## Hình ảnh

<!-- Thêm hình minh họa Savings Plans, ảnh Cost Explorer hoặc sơ đồ so sánh tại đây. -->

## Link

<!-- Dán đường dẫn bài đăng Facebook trong AWS Study Group tại đây. -->

## Tài liệu hướng dẫn

* [Savings Plans là gì?](https://docs.aws.amazon.com/savingsplans/latest/userguide/what-is-savings-plans.html)
* [Câu hỏi thường gặp về Savings Plans](https://aws.amazon.com/savingsplans/faqs/)
