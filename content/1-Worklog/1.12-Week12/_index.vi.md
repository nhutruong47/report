---
title: "Nhật ký tuần 12"
date: "2025-11-24"
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu tuần 12:

* Thực hành xây dựng và xem dữ liệu chi phí/sử dụng trên AWS  
* Làm quen các cách làm việc với AWS: CloudShell, Console, SDK  
* Sử dụng Cloud9 và AWS Glue DataBrew để chuẩn bị và xử lý dữ liệu  
* Thực hành pipeline phân tích dữ liệu end-to-end với Glue, EMR, Athena, Kinesis Data Analytics, QuickSight, Lambda, Redshift  

### Các công việc trong tuần:
| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --------- | ------------ | --------------- | ------------------- |
| 1   | - **Lab 40:** (Cost và Usage Data) <br>&emsp;2.1 Chuẩn bị database (Preparing the database) <br>&emsp;2.2 Xây dựng database (Building a database) <br>&emsp;3.1 Data in the Table <br>&emsp;3.2 Cost <br>&emsp;3.3 Tagging and Cost Allocation <br>&emsp;3.4 Usage <br>&emsp;3.5 Additional Result Query <br>&emsp;4 Clean up resources | 24/11/2025 | 24/11/2025 | <https://000040.awsstudygroup.com/> |
| 2   | - **Lab 60 & Lab 70:** Công cụ AWS và chuẩn bị dữ liệu <br>&emsp;**Lab 60:** CloudShell, Console, SDK <br>&emsp;**Lab 70:** Cloud9, Dataset, S3 và AWS Glue DataBrew (profiling, clean & transform) | 25/11/2025 | 25/11/2025 | <https://000060.awsstudygroup.com/>, <https://000070.awsstudygroup.com/> |
| 3   | - **Thực hành:** Ôn lại Lab 40 & Lab 70 <br>&emsp;+ Thực hành xem lại dữ liệu cost/usage và query trong Lab 40 <br>&emsp;+ Thực hành dùng Cloud9 và S3 để chuẩn bị dữ liệu <br>&emsp;+ Thực hành tạo và chạy job DataBrew để profiling/clean dữ liệu <br>&emsp;+ Ghi chú ngắn về cách các công cụ này hỗ trợ cost & data preparation | 26/11/2025 | 26/11/2025 | <https://000040.awsstudygroup.com/>, <https://000070.awsstudygroup.com/> |
| 4   | - **Lab 72:** Pipeline phân tích dữ liệu end-to-end <br>&emsp;Bước chuẩn bị, ingest & store, catalog dữ liệu <br>&emsp;Biến đổi dữ liệu với Glue (interactive & GUI), DataBrew, EMR <br>&emsp;Phân tích với Athena và Kinesis Data Analytics <br>&emsp;Trực quan hóa với QuickSight, serve với Lambda, warehouse trên Redshift | 27/11/2025 | 27/11/2025 | <https://000072.awsstudygroup.com/> |
| 5   | - **Lab 73 + Thực hành:** Dashboard và ôn lại Lab 72 <br>&emsp;Xây dựng dashboard, cải thiện dashboard, tạo dashboard tương tác <br>&emsp;Thực hành xem lại các phần pipeline trong Lab 72 (Athena, Kinesis Data Analytics, QuickSight, Lambda, Redshift) <br>&emsp;Ghi chú một số best practice khi xây dựng dashboard/báo cáo | 28/11/2025 | 28/11/2025 | <https://000073.awsstudygroup.com/>, <https://000072.awsstudygroup.com/> |

### 🏆 Thành tựu tuần 12

* **Hiểu dữ liệu chi phí và sử dụng**
  * Xây dựng database đơn giản để lưu trữ dữ liệu cost/usage
  * Xem dữ liệu bảng, chi phí, tag và usage cơ bản
  * Chạy một số truy vấn bổ sung và dọn dẹp tài nguyên lab

* **Công cụ AWS và chuẩn bị dữ liệu**
  * Làm quen với CloudShell, Console và SDK để thao tác với AWS
  * Tạo môi trường Cloud9, làm việc với dataset và S3
  * Dùng AWS Glue DataBrew để profiling, làm sạch và biến đổi dữ liệu

* **Pipeline phân tích end-to-end**
  * Nạp, lưu trữ và tạo catalog dữ liệu với Glue
  * Biến đổi dữ liệu bằng Glue (interactive, GUI), DataBrew và EMR
  * Phân tích dữ liệu bằng Athena và Kinesis Data Analytics