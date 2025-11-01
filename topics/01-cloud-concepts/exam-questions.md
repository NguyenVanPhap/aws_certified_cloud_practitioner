# Cloud Concepts - Exam Style Questions

> 📝 **Lưu ý**: Đây là các câu hỏi theo format đề thi thật AWS Certified Cloud Practitioner. Làm như đang thi thật - không xem đáp án ngay!

---

## Question 1
A company wants to move its infrastructure to the cloud to reduce operational costs and increase scalability. Which cloud computing characteristic allows the infrastructure to automatically adjust capacity based on demand?

A. High availability  
B. Elasticity  
C. Durability  
D. Consistency

<details>
<summary><strong>Answer: B - Elasticity</strong></summary>

**Explanation:** Elasticity là khả năng tự động scale resources up hoặc down dựa trên demand. High availability = minimal downtime, Durability = data persistence, Consistency = data consistency.

**Exam Tip:** Elasticity vs Scalability - Elasticity = automatic, Scalability = ability to grow (có thể manual hoặc automatic).
</details>

---

## Question 2
Which of the following is a benefit of using cloud computing over traditional on-premises infrastructure? (Select TWO)

A. Reduced capital expenditure (CapEx)  
B. Increased operational expenditure (OpEx)  
C. Manual capacity planning  
D. Pay-as-you-go pricing model  
E. Fixed infrastructure costs

<details>
<summary><strong>Answer: A, D</strong></summary>

**Explanation:** 
- **A. Reduced CapEx**: Cloud eliminates upfront hardware costs
- **D. Pay-as-you-go**: Pay only for what you use, variable costs
- B, C, E là đặc điểm của on-premises, không phải benefits của cloud

**Exam Tip:** Multiple response questions - chọn tất cả đáp án đúng. CapEx = Capital expenditure (upfront), OpEx = Operational expenditure (ongoing).
</details>

---

## Question 3
An organization needs to store sensitive data in a dedicated cloud infrastructure that is only accessible to its employees. Which cloud deployment model should they use?

A. Public cloud  
B. Private cloud  
C. Hybrid cloud  
D. Multi-cloud

<details>
<summary><strong>Answer: B - Private cloud</strong></summary>

**Explanation:** Private cloud = dedicated infrastructure cho một organization, highest control và security. Public = shared, Hybrid = mix on-premises + cloud, Multi-cloud = multiple providers.

**Exam Tip:** Private cloud thường dùng cho organizations cần strict security/compliance (banking, healthcare).
</details>

---

## Question 4
What does the AWS Shared Responsibility Model state about security responsibilities?

A. AWS is responsible for all security aspects  
B. Customer is responsible for all security aspects  
C. AWS is responsible for security OF the cloud, customer is responsible for security IN the cloud  
D. Security responsibilities are split equally between AWS and customer

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** AWS = Security OF the cloud (infrastructure, hardware, networking, physical security). Customer = Security IN the cloud (data, applications, OS - tùy service model).

**Exam Tip:** Đây là một trong những concept quan trọng nhất trong exam. Nhớ: AWS = OF, Customer = IN.
</details>

---

## Question 5
Which AWS service provides Infrastructure as a Service (IaaS)?

A. AWS Lambda  
B. Amazon EC2  
C. AWS Elastic Beanstalk  
D. Amazon RDS

<details>
<summary><strong>Answer: B - Amazon EC2</strong></summary>

**Explanation:** EC2 = IaaS vì bạn quản lý OS, applications; AWS quản lý infrastructure. Lambda = FaaS/Serverless, Beanstalk = PaaS, RDS = Managed database (PaaS).

**Exam Tip:** IaaS = You manage OS & apps | PaaS = AWS manages OS | SaaS = AWS manages everything
</details>

---

## Question 6
A company wants to deploy an application that can automatically scale based on traffic. Which cloud computing benefit does this represent?

A. Agility  
B. Elasticity  
C. Durability  
D. High availability

<details>
<summary><strong>Answer: B - Elasticity</strong></summary>

**Explanation:** Elasticity = tự động scale based on traffic/demand. Agility = speed of deployment, Durability = data persistence, High availability = minimal downtime.

**Exam Tip:** Elasticity = automatic scaling based on demand là một trong những benefits chính của cloud.
</details>

---

## Question 7
What is the purpose of AWS Regions?

