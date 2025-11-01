# Compute Services - Exam Style Questions

> 📝 **Format đề thi thật**: Multiple choice và multiple response

---

## Question 1
What is Amazon EC2?

A. A database service  
B. A compute service that provides virtual servers in the cloud  
C. A storage service  
D. A networking service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** EC2 = Elastic Compute Cloud = virtual servers trong cloud. Bạn có thể launch instances với OS và applications, scale theo nhu cầu.

**Exam Tip:** EC2 = Virtual servers, IaaS model.
</details>

---

## Question 2
Which AWS service allows you to run code without managing servers?

A. Amazon EC2  
B. AWS Lambda  
C. Amazon ECS  
D. AWS Elastic Beanstalk

<details>
<summary><strong>Answer: B - AWS Lambda</strong></summary>

**Explanation:** Lambda = serverless compute. Bạn chỉ viết code (function), AWS quản lý servers, scaling, patching. Pay-per-execution, no servers to manage.

**Exam Tip:** Lambda = Serverless = No server management.
</details>

---

## Question 3
Which EC2 pricing model allows you to pay for instances on a per-second basis with no upfront payment?

A. Reserved Instances  
B. Spot Instances  
C. On-Demand Instances  
D. Dedicated Instances

<details>
<summary><strong>Answer: C - On-Demand Instances</strong></summary>

**Explanation:** On-Demand = pay per-second (minimum 1 minute), no upfront payment, no commitment. Most flexible, highest cost. Reserved = commitment cho discount, Spot = unused capacity.

**Exam Tip:** On-Demand = Most flexible, pay per-second, no commitment.
</details>

---

## Question 4
What happens to a Spot Instance when AWS needs the capacity back?

A. Nothing, it continues running  
B. You get a 2-minute warning before termination  
C. It is automatically stopped  
D. It is automatically migrated

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Spot Instances = dùng unused capacity với discount lớn. Khi AWS cần capacity, bạn nhận 2-minute warning trước khi terminate. Phù hợp cho fault-tolerant workloads.

**Exam Tip:** Spot = Cheapest, interruptible với 2-minute warning.
</details>

---

## Question 5
What is AWS Lambda's maximum execution time?

A. 5 minutes  
B. 15 minutes  
C. 1 hour  
D. Unlimited

<details>
<summary><strong>Answer: B - 15 minutes</strong></summary>

**Explanation:** Lambda có timeout tối đa 15 minutes. Nếu function chạy lâu hơn, sẽ timeout. Cho long-running tasks, dùng EC2 hoặc ECS.

**Exam Tip:** Lambda timeout = 15 minutes maximum.
</details>

---

## Question 6
Which AWS service is a container orchestration service?

A. AWS Lambda  
B. Amazon ECS  
C. Amazon EC2  
D. AWS Elastic Beanstalk

<details>
<summary><strong>Answer: B - Amazon ECS</strong></summary>

**Explanation:** ECS = Elastic Container Service = fully managed container orchestration. Chạy Docker containers trên EC2 hoặc Fargate (serverless).

**Exam Tip:** ECS = Container orchestration. Fargate = Serverless option.
</details>

---

## Question 7
What is AWS Elastic Beanstalk?

A. A database service  
B. A service that automatically handles deployment, capacity provisioning, and load balancing  
C. A storage service  
D. A networking service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Elastic Beanstalk = PaaS. Bạn upload code, Beanstalk tự động handle deployment, provisioning, load balancing, monitoring. Support nhiều languages.

**Exam Tip:** Beanstalk = PaaS = Upload code, AWS handles infrastructure.
</details>

---

## Question 8
What is an AMI in EC2?

A. Amazon Machine Image - a template for EC2 instances  
B. Amazon Management Interface  
C. Amazon Monitoring Instance  
D. Amazon Migration Instance

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** AMI = Amazon Machine Image = template chứa OS, applications, configurations. Khi launch EC2, bạn chọn AMI. Có thể tạo custom AMIs.

**Exam Tip:** AMI = Template cho EC2 instances.
</details>

---

## Question 9
Which EC2 pricing model offers the highest discount but requires 1-3 year commitment?

A. On-Demand  
B. Reserved Instances  
C. Spot Instances  
D. Dedicated Instances

<details>
<summary><strong>Answer: B - Reserved Instances</strong></summary>

**Explanation:** Reserved Instances = commit 1 hoặc 3 years, discount up to 72% so với On-Demand. Cho steady-state workloads. Spot = cheaper nhưng interruptible.

**Exam Tip:** Reserved = Commitment = Highest discount (up to 72%).
</details>

---

## Question 10
What is EC2 Auto Scaling used for?

A. To automatically start instances  
B. To automatically adjust the number of EC2 instances based on demand  
C. To automatically stop instances  
D. To automatically migrate instances

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Auto Scaling = tự động adjust số lượng instances dựa trên demand (CPU, network, custom metrics). Scale out khi tăng, scale in khi giảm.

**Exam Tip:** Auto Scaling = Automatic capacity adjustment based on demand.
</details>

---

## Question 11
What is AWS Fargate?

A. A database service  
B. A serverless compute engine for containers  
C. A storage service  
D. A networking service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Fargate = serverless compute engine cho containers. Chạy containers mà không cần manage EC2 instances. Dùng với ECS hoặc EKS. Pay cho resources sử dụng.

**Exam Tip:** Fargate = Serverless containers, no EC2 management.
</details>

---

## Question 12
Which AWS service is best suited for event-driven applications?

