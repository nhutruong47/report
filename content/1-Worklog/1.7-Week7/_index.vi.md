---
title: "Nhật ký tuần 7"
date: "2025-10-20"
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Hiểu các khái niệm cơ bản và use case chính của Amazon S3  
* Nắm vững khái niệm cơ bản và các trường hợp sử dụng chính của Amazon S3  
* Tạo và cấu hình S3 bucket để lưu trữ website tĩnh  
* Thực hành cấu hình quyền truy cập, tích hợp CloudFront và bật versioning  

### Các công việc trong tuần:
| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --------- | ------------ | --------------- | ------------------- |
| 1   | - **Module:** Bắt đầu với Amazon S3 <br>&emsp;+ Tìm hiểu các khái niệm cơ bản: bucket, object, region, host website tĩnh | 20/10/2025 | 20/10/2025 | <https://000057.awsstudygroup.com/> |
| 2   | - **Lab (Phần 1):** Tạo và chuẩn bị S3 bucket <br>&emsp;2. Tạo S3 bucket <br>&emsp;2.1 Tải source code về máy (load data) <br>&emsp;3. Bật tính năng static website hosting | 21/10/2025 | 21/10/2025 | <https://000057.awsstudygroup.com/> |
| 3   | - **Lab (Phần 2):** Quyền truy cập public và kiểm thử <br>&emsp;4. Cấu hình public access block <br>&emsp;5. Cấu hình object public <br>&emsp;6. Kiểm tra website tĩnh | 22/10/2025 | 22/10/2025 | <https://000057.awsstudygroup.com/> |
| 4   | - **Lab (Phần 3):** CloudFront, versioning và replication <br>&emsp;7. Tăng tốc website tĩnh với CloudFront <br>&emsp;7.1 Chặn toàn bộ public access trực tiếp S3 <br>&emsp;7.2 Cấu hình Amazon CloudFront <br>&emsp;7.3 Kiểm tra truy cập qua CloudFront <br>&emsp;8. Bật bucket versioning <br>&emsp;9. Di chuyển object <br>&emsp;10. Replication object giữa nhiều Region <br>&emsp;11. Dọn dẹp tài nguyên <br>&emsp;12. Ghi chú và best practice | 23/10/2025 | 23/10/2025 | <https://000057.awsstudygroup.com/> |
| 5   | - **Thực hành & Ôn tập:** <br>&emsp;+ Lặp lại toàn bộ quy trình S3 static website (tạo bucket, upload code, host website) <br>&emsp;+ Thực hành lại cấu hình public access, CloudFront và versioning <br>&emsp;+ Xem lại ghi chú và best practice từ lab | 24/10/2025 | 24/10/2025 | <https://000057.awsstudygroup.com/> |

### 🏆 **Thành tựu tuần 7**

* **Nắm cơ bản về Amazon S3**
  * Hiểu Amazon S3 là dịch vụ lưu trữ object trên đám mây
  * Nắm rõ khái niệm bucket, object, region và cách host website tĩnh trên S3

* **Tạo và cấu hình S3 bucket**
  * Tạo S3 bucket để lưu trữ website tĩnh
  * Tải source code về máy và upload nội dung lên S3
  * Bật tính năng static website hosting cho bucket

* **Quản lý public access và kiểm tra website**
  * Cấu hình public access block cho bucket
  * Thiết lập quyền public cho các object cần thiết
  * Mở URL website tĩnh và kiểm tra hoạt động

* **Tích hợp Amazon CloudFront**
  * Chặn truy cập công khai trực tiếp đến S3 bucket
  * Cấu hình CloudFront để phân phối nội dung từ S3
  * Kiểm tra truy cập qua CloudFront để cải thiện tốc độ và bảo mật

* **Sử dụng versioning và replication**
  * Bật bucket versioning để theo dõi các phiên bản object
  * Di chuyển object giữa các bucket/thư mục khi cần
  * Cấu hình cross-Region replication cho object


