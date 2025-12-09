---
title: "Bản đề xuất"
date: "2025-09-09"
weight: 2
chapter: false
pre: " <b> 2. </b> "
---
# Đề xuất – Trình phân tích CV thông minh
_Một giải pháp serverless hợp nhất trên AWS để phân tích CV so với mô tả công việc và tạo Điểm Phù Hợp_

> **Lưu ý:** Bản đề xuất này giữ bố cục theo mẫu `_index.md` trước đó nhưng đã được viết lại cho dự án Trình phân tích CV thông minh.

---

## 1) Tóm tắt điều hành
**Trình phân tích CV thông minh** là một nền tảng web serverless đánh giá mức độ phù hợp giữa **CV** của ứng viên và **Mô tả công việc (JD)**. Hệ thống tính toán **Điểm Phù Hợp (Fit Score)**, phát hiện **khoảng cách kỹ năng**, và đưa ra **gợi ý học tập cá nhân hóa**.  
Giải pháp được triển khai bởi đội 5 người trong **4 tuần** trên **AWS** sử dụng các dịch vụ quản lý, trả tiền theo sử dụng để giữ chi phí gần như bằng không cho khối lượng demo. Giao diện được xây bằng **Next.js** và host trên **AWS Amplify**; backend dùng **API Gateway + Lambda** với **DynamoDB**, **S3**, **Comprehend**, **Textract**, và **Cognito**.

**Kết quả chính**
- Rút ngắn 90% thời gian sàng lọc CV cho kịch bản demo.
- Điểm Phù Hợp khách quan kèm báo cáo hình ảnh.
- Lộ trình học tập có thể hành động cho từng ứng viên.

---

## 2) Vấn đề
### 2.1 Vấn đề là gì?
- Nhân sự tuyển dụng phải mất nhiều thời gian đọc thủ công CV và so sánh với JD.  
- Ứng viên thiếu thông tin về kỹ năng còn thiếu và cách cải thiện.  
- Các công cụ hiện có đắt tiền hoặc không phù hợp cho thị trường Việt Nam/Đông Nam Á.

### 2.2 Giải pháp
- Tải lên CV (PDF/DOCX) và JD → tự động trích xuất văn bản và xử lý NLP.  
- Phát hiện **kỹ năng, kinh nghiệm, học vấn**; tính **Điểm Phù Hợp** so với JD.  
- Gợi ý **lộ trình kỹ năng** dựa trên kho **SkillOntology** nhỏ.  
- Đăng nhập an toàn bằng **Cognito**; kết quả hiển thị trên dashboard **Next.js** gọn gàng.

---

## 3) Kiến trúc giải pháp (tổng quan)