A. To reduce costs  
B. To reduce latency by placing resources closer to users  
C. To improve security  
D. To simplify management

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Regions = geographic areas chứa multiple AZs. Đặt resources gần users → giảm latency. Cũng dùng cho compliance (data residency requirements).

**Exam Tip:** Regions = Geographic locations, chọn dựa trên user location hoặc compliance requirements.
</details>

---

## Question 8
Which of the following are characteristics of cloud computing according to the NIST definition? (Select THREE)

A. On-demand self-service  
B. Fixed capacity  
C. Resource pooling  
D. Rapid elasticity  
E. Manual provisioning

<details>
<summary><strong>Answer: A, C, D</strong></summary>

**Explanation:** NIST 5 characteristics: 1) On-demand self-service, 2) Broad network access, 3) Resource pooling, 4) Rapid elasticity, 5) Measured service. Fixed capacity và manual provisioning là đặc điểm của on-premises.

**Exam Tip:** Nhớ 5 NIST characteristics: On-demand, Broad access, Resource pooling, Elasticity, Measured service.
</details>

---

## Question 9
What is the difference between horizontal scaling and vertical scaling?

A. Horizontal scaling adds more servers, vertical scaling increases server capacity  
B. Horizontal scaling is manual, vertical scaling is automatic  
C. Horizontal scaling is for cloud, vertical scaling is for on-premises  
D. They are the same thing

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** Horizontal scaling (scale out) = thêm nhiều servers/instances. Vertical scaling (scale up) = tăng CPU/RAM của existing server. Cloud thường dùng horizontal scaling vì dễ hơn.

**Exam Tip:** Horizontal = More servers | Vertical = More power to server
</details>

---

## Question 10
Which AWS service model does AWS Lambda represent?

A. Infrastructure as a Service (IaaS)  
B. Platform as a Service (PaaS)  
C. Function as a Service (FaaS) / Serverless  
D. Software as a Service (SaaS)

<details>
<summary><strong>Answer: C - Function as a Service (FaaS) / Serverless</strong></summary>

**Explanation:** Lambda = Serverless/FaaS - bạn chỉ viết code (function), AWS quản lý mọi thứ khác. Không phải IaaS, PaaS, hay SaaS.

**Exam Tip:** Serverless = No servers to manage, pay-per-execution
</details>

---

## Question 11
An organization wants to use both on-premises infrastructure and cloud services. Which cloud deployment model should they use?

A. Public cloud  
B. Private cloud  
C. Hybrid cloud  
D. Community cloud

<details>
<summary><strong>Answer: C - Hybrid cloud</strong></summary>

**Explanation:** Hybrid cloud = kết hợp on-premises + cloud services. Cho phép kết nối giữa 2 môi trường. Dùng khi migrate dần hoặc sensitive data ở on-premises.

**Exam Tip:** Hybrid = On-premises + Cloud, kết nối giữa 2 environments
</details>

---

## Question 12
What is an Availability Zone (AZ) in AWS?

A. A geographic region  
B. One or more discrete data centers with redundant power, networking, and connectivity  
C. A virtual network  
D. A storage location

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** AZ = một hoặc nhiều data centers riêng biệt với redundant power, networking, connectivity. Mỗi Region có multiple AZs. Isolated từ AZ khác.

**Exam Tip:** Region → Contains → Availability Zones → Contains → Data Centers
</details>

---

## Question 13
Which statement about cloud computing costs is correct?

A. Cloud computing always costs less than on-premises  
B. Cloud computing uses variable costs based on usage  
C. Cloud computing requires upfront capital investment  
D. Cloud computing has fixed monthly fees

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Cloud = variable costs (pay-as-you-go) based on actual usage. Không có upfront capital investment (đó là on-premises). Không phải always cheaper - tùy use case.

**Exam Tip:** Cloud = Variable costs, OpEx model. On-premises = Fixed costs, CapEx model.
</details>

---

## Question 14
What does "agility" mean in cloud computing?

A. Fast internet connection  
B. The ability to quickly develop and deploy applications  
C. The ability to scale horizontally  
D. The ability to reduce costs

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Agility = khả năng develop và deploy applications nhanh chóng. Cloud cho phép provision resources trong vài phút vs vài tuần on-premises.

**Exam Tip:** Agility = Speed of innovation, faster time to market
</details>

---

## Question 15
Which of the following best describes resource pooling in cloud computing?

