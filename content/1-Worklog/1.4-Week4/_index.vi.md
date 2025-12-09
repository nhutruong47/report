---
title: "Nhật ký Tuần 4"
date: "2025-09-29"
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---


### Mục tiêu Tuần 4:

* Triển khai AWS Backup để tự động hóa việc bảo vệ dữ liệu
* Tìm hiểu AWS Storage Gateway cho mô hình lưu trữ hybrid
* Khởi động với các khái niệm cơ bản về Amazon S3 và hosting website tĩnh

### Nhiệm vụ thực hiện trong tuần:

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | ---- | ---------- | --------------- | ------------------ |
| 1   | - Triển khai AWS Backup cho hệ thống <br>&emsp;+ Giới thiệu AWS Backup và SNS <br>&emsp;+ Triển khai hạ tầng <br>&emsp;+ Tạo Backup Plan cho các tài nguyên AWS | 29/09/2025 | 29/09/2025 | <https://000013.awsstudygroup.com/> |
| 2   | - Hoàn thiện cấu hình AWS Backup <br>&emsp;+ Cài đặt thông báo với SNS <br>&emsp;+ Kiểm tra hoạt động khôi phục <br>&emsp;+ Dọn dẹp tài nguyên thử nghiệm | 30/09/2025 | 30/09/2025 | <https://000013.awsstudygroup.com/> |
| 3   | - Làm quen với File Storage Gateway <br>&emsp;+ Chuẩn bị và cài đặt <br>&emsp;+ Tạo Storage Gateway <br>&emsp;+ Tạo File Shares <br>&emsp;+ Mount file share trên máy on-premise <br>&emsp;+ Dọn dẹp tài nguyên | 01/10/2025 | 01/10/2025 | <https://000024.awsstudygroup.com/> |
| 4   | - Khởi động với Amazon S3 (Phần 1) <br>&emsp;+ Giới thiệu Amazon S3 <br>&emsp;+ Chuẩn bị và cài đặt <br>&emsp;+ Kích hoạt tính năng Static website <br>&emsp;+ Cấu hình public access block <br>&emsp;+ Cấu hình public objects <br>&emsp;+ Kiểm tra website | 02/10/2025 | 02/10/2025 | <https://000057.awsstudygroup.com/> |
| 5   | - Tính năng nâng cao Amazon S3 (Phần 2) <br>&emsp;+ Tăng tốc Static website với CloudFront <br>&emsp;+ Bucket Versioning <br>&emsp;+ Di chuyển Objects <br>&emsp;+ Replication Object đa vùng <br>&emsp;+ Ghi chú & Thực hành tốt nhất | 03/10/2025 | 03/10/2025 | <https://000057.awsstudygroup.com/> |



### 🏆 **Thành tựu Tuần 4**

* **Nắm bắt dịch vụ AWS Backup**
  * Hiểu cách AWS Backup cung cấp bảo vệ dữ liệu tập trung
  * Thiết kế và tạo Backup Plan tự động cho các tài nguyên
  * Cấu hình chính sách backup cho EBS, RDS, DynamoDB và EFS
  * Thiết lập hệ thống thông báo qua AWS SNS
  * Thực hiện kiểm tra backup và khôi phục thành công

* **Hiểu cơ bản về Amazon S3 và Static Website Hosting**
  * Nắm các khái niệm về object storage trong S3
  * Cấu hình hosting website tĩnh trên S3
  * Điều chỉnh public access block và quyền truy cập object
  * Sử dụng CloudFront để tăng tốc phân phối nội dung
  * Làm quen với versioning và chính sách vòng đời objects

* **Các tính năng nâng cao của S3**
  * Bật và quản lý bucket versioning để bảo vệ dữ liệu
  * Lên kế hoạch di chuyển objects và cấu hình lifecycle
  * Thiết lập cross-region replication cho mục tiêu khôi phục thảm họa
  * Áp dụng best practices và khuyến nghị bảo mật cho S3
  * Hiểu các storage class và tối ưu chi phí lưu trữ