A. EC2  
B. Lambda  
C. ECS  
D. Elastic Beanstalk

<details>
<summary><strong>Answer: B - Lambda</strong></summary>

**Explanation:** Lambda = perfect cho event-driven. Triggers từ S3, API Gateway, CloudWatch events, etc. Automatic scaling, pay-per-execution. Không cần maintain servers.

**Exam Tip:** Lambda = Event-driven applications.
</details>

---

## Question 13
What is the difference between EC2 Instance Store and EBS volumes?

A. Instance Store is persistent, EBS is ephemeral  
B. Instance Store is ephemeral (lost on stop/terminate), EBS is persistent  
C. They are the same  
D. Instance Store is for databases, EBS is for applications

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Instance Store = temporary storage (ephemeral), data mất khi instance stop/terminate. EBS = persistent block storage, data tồn tại độc lập với instance lifecycle.

**Exam Tip:** Instance Store = Ephemeral | EBS = Persistent.
</details>

---

## Question 14
What is an EC2 Security Group?

A. A group of EC2 instances  
B. A virtual firewall that controls inbound and outbound traffic  
C. A group of users  
D. A backup group

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Security Groups = virtual firewall cho EC2 instances. Control inbound (incoming) và outbound (outgoing) traffic. Rules-based, stateful (allow return traffic automatically).

**Exam Tip:** Security Groups = Virtual firewall for EC2.
</details>

---

## Question 15
Which AWS service would you use to run Docker containers without managing servers?

A. EC2  
B. Lambda  
C. ECS with Fargate  
D. Elastic Beanstalk

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** ECS với Fargate = run Docker containers mà không cần manage EC2 instances. Fargate = serverless. Lambda không support Docker containers directly.

**Exam Tip:** Containers without servers = ECS + Fargate.
</details>

---

## Question 16
What happens to data stored on an EC2 instance's Instance Store when the instance is stopped?

A. Data persists  
B. Data is backed up automatically  
C. Data is lost (Instance Store is ephemeral)  
D. Data is migrated to S3

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Instance Store = ephemeral storage, data mất khi instance stop/terminate. Chỉ dùng cho temporary data, cache. Cho persistent data, dùng EBS volumes.

**Exam Tip:** Instance Store = Lost on stop/terminate.
</details>

---

## Question 17
What is the purpose of an Elastic Load Balancer (ELB)?

A. To balance storage across multiple S3 buckets  
B. To distribute incoming traffic across multiple EC2 instances  
C. To balance database connections  
D. To balance network bandwidth

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** ELB = distribute incoming traffic across multiple EC2 instances (hoặc targets) để đảm bảo high availability và fault tolerance. Types: ALB (application), NLB (network), CLB (classic).

**Exam Tip:** ELB = Distribute traffic across instances.
</details>

---

## Question 18
Which EC2 instance type family is optimized for compute-intensive workloads?

A. T family (burstable)  
B. M family (general purpose)  
C. C family (compute optimized)  
D. R family (memory optimized)

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** C = Compute-optimized (high CPU) cho compute-intensive workloads. M = General purpose, R = Memory-optimized, T = Burstable performance.

**Exam Tip:** Instance families: C = Compute, R = Memory, M = General, T = Burstable.
</details>

---

## Question 19
What is the difference between EC2 and Lambda? (Select TWO)

A. EC2 requires server management, Lambda is serverless  
B. EC2 has a 15-minute execution limit, Lambda has unlimited execution time  
C. Lambda requires server management, EC2 is serverless  
D. Lambda has a 15-minute execution limit, EC2 has unlimited execution time  
E. EC2 is for containers, Lambda is for virtual machines

<details>
<summary><strong>Answer: A, D</strong></summary>

**Explanation:** 
- EC2 = requires server management, unlimited execution time
- Lambda = serverless, 15-minute execution limit
- B sai (ngược), C sai (ngược), E sai (Lambda = functions, không phải containers)

**Exam Tip:** EC2 = Servers, unlimited time | Lambda = Serverless, 15-min limit.
</details>

---

## Question 20
Which of the following are benefits of using Reserved Instances? (Select TWO)

A. Highest flexibility  
B. Up to 72% discount compared to On-Demand  
C. No commitment required  
D. 1-3 year commitment  
E. Can be terminated anytime without penalty

<details>
<summary><strong>Answer: B, D</strong></summary>

**Explanation:** Reserved Instances benefits: Discount up to 72%, commitment options (1-3 years). A, C, E mô tả On-Demand, không phải Reserved.

**Exam Tip:** Reserved = Discount với commitment | On-Demand = Flexibility với no commitment.
</details>

---

## 📊 Exam Simulation

Làm 20 câu trong **30 phút**:
- **18-20 đúng**: ✅ Ready!
- **15-17 đúng**: ✅ Good!
- **Dưới 15 đúng**: 📚 Review

---

## 💡 Exam Tips

1. **EC2** = Virtual servers, full control
2. **Lambda** = Serverless, 15-min limit, event-driven
3. **Pricing**: On-Demand (flexible), Reserved (discount), Spot (cheapest, interruptible)
4. **Auto Scaling** = Automatic capacity adjustment
5. **ECS** = Containers, **Fargate** = Serverless containers

---

## 🔄 Review Schedule

- Lần 1: Sau khi học notes
- Lần 2: Sau 2 ngày
- Lần 3: Sau 5 ngày
- Lần 4: 1 tuần trước khi thi

Mục tiêu: 100%!

