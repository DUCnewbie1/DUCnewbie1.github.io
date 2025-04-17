# 🚀 CI/CD Pipeline using Jenkins, Ansible, Docker & Kubernetes on AWS ☁️

![CI/CD Diagram](./5b3011b6-d9e5-47b2-a232-12e452e9c0ff.png)

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

