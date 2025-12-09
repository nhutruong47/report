---
title: "Worklog Tuần 2"
date: "2025-09-15"
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục Tiêu Tuần 2:

* Thiết lập Hybrid DNS với Route 53 Resolver.
* Thiết lập VPC peering

### Các nhiệm vụ được thực hiện trong tuần này:
| Ngày | Nhiệm vụ                                                                                                                                                                                                   | Ngày Bắt Đầu | Ngày Hoàn Thành | Tài Liệu Tham Khảo                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 1   | - Triển khai Amazon EC2 và cấu hình mạng cốt lõi <br>&emsp;+ Tạo EC2 Server và kiểm tra kết nối <br>&emsp;+ Cấu hình NAT Gateway và sử dụng Reachability Analyzer <br>&emsp;+ Tạo EC2 Instance Connect Endpoint và sử dụng Systems Manager Session Manager <br>&emsp;+ Kích hoạt CloudWatch monitoring và alerts <br>&emsp;+ Thiết lập Site-to-Site VPN (Tạo VGW, CGW, kết nối VPN) và cấu hình Customer Gateway <br>&emsp;+ Chỉnh sửa tunnel VPN, thử nghiệm cấu hình VPN thay thế và khắc phục sự cố VPN | 15/09/2025 | 15/09/2025 | <https://000003.awsstudygroup.com/> |
| 2   | - Xây dựng kết nối VPN sử dụng Strongswan và Transit Gateway <br>&emsp;+ Tạo Transit Gateway và attachments <br>&emsp;+ Cấu hình route tables và Customer Gateway <br>&emsp;+ Dọn dẹp tài nguyên sau khi kiểm thử <br>&emsp;+ Thiết lập Hybrid DNS với Route 53 Resolver và ôn lại kiến thức Route 53 |16/09/2025 | 16/09/2025      | <https://000003.awsstudygroup.com/> <br> <https://000004.awsstudygroup.com/>|
| 3   | - Chuẩn bị Route 53 và hạ tầng liên quan <br>&emsp;+ Tạo key pair và khởi tạo CloudFormation templates <br>&emsp;+ Cấu hình security groups và kết nối tới RDGW <br>&emsp;+ Triển khai Microsoft AD và thiết lập DNS <br>&emsp;+ Tạo Route 53 outbound/inbound endpoints và resolver rules <br>&emsp;+ Kiểm tra phân giải DNS và dọn dẹp tài nguyên | 17/09/2025 | 17/09/2025 | <https://000004.awsstudygroup.com/> |
| 4   | - Thiết lập VPC peering và kết nối giữa các VPC <br>&emsp;+ Ôn lại yêu cầu tiên quyết và khởi tạo CloudFormation templates <br>&emsp;+ Tạo security groups và EC2 instances khi cần <br>&emsp;+ Cập nhật Network ACLs, cấu hình route tables và kích hoạt Cross-Peer DNS <br>&emsp;+ Dọn dẹp tài nguyên sau khi kiểm tra | 18/09/2025 | 18/09/2025 | <https://000019.awsstudygroup.com/> |
| 5   | - Bài thực hành: <br>&emsp;+ Tạo và cấu hình EC2 server <br>&emsp;+ Kiểm tra kết nối tới EC2 instances <br>&emsp;+ Thiết lập Hybrid DNS với Route 53 Resolver <br>&emsp;+ Khám phá tính năng của Amazon Route 53 <br>&emsp;+ Tạo key pair và xác thực hệ thống | 19/09/2025 | 19/09/2025 | |
### 🏆 **Thành Tựu Tuần 2**

**1. Triển khai EC2 & mạng cốt lõi**

- Triển khai Amazon EC2 instances và xác nhận kết nối.
- Cấu hình NAT Gateway và sử dụng Reachability Analyzer để kiểm tra định tuyến.
- Kích hoạt EC2 Instance Connect và Systems Manager Session Manager; thiết lập CloudWatch monitoring và cảnh báo.

**2. Kết nối Site-to-Site VPN**

- Thiết lập Virtual Private Gateway, Customer Gateway và kết nối VPN.
- Chỉnh sửa tunnel VPN, thử nghiệm và thực hiện khắc phục sự cố khi cần.

**3. Transit Gateway & StrongSwan VPN**

- Thiết lập VPN bằng StrongSwan với Transit Gateway; tạo TGW và attachments.
- Cấu hình route tables và Customer Gateway; xác minh routing giữa các VPC.

**4. Route 53 & Microsoft AD**

- Triển khai Microsoft AD và cấu hình Route 53: tạo inbound/outbound endpoints và resolver rules.
- Kiểm tra phân giải DNS và xác nhận kết nối giữa các hệ thống.

**5. VPC Peering & Thực hành**

- Thiết lập VPC peering và cấu hình Cross-Peer DNS; xác minh mạng và DNS giữa các VPC.
- Hoàn thành các bài thực hành: tạo EC2, kiểm tra kết nối, cấu hình Hybrid DNS và xác thực key pair.
