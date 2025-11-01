# Cloud Concepts - Practice Questions

> 💡 **Cách học**: Đọc kỹ câu hỏi, tự trả lời trước khi xem đáp án. Đọc kỹ phần giải thích để hiểu sâu.

---

## Question 1
**What is the primary benefit of cloud computing over on-premises infrastructure?**

A. Increased capital expenditure (CapEx)  
B. Reduced operational expenses (OpEx)  
C. Manual scaling required  
D. Limited geographic reach

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Cloud computing chuyển từ CapEx (mua phần cứng trước) sang OpEx (trả tiền theo dùng). Bạn chỉ trả tiền cho những gì sử dụng, giúp giảm chi phí vận hành. Manual scaling và limited geographic reach là đặc điểm của on-premises.

**Key Concept:** Cloud = Pay-as-you-go model → Reduced OpEx
</details>

---

## Question 2
**Which cloud deployment model allows you to use both on-premises infrastructure and cloud services?**

A. Public cloud  
B. Private cloud  
C. Hybrid cloud  
D. Multi-cloud

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Hybrid cloud kết hợp on-premises infrastructure với cloud services, cho phép kết nối giữa hai môi trường. Public cloud = 100% cloud, Private cloud = on-premises hoặc dedicated cloud, Multi-cloud = nhiều cloud providers.

**Key Concept:** Hybrid = On-premises + Cloud services
</details>

---

## Question 3
**What does "elasticity" mean in cloud computing?**

A. The ability to automatically scale resources up or down based on demand  
B. The ability to store unlimited data  
C. The ability to access resources from anywhere  
D. The ability to reduce costs permanently

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** Elasticity là khả năng tự động scale resources (tăng/giảm) dựa trên nhu cầu. Ví dụ: Auto Scaling trong EC2 tự động thêm/xóa instances khi traffic tăng/giảm. Khác với scalability (khả năng scale overall).

**Key Concept:** Elasticity = Auto scaling based on demand
</details>

---

## Question 4
**Which AWS service provides Infrastructure as a Service (IaaS)?**

A. AWS Lambda  
B. AWS Elastic Beanstalk  
C. Amazon EC2  
D. AWS RDS

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** EC2 là IaaS vì bạn quản lý OS, applications, nhưng AWS quản lý hardware, networking. Lambda = Serverless (PaaS), Elastic Beanstalk = PaaS, RDS = Managed Database (PaaS).

**Key Concept:** IaaS = You manage OS & applications, AWS manages infrastructure
</details>

---

## Question 5
**What is the difference between scalability and elasticity?**

A. They are the same concept  
B. Scalability is automatic, elasticity is manual  
C. Scalability is the ability to handle growth, elasticity is automatic scaling based on demand  
D. Scalability requires cloud, elasticity works on-premises

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Scalability = khả năng xử lý tăng trưởng (growth), có thể manual hoặc automatic. Elasticity = tự động scale up/down theo demand. Elasticity là subset của scalability với tính tự động.

**Key Concept:** Scalability = Handle growth | Elasticity = Auto scaling
</details>

---

## Question 6
**Which of the following is NOT a benefit of cloud computing?**

A. Pay-as-you-go pricing  
B. Unlimited capacity  
C. Reduced time to market  
D. Fixed monthly costs regardless of usage

<details>
<summary><strong>Answer: D</strong></summary>

**Explanation:** Cloud computing dùng pay-as-you-go model, không có fixed monthly costs. Bạn trả theo actual usage. Unlimited capacity (thực tế gần như unlimited), reduced time to market (deploy nhanh) là lợi ích của cloud.

**Key Concept:** Cloud = Variable costs based on usage, not fixed costs
</details>

---

## Question 7
**What does "agility" mean in cloud computing?**

A. Fast internet connection  
B. The ability to quickly develop and deploy applications  
C. The ability to scale horizontally  
D. The ability to reduce costs

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Agility = khả năng phát triển và deploy applications nhanh chóng. Cloud cho phép bạn provision resources trong vài phút thay vì vài tuần như on-premises. Điều này giúp innovate và release features nhanh hơn.

