# Compute Services - Tóm tắt kiến thức

## 1. Amazon EC2 (Elastic Compute Cloud)

### Khái niệm
EC2 = Virtual servers trong cloud. Bạn có thể launch instances với OS và applications, scale up/down theo nhu cầu.

### EC2 Components:

#### **Instances**
- Virtual servers với CPU, memory, storage, networking
- Chọn instance type dựa trên workload

#### **AMI (Amazon Machine Image)**
- Template cho EC2 instances
- Chứa OS, applications, configurations
- AWS cung cấp hoặc custom AMIs

#### **Instance Types**
- **T family**: Burstable performance (t2.micro - Free Tier)
- **M family**: General purpose (balanced CPU, memory)
- **C family**: Compute-optimized (high CPU)
- **R family**: Memory-optimized (high RAM)
- **G family**: GPU instances
- **I family**: Storage-optimized (high IOPS)

#### **Storage Options:**
- **EBS volumes**: Persistent block storage
- **Instance Store**: Ephemeral (temporary) storage

#### **Security Groups**
- Virtual firewall cho EC2 instances
- Control inbound và outbound traffic
- Rules-based, stateful (auto allow return traffic)

### EC2 Pricing Models:

#### **On-Demand Instances**
- Pay per-second (minimum 1 minute)
- No upfront payment, no commitment
- **Use case**: Short-term, unpredictable workloads
- **Đặc điểm**: Most flexible, highest cost

#### **Reserved Instances**
- 1 hoặc 3 year commitment
- Discount up to 72% so với On-Demand
- **Types**:
  - **Standard**: Highest discount, no modifications
  - **Convertible**: Can change instance types
  - **Scheduled**: Specific time periods
- **Use case**: Steady-state workloads

#### **Spot Instances**
- Dùng unused EC2 capacity
- Discount up to 90%
- **Đặc điểm**: Can be terminated with 2-minute warning
- **Use case**: Fault-tolerant, flexible workloads (batch processing, data analysis)

#### **Dedicated Instances**
- Physical EC2 servers dedicated to your account
- **Use case**: Compliance requirements, licensing

#### **Savings Plans**
- Commit to $ amount per hour for 1 hoặc 3 years
- Flexible across instance families and sizes
- Discount up to 72%

### EC2 Auto Scaling:
- Tự động adjust số lượng instances dựa trên demand
- **Metrics**: CPU, network, custom metrics
- **Benefits**: 
  - High availability
  - Cost optimization (không over-provision)
  - Automatic scaling

---

## 2. AWS Lambda

### Khái niệm
Lambda = Serverless compute service. Bạn chỉ viết code (function), AWS quản lý servers, scaling, patching.

### Đặc điểm:
- **No servers to manage**
- **Automatic scaling** - handle thousands of concurrent executions
- **Pay-per-execution** - chỉ trả khi function chạy
- **Timeout**: Maximum 15 minutes
- **Supported languages**: Python, Node.js, Java, C#, Go, Ruby, etc.

### Use Cases:
- **Event-driven applications**: S3 uploads, API requests, CloudWatch events
- **API backends**: Với API Gateway
- **Data processing**: Transform data, ETL
- **Scheduled tasks**: Cron jobs

### Triggers:
- API Gateway (REST APIs)
- S3 (object uploads/deletes)
- CloudWatch Events (scheduled, event-based)
- DynamoDB (streams)
- Kinesis (streaming data)
- SNS, SQS (messages)

### Pricing:
- **Requests**: $0.20 per 1M requests
- **Compute**: $0.0000166667 per GB-second

---

## 3. Amazon ECS (Elastic Container Service)

### Khái niệm
ECS = Fully managed container orchestration service. Chạy Docker containers trên AWS.

### Components:
- **Tasks**: Running containers
- **Task Definitions**: Blueprint for tasks (container image, CPU, memory)
- **Services**: Maintain desired number of tasks
- **Clusters**: Group of EC2 instances hoặc Fargate capacity

### Launch Types:

#### **EC2 Launch Type**
- Chạy containers trên EC2 instances bạn quản lý
- Full control, tự quản lý servers

#### **Fargate Launch Type**
- Serverless compute engine cho containers
- Không cần manage EC2 instances
- Pay cho resources sử dụng
- **Use case**: Không muốn manage infrastructure

### Use Cases:
- Microservices architectures
- Batch processing
- Machine learning workloads

---

## 4. AWS Elastic Beanstalk

### Khái niệm
Elastic Beanstalk = Platform as a Service (PaaS). Bạn upload code, Beanstalk tự động handle deployment, infrastructure.

### Đặc điểm:
- **No infrastructure management** - AWS handles everything
- **Automatic deployment** - từ code repository hoặc upload
- **Auto scaling** - tự động scale based on demand
- **Load balancing** - automatic load balancer
- **Monitoring** - integrated với CloudWatch

### Supported Platforms:
- Java, .NET, Python, Ruby, Go, PHP, Node.js, Docker

### Use Cases:
- Web applications
- APIs
- Background workers

---

## 5. AWS Fargate

### Khái niệm
Fargate = Serverless compute engine cho containers. Chạy containers mà không cần manage EC2 instances.

### Đặc điểm:
- **Serverless** - no servers to manage
- **Pay per task** - chỉ trả cho resources sử dụng
- Dùng với **ECS** hoặc **EKS** (Kubernetes)

---

## 6. So sánh Compute Services

| Service | Control | Management | Use Case |
|---------|---------|------------|----------|
| **EC2** | Full control | You manage OS, apps | Full control needed |
| **Lambda** | Code only | Serverless | Event-driven, short tasks |
| **ECS** | Containers | Container orchestration | Container workloads |
| **Fargate** | Containers | Serverless | Containers without servers |
| **Beanstalk** | Application | PaaS | Deploy code quickly |

---

## 7. Elastic Load Balancer (ELB)

### Khái niệm
ELB = Distribute incoming traffic across multiple targets (EC2 instances, containers, Lambda functions).

### Types:

#### **Application Load Balancer (ALB)**
- Layer 7 (HTTP/HTTPS)
- Content-based routing
- **Use case**: Web applications, microservices

#### **Network Load Balancer (NLB)**
- Layer 4 (TCP/UDP)
- High performance, low latency
- **Use case**: High performance, extreme performance

#### **Classic Load Balancer (CLB)**
- Legacy (không nên dùng cho new applications)
- Layer 4 và Layer 7

### Benefits:
- High availability
- Fault tolerance
- Automatic scaling
- SSL/TLS termination

---

## 📚 Key Concepts Summary

### EC2:
- Virtual servers với full control
- Pricing: On-Demand, Reserved, Spot
- Auto Scaling cho automatic capacity adjustment
- Security Groups = firewall

### Lambda:
- Serverless functions
- Event-driven
- 15-minute timeout
- Pay-per-execution

### ECS:
- Container orchestration
- EC2 launch type hoặc Fargate (serverless)

### Beanstalk:
- PaaS - deploy code, AWS handles infrastructure
- Quick deployment

---

## ✅ Checklist hiểu biết

- [ ] Hiểu EC2 instances, AMIs, instance types
- [ ] Biết các EC2 pricing models và khi nào dùng
- [ ] Hiểu Lambda và use cases
- [ ] Biết ECS, Fargate, Beanstalk
- [ ] Hiểu Auto Scaling và Load Balancing
- [ ] So sánh được các compute services

