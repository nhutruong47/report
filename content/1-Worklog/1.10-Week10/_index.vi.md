---
title: "Nhật ký tuần 10"
date: "2025-11-10"
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:

* Thực hành mã hóa dữ liệu lưu trữ (encrypt at rest) với AWS KMS, S3, CloudTrail và Athena  
* Ôn lại IAM Role, các condition key và mẫu kiểm soát truy cập  
* Thực hành cấp quyền cho ứng dụng truy cập AWS (EC2 → S3) bằng IAM Role  
* Tìm hiểu các dịch vụ cơ sở dữ liệu chính trên AWS: RDS, Aurora, Redshift và ElastiCache  

### Các công việc trong tuần:
| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --------- | ------------ | --------------- | ------------------- |
| 1   | - **Lab 33:** Encrypt at rest with AWS KMS <br>&emsp;1. Introduction <br>&emsp;2. Preparation steps: <br>&emsp;&emsp;- 2.1 Tạo Policy và Role <br>&emsp;&emsp;- 2.2 Tạo Group và User <br>&emsp;3. Tạo AWS Key Management Service (KMS) key <br>&emsp;4. Tạo Amazon S3: <br>&emsp;&emsp;- 4.1 Tạo S3 bucket <br>&emsp;&emsp;- 4.2 Upload dữ liệu lên S3 <br>&emsp;5. Tạo AWS CloudTrail và Amazon Athena: <br>&emsp;&emsp;- 5.1 Tạo CloudTrail <br>&emsp;&emsp;- 5.2 Ghi log vào CloudTrail <br>&emsp;&emsp;- 5.3 Tạo Amazon Athena <br>&emsp;&emsp;- 5.4 Truy vấn log bằng Athena <br>&emsp;6. Kiểm tra và chia sẻ dữ liệu mã hoá trên S3 <br>&emsp;7. Dọn dẹp tài nguyên | 10/11/2025 | 10/11/2025 | <https://000033.awsstudygroup.com/> |
| 2   | - **Lab 44:** IAM Role & Condition <br>&emsp;1. Giới thiệu về IAM <br>&emsp;&emsp;- 1.1 Request tới dịch vụ AWS <br>&emsp;&emsp;- 1.2 Xác thực (authenticate) request <br>&emsp;&emsp;- 1.3 Quy trình Assume Role <br>&emsp;2. Tạo IAM Group <br>&emsp;3. Tạo IAM User: <br>&emsp;&emsp;- 3.1 Tạo IAM Users <br>&emsp;&emsp;- 3.2 Kiểm tra quyền (permissions) <br>&emsp;4. Cấu hình Role Condition: <br>&emsp;&emsp;- 4.1 Tạo Admin IAM Role <br>&emsp;&emsp;- 4.2 Cấu hình Switch Role <br>&emsp;&emsp;- 4.3 Hạn chế quyền Role: <br>&emsp;&emsp;&emsp;• 4.3.1 Giới hạn switch role theo IP <br>&emsp;&emsp;&emsp;• 4.3.2 Giới hạn switch role theo thời gian <br>&emsp;5. Dọn dẹp tài nguyên | 11/11/2025 | 11/11/2025 | <https://000044.awsstudygroup.com/> |
| 3   | - **Thực hành:** Ôn lại Lab 33 & Lab 44 <br>&emsp;+ Thực hành tạo và sử dụng KMS key để mã hóa dữ liệu trên S3 <br>&emsp;+ Ôn lại cách dùng CloudTrail và Athena để truy vấn hoạt động KMS/S3 <br>&emsp;+ Thực hành IAM Role với Condition (IP, thời gian) và Switch Role <br>&emsp;+ Ghi chú ngắn về KMS, IAM Role và các condition key | 12/11/2025 | 12/11/2025 | <https://000033.awsstudygroup.com/>, <https://000044.awsstudygroup.com/> |
| 4   | - **Lab 48:** Cấp quyền cho ứng dụng truy cập AWS bằng IAM Role <br>&emsp;1. Chuẩn bị: <br>&emsp;&emsp;- 1.1 Tạo EC2 instance <br>&emsp;&emsp;- 1.2 Tạo S3 bucket <br>&emsp;2. Dùng access key: <br>&emsp;&emsp;- 2.1 Tạo IAM user và access key <br>&emsp;&emsp;- 2.2 Dùng access key để truy cập S3 từ ứng dụng <br>&emsp;3. IAM Role trên EC2: <br>&emsp;&emsp;- 3.1 Tạo IAM Role <br>&emsp;&emsp;- 3.2 Dùng IAM Role trên EC2 thay cho access key dài hạn <br>&emsp;4. Dọn dẹp tài nguyên | 13/11/2025 | 13/11/2025 | <https://000048.awsstudygroup.com/> |
| 5   | - **Module 06:** AWS Database Services <br>&emsp;+ Module 06-01: Database Concepts Review (ôn lại khái niệm DB) <br>&emsp;+ Module 06-02: Amazon RDS & Amazon Aurora <br>&emsp;+ Module 06-03: Amazon Redshift & ElastiCache <br>&emsp;+ Ghi chú sự khác nhau giữa CSDL quan hệ, data warehouse và cache in-memory | 14/11/2025 | 14/11/2025 |  |

### 🏆 **Thành tựu tuần 10**

* **KMS và mã hoá dữ liệu lưu trữ**
  * Tạo và quản lý AWS KMS key
  * Mã hóa dữ liệu trên S3 và kiểm tra truy cập bằng CloudTrail và Athena
  * Kiểm thử chia sẻ dữ liệu mã hóa trên S3 và dọn dẹp tài nguyên lab

* **IAM Role và điều kiện truy cập**
  * Ôn lại các khái niệm IAM: request, authenticate và quy trình assume role
  * Tạo IAM User, Group và Admin Role
  * Áp dụng điều kiện (Condition) để giới hạn switch role theo IP và thời gian

* **Ứng dụng truy cập AWS bằng IAM Role**
  * Tạo EC2 instance và S3 bucket phục vụ cho lab
  * Dùng access key để truy cập S3 rồi thay bằng IAM Role
  * Xác nhận EC2 truy cập S3 an toàn hơn khi dùng Role thay cho access key dài hạn

* **Tổng quan dịch vụ cơ sở dữ liệu**
  * Ôn lại khái niệm cơ bản về cơ sở dữ liệu trên AWS
  * Nắm tổng quan Amazon RDS và Aurora cho cơ sở dữ liệu quan hệ
  * Hiểu vai trò của Redshift (data warehouse) và ElastiCache (cache in-memory)