**Key Concept:** Agility = Speed of development and deployment
</details>

---

## Question 8
**Which cloud service model requires you to manage the operating system, but AWS manages the underlying infrastructure?**

A. Software as a Service (SaaS)  
B. Platform as a Service (PaaS)  
C. Infrastructure as a Service (IaaS)  
D. Function as a Service (FaaS)

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** IaaS (như EC2) = bạn quản lý OS, applications, data; AWS quản lý hardware, networking, virtualization. PaaS = AWS quản lý cả OS; SaaS = AWS quản lý mọi thứ.

**Key Concept:** IaaS = You manage OS | PaaS = AWS manages OS | SaaS = AWS manages everything
</details>

---

## Question 9
**What is an Availability Zone (AZ) in AWS?**

A. A geographic region containing multiple data centers  
B. One or more discrete data centers with redundant power, networking, and connectivity  
C. A physical location where AWS has data centers  
D. A virtual network in AWS

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Availability Zone = một hoặc nhiều data centers riêng biệt với redundant power, networking, connectivity. Mỗi Region có nhiều AZs để đảm bảo high availability. Region = geographic area, AZ = data centers trong region đó.

**Key Concept:** AZ = Isolated data centers with redundancy within a Region
</details>

---

## Question 10
**Which statement best describes the AWS Shared Responsibility Model?**

A. AWS is responsible for everything  
B. The customer is responsible for everything  
C. AWS is responsible for security OF the cloud, customer is responsible for security IN the cloud  
D. AWS and customer share all responsibilities equally

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** AWS Shared Responsibility Model: AWS chịu trách nhiệm security OF the cloud (infrastructure, hardware, networking). Customer chịu trách nhiệm security IN the cloud (data, applications, OS - tùy service model).

**Key Concept:** AWS = Security OF cloud | Customer = Security IN cloud
</details>

---

## Question 11
**What is the primary purpose of AWS Regions?**

A. To reduce latency by placing resources closer to users  
B. To reduce costs  
C. To improve security  
D. To simplify management

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** Regions giúp đặt resources gần users hơn → giảm latency. Mỗi region là geographic area độc lập. Bạn chọn region dựa trên vị trí users. Ví dụ: users ở Việt Nam → chọn Singapore hoặc Tokyo region.

**Key Concept:** Regions = Geographic locations to reduce latency
</details>

---

## Question 12
**Which of the following is a characteristic of cloud computing?**

A. Dedicated hardware for each customer  
B. Resource pooling  
C. Fixed capacity  
D. Manual provisioning

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Resource pooling = tài nguyên được chia sẻ giữa nhiều customers (multi-tenant). Đây là đặc điểm chính của cloud computing, giúp giảm cost và tăng efficiency. Dedicated hardware là on-premises hoặc dedicated hosting.

**Key Concept:** Cloud = Resource pooling (multi-tenant), not dedicated hardware
</details>

---

## Question 13
**What does "on-demand self-service" mean in cloud computing?**

A. Customers can request resources from AWS support  
B. Customers can provision resources automatically without human interaction  
C. Customers must wait for AWS approval  
D. Customers can only use predefined resources

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** On-demand self-service = khách hàng có thể tự động provision resources (như EC2 instances, S3 buckets) qua console hoặc API mà không cần AWS staff can thiệp. Đây là một trong 5 đặc điểm chính của cloud computing (NIST definition).

**Key Concept:** Self-service = Provision resources automatically via console/API
</details>

---

## Question 14
**Which deployment model provides the highest level of control and security but requires more management?**

A. Public cloud  
B. Private cloud  
C. Hybrid cloud  
D. Community cloud

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Private cloud = dedicated infrastructure cho một organization → highest control & security nhưng requires more management (tự quản lý). Public cloud = shared, ít control hơn nhưng ít management hơn.

**Key Concept:** Private cloud = Highest control/security, most management
</details>

---

