# Storage Services - Exam Style Questions

---

## Question 1
What is Amazon S3?

A. A compute service  
B. An object storage service  
C. A database service  
D. A networking service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** S3 = Simple Storage Service = object storage. Store và retrieve any amount of data. Unlimited scalability, 99.999999999% durability.

**Exam Tip:** S3 = Object storage, unlimited.
</details>

---

## Question 2
What are S3 storage classes used for?

A. To organize files  
B. To optimize costs based on access patterns  
C. To improve security  
D. To increase speed

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Storage classes = optimize costs dựa trên access frequency. Frequent → Standard, infrequent → Standard-IA, archive → Glacier.

**Exam Tip:** Storage classes = Cost optimization based on access patterns.
</details>

---

## Question 3
Which S3 storage class is designed for long-term archival storage with retrieval times of minutes to hours?

A. S3 Standard  
B. S3 Standard-IA  
C. S3 One Zone-IA  
D. Amazon Glacier

<details>
<summary><strong>Answer: D</strong></summary>

**Explanation:** Glacier = archival với retrieval 1-12 hours. Cheapest storage. Standard-IA = infrequent nhưng instant retrieval.

**Exam Tip:** Glacier = Archive, slower retrieval, cheapest.
</details>

---

## Question 4
What is the durability of Amazon S3 Standard?

A. 99.9%  
B. 99.99%  
C. 99.999999999% (11 nines)  
D. 100%

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** S3 Standard = 11 nines durability (99.999999999%). Extremely durable, data replicated across multiple AZs.

**Exam Tip:** S3 Standard = 11 nines durability (rất quan trọng trong exam!).
</details>

---

## Question 5
What is EBS used for?

A. Object storage  
B. Block storage for EC2 instances  
C. File storage  
D. Database storage

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** EBS = Elastic Block Store = persistent block storage volumes cho EC2. Attach/detach volumes, data persists independently.

**Exam Tip:** EBS = Block storage for EC2, persistent.
</details>

---

## Question 6
Which storage service provides a file system interface for use with EC2 instances?

A. S3  
B. EBS  
C. EFS  
D. Glacier

<details>
<summary><strong>Answer: C - EFS</strong></summary>

**Explanation:** EFS = Elastic File System = file system với NFS interface. Multiple EC2 instances có thể mount cùng một EFS. Shared storage.

**Exam Tip:** EFS = File storage, shared across instances.
</details>

---

## Question 7
What is the main difference between S3 and EBS?

A. S3 is for databases, EBS is for files  
B. S3 is object storage, EBS is block storage  
C. They are the same  
D. S3 is for backups, EBS is for applications

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** S3 = object storage (files as objects với metadata). EBS = block storage (raw blocks, như hard drive). S3 = internet-accessible, EBS = attached to EC2.

**Exam Tip:** S3 = Object | EBS = Block | EFS = File
</details>

---

## Question 8
What happens to S3 objects with lifecycle policies when they transition to Glacier?

A. They are deleted  
B. They are moved to Glacier storage class  
C. They are copied to Glacier  
D. Nothing happens

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Lifecycle policies = automatically transition objects giữa storage classes dựa trên age. Objects được moved (không copy).

**Exam Tip:** Lifecycle policies = Automatic transition/delete based on age.
</details>

---

## Question 9
Which S3 feature allows you to host a static website?

A. S3 Transfer Acceleration  
B. S3 Static Website Hosting  
C. S3 Cross-Region Replication  
D. S3 Versioning

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** S3 Static Website Hosting = host static websites (HTML, CSS, JS). Không hỗ trợ server-side code.

**Exam Tip:** S3 = Static websites only.
</details>

---

## Question 10
What is S3 Versioning?

A. A way to organize files  
B. A feature that keeps multiple versions of objects  
C. A way to improve speed  
D. A security feature

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Versioning = keep multiple versions của cùng object. Khi update/delete, old versions được giữ lại. Restore previous versions.

**Exam Tip:** Versioning = Multiple versions, restore capability.
</details>

---

## Question 11
Which EBS volume type provides the highest IOPS?

A. gp2 (General Purpose SSD)  
B. io1 (Provisioned IOPS SSD)  
C. st1 (Throughput Optimized HDD)  
D. sc1 (Cold HDD)

<details>
<summary><strong>Answer: B - io1</strong></summary>

**Explanation:** io1 = highest IOPS (up to 64,000) cho I/O-intensive workloads (databases). gp2 = general purpose, st1/sc1 = HDD.

**Exam Tip:** io1 = Highest IOPS, cho databases.
</details>

---

## Question 12
What is S3 Cross-Region Replication used for?

A. To reduce costs  
B. To automatically replicate objects to another region  
C. To improve speed  
D. To organize files

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Cross-Region Replication = automatically replicate objects từ source bucket sang destination bucket ở region khác. Disaster recovery, compliance.

**Exam Tip:** Cross-Region Replication = Disaster recovery, compliance.
</details>

---

## Question 13
Which storage service is best for shared file storage across multiple EC2 instances?

A. S3  
B. EBS  
C. EFS  
D. Instance Store

<details>
<summary><strong>Answer: C - EFS</strong></summary>

**Explanation:** EFS = file system, multiple EC2 instances mount cùng một EFS. Shared storage. S3 = object, EBS = one instance.

**Exam Tip:** Shared storage = EFS.
</details>

---

## Question 14
Which statement about S3 is correct?

A. S3 objects have unlimited size  
B. S3 objects have a maximum size of 5TB  
C. S3 objects have a maximum size of 500GB  
D. S3 objects have a maximum size of 50GB

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** S3 objects = maximum 5TB. Cho files lớn hơn, dùng multipart upload. Buckets = unlimited capacity.

**Exam Tip:** S3 object max = 5TB (important!).
</details>

---

## Question 15
What is EBS snapshot used for?

A. To increase storage  
B. To create backups of EBS volumes  
C. To improve speed  
D. To organize volumes

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** EBS snapshots = point-in-time backups của EBS volumes. Incremental (chỉ changed blocks), stored on S3. Restore volumes từ snapshots.

**Exam Tip:** Snapshots = Point-in-time backups, incremental.
</details>

---

## 📊 Exam Simulation

Làm 15 câu trong **23 phút**:
- **14-15 đúng**: ✅ Excellent!
- **12-13 đúng**: ✅ Good!
- **Dưới 12 đúng**: 📚 Review

---

## 💡 Exam Tips

1. **S3** = Object storage, 11 nines durability, max 5TB per object
2. **Storage classes** = Cost optimization (Standard, Standard-IA, Glacier)
3. **EBS** = Block storage, persistent, cho EC2
4. **EFS** = File storage, shared, NFS interface
5. **Lifecycle policies** = Automatic management

---

## 🔄 Review Schedule

- Lần 1: Sau notes
- Lần 2: Sau 2 ngày
- Lần 3: Sau 5 ngày
- Lần 4: 1 tuần trước thi

Mục tiêu: 100%!

