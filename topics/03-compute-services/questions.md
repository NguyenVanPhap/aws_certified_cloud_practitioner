# Compute Services - Practice Questions

> 💡 **Cách học**: Tự trả lời trước, đọc kỹ giải thích. Hiểu use cases của mỗi service.

---

## Question 1
**What is Amazon EC2?**

A. A database service  
B. A compute service that provides virtual servers in the cloud  
C. A storage service  
D. A networking service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** EC2 (Elastic Compute Cloud) = virtual servers trong cloud. Bạn có thể launch instances với OS và applications của bạn. Có thể scale up/down theo nhu cầu.

**Key Concept:** EC2 = Virtual servers in the cloud
</details>

---

## Question 2
**Which AWS service allows you to run code without managing servers?**

A. Amazon EC2  
B. AWS Lambda  
C. Amazon ECS  
D. AWS Elastic Beanstalk

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Lambda = serverless compute service. Bạn chỉ viết code (function), AWS quản lý servers, scaling, patching. Pay-per-execution, no servers to manage.

**Key Concept:** Lambda = Serverless, no server management
</details>

---

## Question 3
**What is an EC2 instance type?**

A. A type of operating system  
B. Different combinations of CPU, memory, storage, and networking capacity  
C. A type of database  
D. A type of storage

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Instance types = different combinations của CPU, memory, storage, networking. Ví dụ: t2.micro (1 vCPU, 1GB RAM), m5.large (2 vCPUs, 8GB RAM). Chọn dựa trên workload requirements.

**Key Concept:** Instance types = CPU + Memory + Storage + Networking combinations
</details>

---

## Question 4
**Which pricing model allows you to pay for EC2 instances on a per-second basis?**

A. Reserved Instances  
B. Spot Instances  
C. On-Demand Instances  
D. Dedicated Instances

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** On-Demand Instances = pay per-second (minimum 1 minute). No upfront payment, no commitment. Flexible nhưng đắt nhất. Reserved = discounted với commitment, Spot = unused capacity với discount lớn nhưng có thể bị terminate.

**Key Concept:** On-Demand = Pay per-second, most flexible
</details>

---

## Question 5
**What happens to a Spot Instance when AWS needs the capacity back?**

A. Nothing, it continues running  
B. You get a 2-minute warning before termination  
C. It is automatically stopped  
D. It is automatically migrated

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Spot Instances = dùng unused EC2 capacity với discount lớn (up to 90%). Khi AWS cần capacity, bạn nhận 2-minute warning trước khi terminate. Phù hợp cho fault-tolerant, flexible workloads.

**Key Concept:** Spot = Cheap but can be terminated with 2-minute warning
</details>

---

## Question 6
**What is AWS Lambda's maximum execution time?**

A. 5 minutes  
B. 15 minutes  
C. 1 hour  
D. Unlimited

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Lambda có timeout tối đa 15 minutes. Nếu function chạy lâu hơn, sẽ timeout. Phù hợp cho short-running tasks. Cho long-running tasks, dùng EC2 hoặc ECS.

**Key Concept:** Lambda timeout = 15 minutes maximum
</details>

---

## Question 7
**Which AWS service is a container orchestration service?**

A. AWS Lambda  
B. Amazon ECS  
C. Amazon EC2  
D. AWS Elastic Beanstalk

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** ECS (Elastic Container Service) = fully managed container orchestration service. Chạy Docker containers trên EC2 hoặc Fargate (serverless). Orchestration = manage và schedule containers.

**Key Concept:** ECS = Container orchestration service
</details>

---

## Question 8
**What is AWS Elastic Beanstalk?**

A. A database service  
B. A service that automatically handles deployment, capacity provisioning, and load balancing  
C. A storage service  
D. A networking service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Elastic Beanstalk = Platform as a Service (PaaS). Bạn chỉ upload code, Beanstalk tự động handle deployment, provisioning, load balancing, monitoring. Support nhiều languages (Java, .NET, Python, etc.).

**Key Concept:** Beanstalk = PaaS, deploy code, AWS handles infrastructure
</details>

---

## Question 9
**What is an AMI in EC2?**

A. Amazon Machine Image - a template for EC2 instances  
B. Amazon Management Interface  
C. Amazon Monitoring Instance  
D. Amazon Migration Instance

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** AMI = Amazon Machine Image, template chứa OS, applications, configurations. Khi launch EC2 instance, bạn chọn AMI. Có thể tạo custom AMIs từ existing instances.

**Key Concept:** AMI = Template for EC2 instances
</details>

---

## Question 10
**Which EC2 pricing model offers the highest discount but requires 1-3 year commitment?**

A. On-Demand  
B. Reserved Instances  
C. Spot Instances  
D. Dedicated Instances

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Reserved Instances = commit 1 hoặc 3 years, nhận discount up to 72% so với On-Demand. Options: Standard (no modifications), Convertible (can change instance types), Scheduled (specific times).

**Key Concept:** Reserved Instances = Commitment = Highest discount
</details>

---

## Question 11
**What is EC2 Auto Scaling used for?**

