---
title: "Nhật ký tuần 11"
date: "2025-11-17"
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

* Thực hành xây dựng và quản lý cơ sở dữ liệu quan hệ bằng Amazon RDS  
* Làm quen với công cụ và kịch bản migration CSDL (Lab 43)  
* Xây dựng data lake cơ bản trên AWS với S3, Glue, Athena và QuickSight  
* Học cách tạo và vận hành Amazon DynamoDB, bao gồm sao lưu và migration   

### Các công việc trong tuần:
| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --------- | ------------ | --------------- | ------------------- |
| 1   | - **Lab 05:** Amazon Relational Database Service (Amazon RDS) <br>&emsp;1. Introduction <br>&emsp;2. Prerequisite Steps: <br>&emsp;&emsp;- 2.1 Tạo VPC <br>&emsp;&emsp;- 2.2 Tạo EC2 Security Group <br>&emsp;&emsp;- 2.3 Tạo RDS Security Group <br>&emsp;&emsp;- 2.4 Tạo DB Subnet Group <br>&emsp;3. Tạo EC2 instance <br>&emsp;4. Tạo RDS database instance <br>&emsp;5. Triển khai ứng dụng (Application Deployment) <br>&emsp;6. Backup và Restore <br>&emsp;7. Dọn dẹp tài nguyên | 17/11/2025 | 17/11/2025 | <https://000005.awsstudygroup.com/> |
| 2   | - **Lab 43:** (DB migration & tools) <br>&emsp;01. EC2 Connect RDP Client <br>&emsp;02. EC2 Connect Fleet Manager <br>&emsp;03. SQLSrv Src Config <br>&emsp;04. Oracle connect SrcDB <br>&emsp;05. Oracle config SrcDB <br>&emsp;06. Drop Constraint <br>&emsp;07. MSSQL to Aurora MySQL target config <br>&emsp;08. MSSQL to Aurora MySQL create project <br>&emsp;09. MSSQL to Aurora MySQL schema conversion <br>&emsp;10. Oracle to MySQL schema conversion (phần 1) <br>&emsp;11. Tạo Migration Task và Endpoint <br>&emsp;12. Kiểm tra dữ liệu trên S3 <br>&emsp;13. Tạo Serverless Migration <br>&emsp;14. Tạo Event Notification <br>&emsp;15. Xem Logs <br>&emsp;16. Troubleshoot kịch bản Mem Pressure <br>&emsp;17. Troubleshoot kịch bản Table Error | 18/11/2025 | 18/11/2025 | *Lab 43* |
| 3   | - **Lab 35:** Data Lake on AWS <br>&emsp;1. Giới thiệu khái niệm Data Lake (Big Data) <br>&emsp;2. Preparation Steps <br>&emsp;3. Data Collection and Storage: <br>&emsp;&emsp;- 3.1 Tạo S3 Bucket <br>&emsp;&emsp;- 3.2 Tạo Delivery Stream (Kinesis Firehose hoặc tương đương) <br>&emsp;&emsp;- 3.3 Tạo Sample Data <br>&emsp;4. Tạo Data Catalog: <br>&emsp;&emsp;- 4.1 Tạo AWS Glue Crawler <br>&emsp;&emsp;- 4.2 Kiểm tra dữ liệu/catalog <br>&emsp;5. Data Transformation <br>&emsp;6. Phân tích và trực quan hóa: <br>&emsp;&emsp;- 6.1 Phân tích với Athena <br>&emsp;&emsp;- 6.2 Vẽ biểu đồ với QuickSight <br>&emsp;7. Dọn dẹp tài nguyên | 19/11/2025 | 19/11/2025 | <https://000035.awsstudygroup.com/> |
| 4   | - **Thực hành:** Ôn lại Lab 05 & Lab 35 <br>&emsp;+ Thực hành lại tạo RDS instance và kết nối từ EC2 <br>&emsp;+ Ôn lại các bước Backup và Restore cho RDS <br>&emsp;+ Thực hành lại tạo S3 Bucket, Glue Crawler và chạy truy vấn Athena <br>&emsp;+ Ghi chú so sánh RDS (CSDL quan hệ) và Data Lake (S3 + Glue + Athena) | 20/11/2025 | 20/11/2025 | <https://000005.awsstudygroup.com/>, <https://000035.awsstudygroup.com/> |
| 5 | - **Lab 39:** Học cách tạo và làm việc với Amazon DynamoDB <br>&emsp;1. LHOL: Thực hành phòng thí nghiệm cho Amazon DynamoDB <br>&emsp;2. Khám phá DynamoDB <br>&emsp;3. Khám phá Bảng điều khiển DynamoDB <br>&emsp;4. Sao lưu <br>&emsp;5. Dọn dẹp <br>&emsp;6. LADV: Các mẫu thiết kế nâng cao cho Amazon DynamoDB <br>&emsp;7. LMR: Xây dựng và triển khai ứng dụng không máy chủ toàn cầu với DynamoDB <br>&emsp;8. LEDA: Xây dựng kiến ​​trúc hướng sự kiện không máy chủ với DynamoDB | 21/11/2025 | 21/11/2025 | <https://000039.awsstudygroup.com/> |
### 🏆 Thành tựu tuần 11

* **Amazon RDS cơ bản**
  * Tạo RDS instance và kết nối từ EC2
  * Thực hành triển khai ứng dụng và backup/restore cơ bản

* **Migration cơ sở dữ liệu**
  * Làm quen với công cụ migration (SQL Server/Oracle → Aurora MySQL)
  * Xem log, kiểm tra dữ liệu trên S3 và xử lý một số lỗi mẫu

* **Data Lake trên AWS**
  * Tạo S3 bucket, AWS Glue Crawler và data catalog
  * Truy vấn dữ liệu bằng Athena và xem báo cáo trong QuickSight

* **Amazon DynamoDB**
  * Tạo bảng DynamoDB và nạp dữ liệu mẫu
  * Đọc/ghi dữ liệu qua CLI và Console; xem các tuỳ chọn sao lưu


