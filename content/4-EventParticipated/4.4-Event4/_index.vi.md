---
title: "Sự kiện 4"
date: 2026-11-07
weight: 4
chapter: false
pre: " <b> 4.4. </b> "
---

# **Sự kiện 4: First Cloud AI Journey – Weekly Meet Up (24/10)**

**Ngày:** Thứ Bảy, ngày 24 tháng 10 năm 2026  
**Thời gian:** 10:30 AM – 12:00 PM (GMT+7)  
**Địa điểm:** Văn phòng AWS Việt Nam, Tầng 26, Bitexco Financial Tower, số 02 Hải Triều, TP. Hồ Chí Minh, Việt Nam.  
**Vai trò:** Người tham dự  
**Video sự kiện:** [Xem trên YouTube](https://www.youtube.com/watch?v=dJiP5890kTg)

### **Mục tiêu sự kiện**

* Tiếp thu kiến thức chuyên sâu và kinh nghiệm thực chiến về Cloud cùng công nghệ AI Agent từ các Tech Lead và kỹ sư trong ngành.
* Khám phá các giải pháp tối ưu kiến trúc hạ tầng đám mây, bảo mật thông tin và kiểm soát chi phí trên AWS.
* Tìm hiểu cách xây dựng và vận hành thực tế các hệ thống Voice AI, Pentest Agent và Agent Framework.
* Giao lưu, kết nối với cộng đồng AWS Student Builder Group và các chuyên gia công nghệ.

### **Diễn giả**

* **Kiet Tran** – Revve AI  
* **Long Huynh** – Styl Solution  
* **Thinh Nguyen** – Styl Solution  
* **Xuan An** – Leader, AWS Student Builder Group HCMUTE  
* **Khoa Kieu** – Tech Lead, ACB  
* **Nghi Danh** – AWS Community Builder  

### **Nội dung nổi bật**

#### **Phiên 1: Hear, Think, Speak – Xây dựng tổng đài Voice-AI tiếng Việt trên AWS**
* Tìm hiểu cách tối ưu pipeline xử lý âm thanh và hội thoại để rút ngắn độ trễ phản hồi xuống còn khoảng **1,8 giây**, mang lại trải nghiệm giao tiếp tự nhiên.
* Theo dõi demo trực tiếp hệ thống Voice AI tiếng Việt phỏng vấn sơ bộ vị trí Cloud Engineer với phản hồi linh hoạt theo ngữ cảnh.

#### **Phiên 2: AWS Resource Access Manager (RAM)**
* Tìm hiểu cách chia sẻ tài nguyên an toàn giữa các tài khoản AWS độc lập trong cùng AWS Organization nhằm giảm chi phí trùng lặp và quản trị mạng tập trung.
* Nắm rõ cách kết hợp IAM policies và Service Control Policies (SCPs) để thiết lập ranh giới quyền hạn và ngăn leo thang đặc quyền trái phép.

#### **Phiên 3: AWS Pentest cùng AWS Continuum / Security Agent**
* Tiếp cận tư duy bảo mật sớm (Shift-Left): tích hợp kiểm tra bảo mật Infrastructure as Code (Terraform) tự động ngay trong quy trình Pull Request trên GitHub/GitLab trước khi merge.
* Tìm hiểu ứng dụng Security Agent mô phỏng hành vi người dùng thật để kiểm thử xâm nhập tự động trên môi trường SIT/UAT trước khi đưa lên production.

#### **Phiên 4: Amazon Bedrock AgentCore**
* Tìm hiểu cách tối ưu chi phí vận hành bằng cách chạy Agent Runtime cô lập trên MicroVM với hạ tầng EC2 Spot.
* Phân biệt kiến trúc bộ nhớ phân tầng: bộ nhớ ngắn hạn đồng bộ trong phiên làm việc và bộ nhớ dài hạn xử lý bất đồng bộ giúp AI Agent duy trì ngữ cảnh người dùng chính xác.

#### **Phiên 5: Kiro Crew – AI Agent 24/7 hỗ trợ Review Code & Giám sát hệ thống**
* Tìm hiểu mô hình AI Agent hoạt động liên tục 24/7 hỗ trợ rà soát mã nguồn, theo dõi sức khỏe hệ thống và tự động trực quan hóa dữ liệu bằng biểu đồ ngay trong khung chat.
* Nắm cơ chế quản lý context và chi phí token: **Auto Compact** tự động nén ngữ cảnh khi đạt 70–90% dung lượng, **Break Down Context** phân tích lượng token theo từng thành phần, kết hợp **Guardrails** chặn lệnh nguy hiểm (xóa hạ tầng, lộ bí mật) và dọn dẹp bộ nhớ cũ.

### **Bài học rút ra & Ứng dụng**

* **Cân bằng Độ trễ – Bảo mật – Chi phí:** Hiểu rõ bài toán đánh đổi giữa độ chính xác và độ trễ thời gian thực ở Voice AI, giá trị của Shift-Left Security trong CI/CD và cách quản lý bộ nhớ, token, EC2 Spot khi vận hành AI Agent liên tục.
* **Phòng thủ nhiều lớp:** Củng cố cách phối hợp IAM, SCP và AWS RAM để giữ nguyên tắc quyền tối thiểu, đồng thời dùng Guardrails kiểm soát hành vi của AI Agent.
* **Ứng dụng thực tiễn:** Nghiên cứu đưa quét bảo mật Terraform vào quy trình Pull Request, áp dụng mô hình bộ nhớ phân tầng và nén ngữ cảnh khi tích hợp LLM API, cũng như thực hành cấu hình AWS Organizations, RAM và SCP.

### **Trải nghiệm sự kiện**

Tham dự buổi Weekly Meet Up ngày 24/10 tại tầng 26 tòa nhà Bitexco mang lại nhiều góc nhìn thực tế quý giá qua 5 phiên chia sẻ chuyên sâu. Phần demo Voice AI tiếng Việt phản hồi ~1,8 giây từ Revve AI đặc biệt ấn tượng, cùng các chia sẻ sát thực tiễn từ Styl Solution, HCMUTE và ACB về quản trị hạ tầng, AgentCore và Kiro Crew. Sự kiện giúp tôi nhận diện rõ khoảng cách giữa lý thuyết và yêu cầu doanh nghiệp, từ đó có định hướng cụ thể hơn cho hành trình phát triển chuyên môn về Cloud và Bảo mật.

### **Hình ảnh sự kiện**

![FCAJ Weekly Meet Up 24/10 - Ảnh 1](/images/4-EventParticipated/event4-1.png) ![FCAJ Weekly Meet Up 24/10 - Ảnh 2](/images/4-EventParticipated/event4-2.png)