A. Dedicated resources for each customer  
B. Resources shared among multiple customers  
C. Resources stored in a pool  
D. Resources only available during business hours

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Resource pooling = tài nguyên được chia sẻ giữa nhiều customers (multi-tenant). Đây là một trong 5 NIST characteristics. Giúp tăng efficiency và giảm costs.

**Exam Tip:** Multi-tenant = Shared resources, là đặc điểm chính của public cloud
</details>

---

## Question 16
What is the primary purpose of using multiple Availability Zones?

A. To reduce costs  
B. To increase fault tolerance and high availability  
C. To improve internet speed  
D. To simplify management

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Multiple AZs = đảm bảo high availability và fault tolerance. Nếu một AZ fails, application vẫn chạy ở AZ khác. Đây là best practice cho production workloads.

**Exam Tip:** Multiple AZs = High availability = Minimal downtime
</details>

---

## Question 17
Which cloud service model requires you to manage the operating system, but the cloud provider manages the underlying infrastructure?

A. Software as a Service (SaaS)  
B. Platform as a Service (PaaS)  
C. Infrastructure as a Service (IaaS)  
D. Function as a Service (FaaS)

<details>
<summary><strong>Answer: C - Infrastructure as a Service (IaaS)</strong></summary>

**Explanation:** IaaS (như EC2) = bạn quản lý OS, applications, data; cloud provider quản lý infrastructure (hardware, networking). PaaS = provider quản lý cả OS, SaaS = provider quản lý mọi thứ.

**Exam Tip:** Service models từ thấp đến cao: IaaS → PaaS → SaaS → FaaS
</details>

---

## Question 18
What does "fault tolerance" mean in cloud architecture?

A. The ability to prevent failures  
B. The ability to continue operating even when components fail  
C. The ability to reduce costs  
D. The ability to scale automatically

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Fault tolerance = khả năng tiếp tục hoạt động ngay cả khi có component failures. Đạt được bằng redundancy (multiple instances, multiple AZs).

**Exam Tip:** Fault tolerance vs High availability - Fault tolerance = zero downtime, High availability = minimal downtime
</details>

---

## Question 19
Which of the following is a key benefit of using cloud computing for a startup company?

A. Fixed monthly costs regardless of usage  
B. Pay-as-you-go model with no upfront costs  
C. Manual capacity planning required  
D. Limited scalability options

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Pay-as-you-go với no upfront costs = perfect cho startups vì không cần invest lớn ban đầu. Có thể start small và scale khi grow. A, C, D là đặc điểm của on-premises.

**Exam Tip:** Cloud benefits cho startups = Low barrier to entry, scale as you grow
</details>

---

## Question 20
What is the relationship between AWS Regions and Availability Zones?

A. Regions and Availability Zones are the same  
B. An Availability Zone contains multiple Regions  
C. A Region contains multiple Availability Zones  
D. They are independent of each other

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Region = geographic area chứa multiple Availability Zones. Mỗi AZ = isolated data centers với redundancy. Cấu trúc: Region → AZs → Data Centers.

**Exam Tip:** Hierarchy: Region (geographic) → Availability Zones (data centers) → Data Centers (physical)
</details>

---

## 📊 Exam Simulation

Làm toàn bộ 20 câu này trong **30 phút** (trung bình 1.5 phút/câu như đề thi thật):
- Đếm số câu đúng
- Ghi chú lại những câu sai
- Review lại sau 24 giờ

**Scoring:**
- **18-20 đúng**: ✅ Ready for exam!
- **15-17 đúng**: ✅ Good, review weak areas
- **Dưới 15 đúng**: 📚 Cần học lại notes và flashcards

---

## 💡 Exam Tips

1. **Đọc kỹ câu hỏi** - Đặc biệt chú ý keywords: "best", "primary", "most appropriate"
2. **Loại trừ đáp án sai trước** - Tăng xác suất đúng
3. **Multiple response** - Đọc kỹ "Select TWO" hoặc "Select THREE"
4. **Time management** - 1.5 phút/câu, đừng dừng quá lâu ở một câu
5. **Mark for review** - Nếu không chắc, làm câu khác trước, quay lại sau

---

## 🔄 Spaced Repetition

Làm lại file này sau:
- **Lần 1**: Ngay sau khi học notes
- **Lần 2**: Sau 2 ngày
- **Lần 3**: Sau 5 ngày
- **Lần 4**: 1 tuần trước khi thi

Mục tiêu: Đạt 100% trong lần làm cuối cùng!

