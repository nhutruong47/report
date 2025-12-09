---
title: "Nhật ký Tuần 3"
date: "2025-09-22"
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu Tuần 3:

* Thiết lập AWS Transit Gateway
* Tạo Transit Gateway Attachments và Route Tables
* Học các khái niệm và dịch vụ Amazon EC2 toàn diện
* Nghiên cứu EC2 Auto Scaling, EFS/FSx, Lightsail, và MGN

### Nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | ---- | ---------- | --------------- | ------------------ |
| 1   | - Giới thiệu AWS Transit Gateway và tổng quan lab <br>&emsp;+ Hiểu các khái niệm về Transit Gateway <br>&emsp;+ So sánh VPC Peering và Transit Gateway <br>&emsp;+ Ôn lại lợi ích và các trường hợp sử dụng phổ biến <br>&emsp;+ Xem lại kiến trúc lab và yêu cầu tiên quyết | 22/09/2025 | 22/09/2025 | <https://000020.awsstudygroup.com/> |
| 2   | - Tạo và cấu hình Transit Gateway <br>&emsp;+ Thiết lập tham số và cấu hình Transit Gateway <br>&emsp;+ Kiểm tra cấu hình Transit Gateway | 23/09/2025 | 23/09/2025 | <https://000020.awsstudygroup.com/>|
| 3   | - Tạo attachments cho Transit Gateway và gắn VPC <br>&emsp;+ Cấu hình tham số attachment <br>&emsp;+ Xác minh trạng thái attachment và kết nối | 24/09/2025 | 24/09/2025 | <https://000020.awsstudygroup.com/>|
| 4   | - Cấu hình route tables cho Transit Gateway và kiểm thử kết nối <br>&emsp;+ Tạo TGW route tables <br>&emsp;+ Thêm routes vào route tables của VPC <br>&emsp;+ Kiểm tra kết nối giữa các VPC <br>&emsp;+ Dọn dẹp tài nguyên kiểm thử | 25/09/2025 | 25/09/2025 | <https://000020.awsstudygroup.com/>|
| 5   | - Module 03-01: Đi sâu Amazon EC2 <br>&emsp;+ Họ/loại instance và cách chọn kích thước <br>&emsp;+ AMI, chiến lược backup và quản lý key pair <br>&emsp;+ EBS vs Instance Store: snapshot và mã hóa <br>&emsp;+ User data và metadata <br>&emsp;+ Tổng quan EC2 Auto Scaling <br>&emsp;+ Tổng quan ngắn: EFS/FSx, Lightsail, MGN | 26/09/2025 | 26/09/2025 | |

### 🏆 **Thành tựu Tuần 3**

**1. Khái niệm & Thiết kế Transit Gateway**

- Nắm vững các khái niệm chính của Transit Gateway và ôn lại kiến trúc lab.
- So sánh Transit Gateway và VPC Peering, thảo luận các trường hợp sử dụng và điểm khác biệt.

**2. Transit Gateway Attachments**

- Tạo attachments cho Transit Gateway và gắn các VPC tương ứng.
- Xác minh trạng thái attachment và kiểm tra kết nối VPC-to-TGW.

**3. Route Tables & Kiểm thử**

- Tạo route tables cho Transit Gateway và thêm routes vào route tables của VPC.
- Thực hiện kiểm tra kết nối giữa các VPC và dọn dẹp tài nguyên kiểm thử.

**4. Kiến thức nền tảng Amazon EC2**

- Ôn lại họ/loại instance EC2 và các tiêu chí chọn kích thước.
- Tìm hiểu AMI, chiến lược backup, quản lý key pair, EBS vs Instance Store, snapshot và mã hoá.
- Xem xét user data/metadata và giới thiệu về EC2 Auto Scaling.
