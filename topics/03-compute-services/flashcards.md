# Compute Services - Flashcards

---

## Q: EC2 là gì?
**A:** Elastic Compute Cloud - Virtual servers trong cloud

---

## Q: Lambda là gì?
**A:** Serverless compute service - viết code, AWS quản lý servers

---

## Q: AMI là gì?
**A:** Amazon Machine Image - template cho EC2 instances (OS + apps)

---

## Q: EC2 On-Demand Instances?
**A:** Pay per-second, no commitment, most flexible, highest cost

---

## Q: EC2 Reserved Instances?
**A:** 1-3 year commitment, discount up to 72%, cho steady-state workloads

---

## Q: EC2 Spot Instances?
**A:** Dùng unused capacity, discount up to 90%, can be terminated với 2-min warning

---

## Q: EC2 Auto Scaling?
**A:** Tự động adjust số lượng instances dựa trên demand (CPU, network, custom metrics)

---

## Q: Security Groups là gì?
**A:** Virtual firewall cho EC2 - control inbound/outbound traffic, stateful

---

## Q: Instance Store vs EBS?
**A:** 
- **Instance Store** = Ephemeral (mất khi stop/terminate), nhanh
- **EBS** = Persistent, data tồn tại độc lập

---

## Q: Lambda timeout?
**A:** Maximum 15 minutes per execution

---

## Q: Lambda use cases?
**A:** Event-driven apps, API backends, data processing, scheduled tasks

---

## Q: ECS là gì?
**A:** Elastic Container Service - container orchestration service

---

## Q: ECS Launch Types?
**A:** 
- **EC2** = Containers trên EC2 bạn quản lý
- **Fargate** = Serverless containers

---

## Q: Fargate là gì?
**A:** Serverless compute engine cho containers, không cần manage EC2

---

## Q: Elastic Beanstalk là gì?
**A:** PaaS - upload code, AWS handles deployment, infrastructure, scaling

---

## Q: ELB là gì?
**A:** Elastic Load Balancer - distribute traffic across multiple targets

---

## Q: ALB vs NLB?
**A:** 
- **ALB** = Layer 7 (HTTP/HTTPS), content-based routing
- **NLB** = Layer 4 (TCP/UDP), high performance

---

## Q: EC2 instance families?
**A:** 
- **T** = Burstable
- **M** = General purpose
- **C** = Compute-optimized
- **R** = Memory-optimized

---

## Q: Lambda triggers?
**A:** API Gateway, S3, CloudWatch Events, DynamoDB streams, Kinesis, SNS, SQS

---

## Q: When to use EC2 vs Lambda?
**A:** 
- **EC2** = Full control, long-running, predictable workloads
- **Lambda** = Event-driven, short tasks, no server management

---

## 🎯 Quick Reference

### EC2:
- **On-Demand** = Flexible, no commitment
- **Reserved** = Cheap với commitment
- **Spot** = Cheapest, interruptible
- **Auto Scaling** = Automatic capacity

### Serverless:
- **Lambda** = Functions
- **Fargate** = Containers

### Containers:
- **ECS** = Orchestration
- **Fargate** = Serverless option

### PaaS:
- **Beanstalk** = Deploy code quickly

