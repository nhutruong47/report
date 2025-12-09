---
title: "Nhật ký tuần 8"
date: "2025-10-27"
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

* Nắm lại mô hình trách nhiệm chia sẻ (Shared Responsibility Model) và các dịch vụ bảo mật/IAM chính của AWS  
* Học và thực hành sử dụng AWS Security Hub cùng các tiêu chuẩn bảo mật  
* Tìm hiểu cách tối ưu chi phí EC2 bằng tự động hóa sử dụng AWS Lambda   

### Các công việc trong tuần:
| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --------- | ------------ | --------------- | ------------------- |
| 1   | - **Module 05:** Các dịch vụ bảo mật và IAM trên AWS <br>&emsp;+ Module 05-01: Shared Responsibility Model <br>&emsp;+ Module 05-02: AWS Identity and Access Management (IAM) <br>&emsp;+ Module 05-03: Amazon Cognito <br>&emsp;+ Module 05-04: AWS Organizations <br>&emsp;+ Module 05-05: AWS Identity Center <br>&emsp;+ Module 05-06: AWS Key Management Service (KMS) <br>&emsp;+ Module 05-07: AWS Security Hub <br>&emsp;+ Module 05-08: Hands-on và tìm hiểu thêm | 27/10/2025 | 27/10/2025 | <https://000018.awsstudygroup.com/> |
| 2   | - **Lab 18 (Phần 1):** Bắt đầu với AWS Security Hub <br>&emsp;+ Xem lại Security Standards và AWS Foundational Security Best Practices <br>&emsp;+ 2. Bật AWS Security Hub | 28/10/2025 | 28/10/2025 | <https://000018.awsstudygroup.com/> |
| 3   | - **Lab 18 (Phần 2):** Đánh giá kết quả từ Security Hub <br>&emsp;+ 3. Xem điểm (score) cho từng nhóm tiêu chí <br>&emsp;+ Xem các findings và hiểu khuyến nghị bảo mật <br>&emsp;+ 4. Dọn dẹp tài nguyên lab Security Hub | 29/10/2025 | 29/10/2025 | <https://000018.awsstudygroup.com/> |
| 4   | - **Lab 22:** Tự động hóa tối ưu chi phí EC2 với Lambda <br>&emsp;+ 1. Hiểu cách Lambda hỗ trợ tối ưu chi phí trên AWS <br>&emsp;+ 2. Chuẩn bị: <br>&emsp;&emsp;- 2.1 Tạo VPC <br>&emsp;&emsp;- 2.2 Tạo Security Group <br>&emsp;&emsp;- 2.3 Tạo EC2 instance <br>&emsp;&emsp;- 2.4 Cấu hình Slack incoming webhooks <br>&emsp;+ 3. Tạo tag cho EC2 instance <br>&emsp;+ 4. Tạo IAM Role cho Lambda <br>&emsp;+ 5. Tạo Lambda functions: <br>&emsp;&emsp;- 5.1 Hàm dừng (stop) instance <br>&emsp;&emsp;- 5.2 Hàm khởi động (start) instance <br>&emsp;+ 6. Kiểm tra kết quả và xác nhận tự động hóa hoạt động <br>&emsp;+ 7. Dọn dẹp tài nguyên | 30/10/2025 | 30/10/2025 | <https://000022.awsstudygroup.com/> |
| 5   | - **Thực hành & Ôn tập:** <br>&emsp;+ Ôn lại các khái niệm chính của Module 05 về bảo mật và IAM <br>&emsp;+ Thực hành lại bật Security Hub và đọc các findings cơ bản <br>&emsp;+ Ôn lại Lambda start/stop EC2 để tối ưu chi phí <br>&emsp;+ Ghi lại một số best practice đơn giản về bảo mật và quản lý chi phí | 31/10/2025 | 31/10/2025 | <https://000018.awsstudygroup.com/>, <https://000022.awsstudygroup.com/> |

### 🏆 **Thành tựu tuần 8**

* **Kiến thức cơ bản về bảo mật và IAM trên AWS**
  * Ôn lại mô hình trách nhiệm chia sẻ giữa AWS và khách hàng
  * Nắm các khái niệm chính của IAM, Cognito, AWS Organizations, Identity Center và KMS

* **Sử dụng AWS Security Hub**
  * Bật AWS Security Hub trong tài khoản
  * Xem các Security Standards và AWS Foundational Security Best Practices
  * Kiểm tra điểm số và các findings bảo mật cho từng nhóm kiểm tra
  * Dọn dẹp tài nguyên lab Security Hub sau khi hoàn thành

* **Tối ưu chi phí EC2 với Lambda**
  * Tạo VPC, security group và EC2 instance phục vụ cho lab
  * Cấu hình Slack incoming webhooks để nhận thông báo
  * Tạo tag cho instance để phục vụ tự động hóa
  * Tạo IAM Role và Lambda functions để dừng/khởi động EC2
  * Kiểm tra hoạt động của Lambda và xác nhận EC2 được điều khiển tự động
  * Dọn dẹp tài nguyên EC2 và Lambda sau khi hoàn tất lab

