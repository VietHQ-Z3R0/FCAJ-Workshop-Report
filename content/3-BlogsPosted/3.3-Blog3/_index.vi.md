---
title: "Blog 3"
date: 2026-11-05
weight: 3
chapter: false
pre: " <b> 3.3. </b> "
---

# AURORA SERVERLESS V2: TỰ ĐỘNG TẠM DỪNG VÀ KHỞI ĐỘNG LẠI ĐỂ TỐI ƯU CHI PHÍ DATABASE

## Tổng quan

Một số ứng dụng sử dụng database nhiều trong giờ làm việc nhưng có thời gian dài ít hoạt động ngoài khung giờ đó. Với cấu hình database luôn duy trì compute capacity, chi phí có thể không phản ánh sát nhu cầu sử dụng thực tế.

Amazon Aurora Serverless v2 có thể tự động điều chỉnh capacity dựa trên workload. Với các phiên bản Aurora engine được hỗ trợ, dịch vụ còn có thể giảm capacity xuống **0 Aurora Capacity Units (ACUs)** và tự động tạm dừng sau một khoảng thời gian được cấu hình mà không có hoạt động do người dùng khởi tạo. Khi có yêu cầu kết nối mới, database có thể tự động hoạt động trở lại.

## Các điểm chính cần nắm

* Capacity của Aurora Serverless v2 được đo bằng ACUs. Mỗi ACU đại diện cho một tổ hợp tài nguyên xử lý và bộ nhớ.
* Để sử dụng automatic pause, cần cấu hình minimum capacity của cluster bằng **0 ACUs** và thiết lập khoảng thời gian không hoạt động trước khi tạm dừng.
* Khi một instance đủ điều kiện không có kết nối do người dùng khởi tạo trong khoảng thời gian đã cấu hình, instance có thể tự động pause; yêu cầu kết nối tiếp theo có thể kích hoạt quá trình resume.
* Không phát sinh chi phí instance capacity trong thời gian instance ở trạng thái paused. Tuy nhiên, vẫn cần tính đến các khoản phí database khác, chẳng hạn storage, khi ước tính tổng chi phí.
* Automatic pause chỉ khả dụng với các phiên bản engine Aurora PostgreSQL và Aurora MySQL cùng cấu hình được hỗ trợ. Cần kiểm tra compatibility và limitations hiện hành trước khi bật.
* Ứng dụng cần chấp nhận độ trễ trong lúc instance resume. AWS ghi nhận thời gian resume điển hình có thể khoảng 15 giây với một hoặc một số ít kết nối đến.

## Ví dụ sử dụng

Xét một ứng dụng phát triển nội bộ chủ yếu được sử dụng vào buổi sáng và có rất ít lưu lượng vào ban đêm. Khi Aurora Serverless v2 được cấu hình minimum capacity bằng 0 ACUs, database instance đủ điều kiện có thể tự động pause sau khoảng thời gian không hoạt động đã thiết lập. Khi người dùng quay lại và ứng dụng mở kết nối database, instance sẽ resume để tiếp tục xử lý yêu cầu.

Cách triển khai này có thể giảm chi phí compute capacity trong những khoảng thời gian dài không sử dụng mà không cần quản trị viên phải dừng và khởi động database thủ công mỗi ngày. Tính năng phù hợp nhất với workload có thể chấp nhận độ trễ resume và không yêu cầu truy cập database liên tục với độ trễ thấp.

## Những điểm cần lưu ý

Automatic pause không xảy ra chỉ vì ứng dụng không gửi câu lệnh SQL. Các kết nối do người dùng khởi tạo vẫn đang mở có thể ngăn instance pause; một số tính năng hoặc cấu hình cluster cũng có thể ảnh hưởng đến điều kiện này. Cần xác nhận engine version hỗ trợ 0 ACUs, đọc các giới hạn được AWS công bố và kiểm thử cơ chế retry/timeout khi kết nối. Các CloudWatch metrics như `ServerlessDatabaseCapacity` có thể giúp xác minh instance đã giảm về zero capacity hay chưa.

## Hình ảnh

<!-- Thêm sơ đồ Aurora Serverless v2 hoặc ảnh chụp cấu hình minimum capacity và auto-pause tại đây. -->

## Link

<!-- Dán đường dẫn bài đăng Facebook trong AWS Study Group tại đây. -->

## Tài liệu hướng dẫn

* [Scaling về 0 ACUs với automatic pause và resume](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/aurora-serverless-v2-auto-pause.html)
* [Cách Aurora Serverless v2 hoạt động](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/aurora-serverless-v2.how-it-works.html)