## Question 15
**What is the main difference between horizontal scaling and vertical scaling?**

A. Horizontal scaling adds more servers, vertical scaling adds more power to existing servers  
B. Horizontal scaling is manual, vertical scaling is automatic  
C. Horizontal scaling is for cloud, vertical scaling is for on-premises  
D. They are the same thing

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** Horizontal scaling (scale out) = thêm nhiều servers/instances. Vertical scaling (scale up) = tăng CPU/RAM của existing server. Cloud thường dùng horizontal scaling vì dễ hơn và không bị giới hạn hardware.

**Key Concept:** Horizontal = More servers | Vertical = More power to server
</details>

---

## Question 16
**Which AWS service model does AWS Lambda represent?**

A. Infrastructure as a Service (IaaS)  
B. Platform as a Service (PaaS)  
C. Function as a Service (FaaS) / Serverless  
D. Software as a Service (SaaS)

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Lambda = Function as a Service (FaaS) / Serverless. Bạn chỉ viết code (function), AWS quản lý mọi thứ khác (servers, scaling, patching). Bạn trả tiền chỉ khi function chạy.

**Key Concept:** Lambda = Serverless/FaaS = You write code, AWS manages everything else
</details>

---

## Question 17
**What is a key advantage of using multiple Availability Zones?**

A. Reduced costs  
B. Increased fault tolerance and high availability  
C. Simplified management  
D. Faster internet speed

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Multiple AZs giúp đảm bảo high availability và fault tolerance. Nếu một AZ fails, application vẫn chạy ở AZ khác. Đây là best practice cho production workloads.

**Key Concept:** Multiple AZs = High availability and fault tolerance
</details>

---

## Question 18
**Which statement about cloud computing costs is correct?**

A. Cloud computing always costs less than on-premises  
B. Cloud computing uses variable costs based on usage  
C. Cloud computing requires upfront capital investment  
D. Cloud computing has fixed monthly fees

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Cloud computing dùng variable costs (pay-as-you-go) = bạn trả theo actual usage. Không có upfront capital investment như on-premises. Tuy nhiên, cloud không "always" rẻ hơn - tùy use case.

**Key Concept:** Cloud = Variable costs (usage-based), no upfront CapEx
</details>

---

## Question 19
**What does "fault tolerance" mean in cloud architecture?**

A. The ability to prevent failures  
B. The ability to continue operating even when components fail  
C. The ability to reduce costs  
D. The ability to scale automatically

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Fault tolerance = khả năng tiếp tục hoạt động ngay cả khi có components fail. Đạt được bằng cách dùng redundancy (multiple instances, multiple AZs, backup systems).

**Key Concept:** Fault tolerance = Continue operating despite component failures
</details>

---

## Question 20
**Which of the following is a key characteristic of cloud computing according to NIST?**

A. Fixed pricing  
B. Rapid elasticity  
C. Manual provisioning  
D. Single tenant

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Rapid elasticity là một trong 5 đặc điểm chính của cloud computing (NIST definition). Cloud có thể tự động scale resources nhanh chóng. Fixed pricing, manual provisioning, single tenant không phải đặc điểm của cloud.

**Key Concept:** NIST 5 characteristics: On-demand, Broad network access, Resource pooling, Rapid elasticity, Measured service
</details>

---

## 📊 Tự đánh giá

Sau khi làm xong, đếm số câu đúng:
- **18-20 câu đúng**: ✅ Excellent! Bạn đã nắm vững Cloud Concepts
- **15-17 câu đúng**: ✅ Good! Ôn lại những câu sai
- **Dưới 15 câu**: 📚 Review lại notes.md và flashcards.md, làm lại sau 2-3 ngày

---

## 💡 Tips

1. Đọc kỹ giải thích cho mỗi câu, đặc biệt là phần "Key Concept"
2. Ghi chú lại những câu sai và review lại sau
3. Kết hợp với thực hành trên AWS Free Tier
4. Làm lại toàn bộ sau 3-5 ngày để reinforce memory

