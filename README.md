# 🚀 CI/CD Pipeline using Jenkins, Ansible, Docker & Kubernetes on AWS ☁️

![CI/CD Diagram]([https://user-images.githubusercontent.com/xxx/yyyy.png](https://private-user-images.githubusercontent.com/112816078/434653588-6c16688e-b984-4b7e-afea-2146d0219e29.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDQ4Njk5MTUsIm5iZiI6MTc0NDg2OTYxNSwicGF0aCI6Ii8xMTI4MTYwNzgvNDM0NjUzNTg4LTZjMTY2ODhlLWI5ODQtNGI3ZS1hZmVhLTIxNDZkMDIxOWUyOS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNDE3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDQxN1QwNjAwMTVaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1lZjI2MTA5NTFmNmVkZGEyYzAyZjExZjhjNjI2ZTg0MjU4YThlMmNkZGEyMzRhNjA0MGRiM2Y5MGRjYzVjZjAwJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.usyGwElOMcqkbVlsXJrHhnbl5PNcLPQ-NDdIGq8WWB0))


## 📌 Mô tả dự án

Đây là một hệ thống **CI/CD (Continuous Integration / Continuous Deployment)** được triển khai trên **AWS Cloud**, sử dụng các công cụ mạnh mẽ như **Jenkins, Ansible, Docker, và Kubernetes (hoặc EKS)** để tự động hóa toàn bộ quy trình phát triển và triển khai phần mềm.

Quy trình này giúp:
- Tự động hóa build, test và deploy khi có thay đổi mã nguồn
- Đảm bảo phần mềm luôn sẵn sàng triển khai với chất lượng cao
- Giảm rủi ro nhờ kiểm thử sớm và thường xuyên

---

## 🛠️ Công nghệ sử dụng

| Thành phần | Vai trò | Công cụ sử dụng |
|------------|--------|----------------|
| Jenkins Server | CI (Build & Test) | Jenkins, Maven |
| Ansible Server | Automation & Docker Build | Ansible, Docker |
| Kubernetes Server | Deploy & Orchestration | Kubernetes / Amazon EKS |

---

## 🔄 Quy trình hoạt động CI/CD

1️⃣ **Developer đẩy code lên Git**  
→ Jenkins Server sẽ được kích hoạt thông qua webhook hoặc polling

2️⃣ **Jenkins Build + Test ứng dụng**  
→ Dùng Maven để biên dịch, chạy Unit Test, tạo artifact (.JAR/.WAR)

3️⃣ **Ansible + Docker tạo Docker Image**  
→ Ansible script tạo Image và push lên Docker Registry (DockerHub, ECR…)

4️⃣ **Kubernetes triển khai ứng dụng**  
→ Image sẽ được kéo và chạy trong các Pod, đảm bảo khả năng mở rộng, tự phục hồi, và cập nhật liên tục.

---

## 🔁 Luồng hoạt động tổng quát