A. To automatically start instances  
B. To automatically adjust the number of EC2 instances based on demand  
C. To automatically stop instances  
D. To automatically migrate instances

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Auto Scaling = tự động adjust số lượng EC2 instances dựa trên demand (CPU, network, custom metrics). Scale out khi demand tăng, scale in khi giảm. Đảm bảo có đủ capacity nhưng không over-provision.

**Key Concept:** Auto Scaling = Automatically adjust instances based on demand
</details>

---

## Question 12
**What is AWS Fargate?**

A. A database service  
B. A serverless compute engine for containers  
C. A storage service  
D. A networking service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Fargate = serverless compute engine cho containers. Chạy containers mà không cần manage EC2 instances. Dùng với ECS hoặc EKS. Pay cho resources sử dụng, không pay cho idle instances.

**Key Concept:** Fargate = Serverless containers, no EC2 management
</details>

---

## Question 13
**Which AWS service is best suited for event-driven applications?**

A. EC2  
B. Lambda  
C. ECS  
D. Elastic Beanstalk

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Lambda = perfect cho event-driven applications. Triggers từ S3 uploads, API Gateway requests, CloudWatch events, etc. Automatic scaling, pay-per-execution. Không cần maintain servers.

**Key Concept:** Lambda = Event-driven, automatic triggers
</details>

---

## Question 14
**What is the difference between EC2 Instance Store and EBS volumes?**

A. Instance Store is persistent, EBS is ephemeral  
B. Instance Store is ephemeral (lost on stop/terminate), EBS is persistent  
C. They are the same  
D. Instance Store is for databases, EBS is for applications

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Instance Store = temporary storage (ephemeral), data mất khi instance stop/terminate, nhưng nhanh hơn. EBS = persistent block storage, data tồn tại độc lập với instance lifecycle.

**Key Concept:** Instance Store = Ephemeral | EBS = Persistent
</details>

---

## Question 15
**What is an EC2 Security Group?**

A. A group of EC2 instances  
B. A virtual firewall that controls inbound and outbound traffic  
C. A group of users  
D. A backup group

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Security Groups = virtual firewall cho EC2 instances. Control inbound (incoming) và outbound (outgoing) traffic. Rules-based, stateful (allow return traffic automatically).

**Key Concept:** Security Groups = Virtual firewall for EC2
</details>

---

## Question 16
**Which AWS service would you use to run Docker containers without managing servers?**

A. EC2  
B. Lambda  
C. ECS with Fargate  
D. Elastic Beanstalk

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** ECS với Fargate = run Docker containers mà không cần manage EC2 instances. Fargate = serverless, ECS = orchestration. Lambda không support Docker containers directly.

**Key Concept:** ECS + Fargate = Serverless containers
</details>

---

## Question 17
**What happens to data stored on an EC2 instance's Instance Store when the instance is stopped?**

A. Data persists  
B. Data is backed up automatically  
C. Data is lost (Instance Store is ephemeral)  
D. Data is migrated to S3

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Instance Store = ephemeral storage, data mất khi instance stop/terminate. Chỉ dùng cho temporary data, cache. Cho persistent data, dùng EBS volumes.

**Key Concept:** Instance Store = Lost on stop/terminate
</details>

---

## Question 18
**What is the purpose of an Elastic Load Balancer (ELB)?**

A. To balance storage across multiple S3 buckets  
B. To distribute incoming traffic across multiple EC2 instances  
C. To balance database connections  
D. To balance network bandwidth

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** ELB = distribute incoming traffic across multiple EC2 instances (hoặc targets) để đảm bảo high availability và fault tolerance. Types: ALB (application), NLB (network), CLB (classic).

**Key Concept:** ELB = Distribute traffic across instances
</details>

---

## Question 19
**Which EC2 instance type family is optimized for compute-intensive workloads?**

A. T family (burstable)  
B. M family (general purpose)  
C. C family (compute optimized)  
D. R family (memory optimized)

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Instance families: C = Compute-optimized (high CPU), M = General purpose, R = Memory-optimized, T = Burstable performance. Chọn dựa trên workload: compute-intensive → C, memory-intensive → R.

**Key Concept:** C = Compute | R = Memory | M = General | T = Burstable
</details>

---

## Question 20
**What is the difference between EC2 and Lambda?**

A. They are the same  
B. EC2 requires server management, Lambda is serverless  
C. Lambda requires server management, EC2 is serverless  
D. EC2 is only for databases

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** EC2 = virtual servers, bạn quản lý OS, applications, patching. Lambda = serverless, bạn chỉ viết code, AWS quản lý mọi thứ. Lambda = faster to deploy, no infrastructure management.

**Key Concept:** EC2 = Manage servers | Lambda = Serverless
</details>

---

## 📊 Tự đánh giá

- **18-20 câu đúng**: ✅ Excellent!
- **15-17 câu đúng**: ✅ Good!
- **Dưới 15 câu**: 📚 Review notes.md và flashcards.md

---

## 💡 Tips

1. Hiểu rõ use cases: EC2 = full control, Lambda = serverless, ECS = containers
2. Pricing models: On-Demand (flexible), Reserved (cheap với commitment), Spot (cheapest, interruptible)
3. Security Groups = firewall rules
4. Auto Scaling = automatic capacity adjustment