![Solution Architecture Diagram](https://i.ibb.co/ZR0VcspJ/Solution-Architecture.png)

Kiến trúc serverless, hướng sự kiện trên AWS.

**Thành phần chính**
- **Frontend**: Giao diện Next.js (Amplify Hosting) cho upload & dashboard kết quả.  
- **API Layer**: Amazon API Gateway → AWS Lambda functions.  
- **Xử lý**: 
  - `parseResume` → Textract (nếu PDF là scan) → chuẩn hóa văn bản.  
  - `nlpAnalyze` → Comprehend → trích xuất thực thể/kỹ năng/ cụm từ.  
  - `recommendSkills` → so sánh với JD + `SkillOntology` trên DynamoDB.  
- **Dữ liệu**: DynamoDB (kết quả, ontology), S3 (lưu tạm CV/JD).  
- **Nhận dạng**: Cognito (JWT access tokens).  
- **Vận hành**: IaC với AWS SAM, CI/CD bằng CodeBuild + CodePipeline, logging trên CloudWatch.

**(Có kèm sơ đồ kiến trúc Mermaid riêng.)**

---

## 4) Triển khai kỹ thuật
### 4.1 Ngăn xếp công nghệ
- **Backend**: .NET 8 (C# Minimal API trên Lambda)  
- **Frontend**: Next.js + TailwindCSS (Amplify Hosting)  
- **AWS**: Lambda, API Gateway, DynamoDB, S3, Cognito, Comprehend, Textract  
- **IaC**: AWS SAM  
- **CI/CD**: CodeBuild + CodePipeline

### 4.2 Luồng end‑to‑end
1. Người dùng xác thực qua **Cognito** và lấy JWT.
2. Frontend yêu cầu **presigned URL** tới **S3** → upload CV/JD.
3. API Gateway kích hoạt **Lambda `parseResume`**:  
   - Nếu PDF là scan → **Textract** → trích xuất văn bản; nếu không thì parse trực tiếp.  
   - Làm sạch & chuẩn hóa → lưu tạm artifacts lên S3.
4. **Lambda `nlpAnalyze`** dùng **Comprehend** để phát hiện thực thể/kỹ năng → ghi kết quả vào **DynamoDB**.
5. **Lambda `recommendSkills`** load **SkillOntology** từ DynamoDB → so sánh CV vs JD → tính **Điểm Phù Hợp** và khoảng cách.
6. Frontend truy vấn kết quả qua API → hiển thị biểu đồ/bảng.

### 4.3 Mô hình dữ liệu (DynamoDB – giản lược)
- **Bảng `Profiles`** (PK: `userId`, SK: `profileId`) – lưu parse CV gần nhất.  
- **Bảng `Analyses`** (PK: `analysisId`) – điểm phù hợp, khoảng cách kỹ năng, timestamps.  
- **Bảng `SkillOntology`** (PK: `skillId`, thuộc tính: `name`, `tags`, `learningPath[]`).

### 4.4 API (mức cao)
- `POST /upload-url` → presign cho CV/JD.  
- `POST /analyze` → kích hoạt pipeline cho cặp key S3.  
- `GET /analyses/{id}` → trả về Điểm Phù Hợp & khuyến nghị.  
- `GET /skills/{id}` → (tùy chọn) lấy lộ trình học cho một kỹ năng.

---

## 5) Timeline & Mốc (4 tuần)
| Tuần | Mốc hoàn thành                | Deliverables                                       |
| ---- | ---------------------------- | --------------------------------------------------- |
| 1    | Nền tảng cơ sở               | Template SAM, bảng DynamoDB, Cognito, UI cơ bản    |
| 2    | Parsing & NLP                | `parseResume`, `nlpAnalyze`, parsing JD, unit tests |
| 3    | Recommender & tích hợp FE    | `recommendSkills`, dashboard, biểu đồ              |
| 4    | Demo & hoàn thiện            | E2E tests, logging, tinh chỉnh chi phí, slide deck |

---

## 6) Ước tính chi phí (cho demo)
_Giá trị ước tính, giả sử < 500 request/tháng_
- **Lambda**: ~$0.02  
- **API Gateway**: ~$0.01  
- **S3** (vài GB, request thấp): ~$0.10  
- **DynamoDB** (on‑demand, R/W thấp): ~$0.05  
- **Amplify Hosting**: ~$0.30  
- **Comprehend + Textract (trang nhỏ)**: ~$0.40  
- **Cognito**: $0.00  
**Tổng ≈ $0.9 / tháng (~$10 / năm)**

---

## 7) Bảo mật, rủi ro & biện pháp giảm thiểu
**Bảo mật**
- S3 private với **SSE‑KMS**; chỉ dùng presigned uploads.  
- **IAM tối thiểu quyền**; API bảo vệ bằng **Cognito JWT**.  
- **Mã hóa/che chắn PII** trong logs; **CloudWatch** alarms.  
- Tùy chọn: rules lifecycle để xóa CV/JD thô sau khi phân tích.

**Rủi ro & giảm thiểu**
- _Độ chính xác NLP_: Cung cấp định dạng hỗ trợ + fallback bằng quy tắc từ khóa.  
- _CV lớn/không chuẩn_: Kiểm tra kích thước/định dạng; sanitize trước khi NLP.  
- _Spike chi phí_: Cảnh báo Budget của AWS; giới hạn số trang tối đa cho mỗi request.

---

## 8) Kết quả mong đợi
- Tự động hoá việc so khớp CV‑JD với **Điểm Phù Hợp** minh bạch.  
- Phân tích hình ảnh: **kỹ năng trùng khớp vs khoảng cách** và **lộ trình học**.  
- Kiến trúc serverless, ít vận hành, dễ demo, mở rộng và bản địa hoá.

---

## 📄 Tài liệu đề xuất (Google Docs)


👉 **Xem lại đề xuất tại:**  
[GOOGLE DOC LINK](https://docs.google.com/document/d/1ALFieRvZWl1Azg3C8a7L8Z-iL6-chpzS/edit?usp=sharing&ouid=100398969873071071371&rtpof=true&sd=true)
