# Cloud Concepts - Flashcards

> 💡 Cách dùng: Đọc câu hỏi, tự trả lời, rồi xem đáp án. Lặp lại nhiều lần để ghi nhớ.

---

## Q: Cloud computing là gì?
**A:** On-demand delivery của computing resources qua internet với pay-as-you-go pricing.

---

## Q: 5 đặc điểm chính của cloud (NIST)?
**A:** 
1. On-demand self-service
2. Broad network access
3. Resource pooling
4. Rapid elasticity
5. Measured service

---

## Q: Lợi ích chính của cloud computing?
**A:** 
- Giảm CapEx, tăng OpEx (pay-as-you-go)
- Agility (deploy nhanh)
- Scalability & Elasticity
- High availability
- Global reach

---

## Q: IaaS là gì? Ví dụ?
**A:** Infrastructure as a Service - AWS quản lý hardware/networking, bạn quản lý OS/apps.
**Ví dụ AWS:** EC2, EBS, VPC

---

## Q: PaaS là gì? Ví dụ?
**A:** Platform as a Service - AWS quản lý cả OS/runtime, bạn quản lý apps/data.
**Ví dụ AWS:** Elastic Beanstalk, RDS

---

## Q: SaaS là gì? Ví dụ?
**A:** Software as a Service - AWS quản lý mọi thứ, bạn chỉ sử dụng.
**Ví dụ:** Gmail, Office 365

---

## Q: Serverless/FaaS là gì? Ví dụ AWS?
**A:** Function as a Service - Bạn chỉ viết code (function), AWS quản lý mọi thứ khác.
**Ví dụ AWS:** Lambda

---

## Q: Sự khác biệt giữa Public, Private, Hybrid cloud?
**A:** 
- **Public:** Third-party cloud (AWS, Azure)
- **Private:** Dedicated cho một organization
- **Hybrid:** Kết hợp on-premises + cloud

---

## Q: Region là gì?
**A:** Geographic area chứa multiple Availability Zones. Ví dụ: us-east-1, ap-southeast-1

---

## Q: Availability Zone (AZ) là gì?
**A:** Một hoặc nhiều data centers riêng biệt với redundant power/networking trong một Region.

---

## Q: Edge Location là gì?
**A:** Locations gần users để cache content (cho CloudFront CDN), nhiều hơn AZs rất nhiều.

---

## Q: AWS Shared Responsibility Model - AWS chịu trách nhiệm gì?
**A:** Security **OF** the cloud - Infrastructure, hardware, networking, regions/AZs.

---

## Q: AWS Shared Responsibility Model - Customer chịu trách nhiệm gì?
**A:** Security **IN** the cloud - Data, applications, OS (tùy service model), access control.

---

## Q: Scalability vs Elasticity?
**A:** 
- **Scalability:** Khả năng xử lý tăng trưởng (có thể manual)
- **Elasticity:** Tự động scale up/down theo demand (automatic)

---

## Q: Horizontal scaling vs Vertical scaling?
**A:** 
- **Horizontal:** Thêm nhiều servers (scale out)
- **Vertical:** Tăng CPU/RAM cho existing server (scale up)

---

## Q: Agility trong cloud là gì?
**A:** Khả năng phát triển và deploy applications nhanh chóng (vài phút vs vài tuần).

---

## Q: Fault tolerance là gì?
**A:** Khả năng tiếp tục hoạt động khi có component failure (đạt được bằng redundancy).

---

## Q: High availability là gì?
**A:** System vẫn hoạt động với minimal downtime khi có failure.

---

## Q: Resource pooling là gì?
**A:** Tài nguyên được chia sẻ giữa nhiều customers (multi-tenant) để tăng efficiency.

---

## Q: Pay-as-you-go model là gì?
**A:** Trả tiền theo actual usage, không có upfront costs, variable costs thay vì fixed costs.

---

## Q: Tại sao cần deploy across multiple AZs?
**A:** Để đảm bảo high availability và fault tolerance - nếu một AZ fails, app vẫn chạy.

---

## 🎯 Quick Reference

### Service Models (từ thấp đến cao):
**IaaS** → **PaaS** → **SaaS** → **FaaS/Serverless**

Bạn quản lý ít dần từ trái sang phải.

### AWS Infrastructure Hierarchy:
**Region** → Contains → **Availability Zones** → Contains → **Data Centers**

**Edge Locations** = Separate, nhiều hơn AZs (cho CDN)

### Key Concepts:
- **Cloud** = Pay-as-you-go, on-demand, scalable
- **IaaS** = You manage OS, AWS manages infra
- **PaaS** = AWS manages OS too
- **SaaS** = AWS manages everything
- **Shared Responsibility** = AWS: OF cloud | Customer: IN cloud

