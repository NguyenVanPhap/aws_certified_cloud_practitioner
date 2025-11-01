# Storage Services - Practice Questions

> 💡 **Cách học**: Tự trả lời trước, đọc kỹ giải thích. Hiểu use cases và storage classes.

---

## Question 1
**What is Amazon S3?**

A. A compute service  
B. An object storage service  
C. A database service  
D. A networking service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** S3 (Simple Storage Service) = object storage service. Store và retrieve any amount of data từ anywhere. Unlimited scalability, 99.999999999% (11 nines) durability.

**Key Concept:** S3 = Object storage, unlimited scalability
</details>

---

## Question 2
**What are S3 storage classes used for?**

A. To organize files  
B. To optimize costs based on access patterns  
C. To improve security  
D. To increase speed

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** S3 storage classes = optimize costs dựa trên access patterns. Frequent access → Standard, infrequent → Standard-IA, archive → Glacier. Chọn class phù hợp để giảm cost.

**Key Concept:** Storage classes = Cost optimization based on access frequency
</details>

---

## Question 3
**Which S3 storage class is designed for long-term archival storage with retrieval times of minutes to hours?**

A. S3 Standard  
B. S3 Standard-IA  
C. S3 One Zone-IA  
D. Amazon Glacier

<details>
<summary><strong>Answer: D</strong></summary>

**Explanation:** Glacier = archival storage với retrieval times minutes to hours. Cheapest storage, dùng cho long-term backups, archives. Standard-IA = infrequent access nhưng instant retrieval.

**Key Concept:** Glacier = Archive storage, slower retrieval
</details>

---

## Question 4
**What is the durability of Amazon S3 Standard?**

A. 99.9%  
B. 99.99%  
C. 99.999999999% (11 nines)  
D. 100%

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** S3 Standard có 99.999999999% (11 nines) durability - có nghĩa là 0.000000001% chance mất data. Extremely durable, data được replicate across multiple AZs.

**Key Concept:** S3 Standard = 11 nines durability
</details>

---

## Question 5
**What is EBS used for?**

A. Object storage  
B. Block storage for EC2 instances  
C. File storage  
D. Database storage

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** EBS (Elastic Block Store) = persistent block storage volumes cho EC2 instances. Attach/detach volumes, data persists independently of instance lifecycle.

**Key Concept:** EBS = Block storage for EC2, persistent
</details>

---

## Question 6
**Which storage service provides a file system interface for use with EC2 instances?**

A. S3  
B. EBS  
C. EFS  
D. Glacier

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** EFS (Elastic File System) = fully managed file system với NFS interface. Multiple EC2 instances có thể mount cùng một EFS file system. Dùng cho shared storage.

**Key Concept:** EFS = File system, shared across multiple instances
</details>

---

## Question 7
**What is the main difference between S3 and EBS?**

A. S3 is for databases, EBS is for files  
B. S3 is object storage, EBS is block storage  
C. They are the same  
D. S3 is for backups, EBS is for applications

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** S3 = object storage (store files as objects với metadata). EBS = block storage (raw storage blocks, như hard drive). S3 = internet-accessible, EBS = attached to EC2.

**Key Concept:** S3 = Object storage | EBS = Block storage
</details>

---

## Question 8
**What happens to S3 objects with lifecycle policies when they transition to Glacier?**

A. They are deleted  
B. They are moved to Glacier storage class  
C. They are copied to Glacier  
D. Nothing happens

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Lifecycle policies = automatically transition objects giữa storage classes dựa trên age. Ví dụ: sau 30 ngày → Standard-IA, sau 90 ngày → Glacier. Objects được moved (không copy).

**Key Concept:** Lifecycle policies = Automatic transition between storage classes
</details>

---

## Question 9
**Which S3 feature allows you to host a static website?**

A. S3 Transfer Acceleration  
B. S3 Static Website Hosting  
C. S3 Cross-Region Replication  
D. S3 Versioning

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** S3 Static Website Hosting = host static websites (HTML, CSS, JS, images) trên S3. Không hỗ trợ server-side code (PHP, Python). Combine với CloudFront cho better performance.

**Key Concept:** S3 = Static website hosting
</details>

---

## Question 10
**What is S3 Versioning?**

A. A way to organize files  
B. A feature that keeps multiple versions of objects  
C. A way to improve speed  
D. A security feature

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Versioning = keep multiple versions của cùng một object. Khi update/delete object, old versions được giữ lại. Hữu ích cho backup và recovery. Có thể restore previous versions.

**Key Concept:** Versioning = Multiple versions of objects
</details>

---

## Question 11
**Which EBS volume type provides the highest IOPS?**

A. gp2 (General Purpose SSD)  
B. io1 (Provisioned IOPS SSD)  
C. st1 (Throughput Optimized HDD)  
D. sc1 (Cold HDD)

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** io1 (Provisioned IOPS SSD) = highest IOPS, cho I/O-intensive workloads (databases). gp2 = general purpose, st1/sc1 = HDD volumes cho throughput/cold data.

**Key Concept:** io1 = Highest IOPS, gp2 = General purpose, st1/sc1 = HDD
</details>

---

## Question 12
**What is S3 Cross-Region Replication used for?**

A. To reduce costs  
B. To automatically replicate objects to another region  
C. To improve speed  
D. To organize files

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Cross-Region Replication = automatically replicate objects từ source bucket sang destination bucket ở region khác. Dùng cho disaster recovery, compliance, reduce latency.

**Key Concept:** Cross-Region Replication = Automatic replication to another region
</details>

---

## Question 13
**Which storage service is best for shared file storage across multiple EC2 instances?**

A. S3  
B. EBS  
C. EFS  
D. Instance Store

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** EFS = fully managed file system, multiple EC2 instances có thể mount cùng một EFS. Shared storage cho applications cần access cùng files. S3 = object storage, EBS = attached to one instance.

**Key Concept:** EFS = Shared file system across multiple instances
</details>

---

## Question 14
**What is the main advantage of S3 Standard-IA over S3 Standard?**

A. Higher durability  
B. Lower cost for infrequently accessed data  
C. Faster retrieval  
D. Better security

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Standard-IA (Infrequent Access) = cheaper storage cho data ít access. Retrieval fee khi access, nhưng storage cost thấp hơn Standard. Dùng cho backups, long-term storage.

**Key Concept:** Standard-IA = Cheaper for infrequent access
</details>

---

## Question 15
**What is an S3 bucket?**

A. A container for objects  
B. A type of storage class  
C. A security feature  
D. A backup service

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** S3 bucket = container cho objects (files). Global unique name, store unlimited objects. Có thể configure versioning, lifecycle, encryption, access control.

**Key Concept:** Bucket = Container for S3 objects
</details>

---

## Question 16
**Which S3 storage class offers the same durability as Standard but stores data in a single Availability Zone?**

A. Standard-IA  
B. One Zone-IA  
C. Glacier  
D. Reduced Redundancy Storage

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** One Zone-IA = infrequent access nhưng data stored trong single AZ (thay vì multiple AZs như Standard-IA). Cheaper nhưng lower durability. Phù hợp cho data có backup ở nơi khác.

**Key Concept:** One Zone-IA = Single AZ, cheaper, lower durability
</details>

---

## Question 17
**What is EBS snapshot used for?**

A. To increase storage  
B. To create backups of EBS volumes  
C. To improve speed  
D. To organize volumes

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** EBS snapshots = point-in-time backups của EBS volumes. Incremental (chỉ backup changed blocks), stored trên S3. Có thể restore volumes từ snapshots, copy snapshots across regions.

**Key Concept:** Snapshots = Point-in-time backups of EBS volumes
</details>

---

## Question 18
**Which statement about S3 is correct?**

A. S3 objects have unlimited size  
B. S3 objects have a maximum size of 5TB  
C. S3 objects have a maximum size of 500GB  
D. S3 objects have a maximum size of 50GB

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** S3 objects có maximum size 5TB. Cho files lớn hơn, dùng multipart upload. S3 buckets có unlimited capacity, nhưng individual object max 5TB.

**Key Concept:** S3 object max size = 5TB
</details>

---

## Question 19
**What is the difference between S3 and EFS?**

A. S3 is block storage, EFS is object storage  
B. S3 is object storage, EFS is file storage  
C. They are the same  
D. S3 is for databases, EFS is for files

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** S3 = object storage (store files as objects, access qua API). EFS = file storage (file system interface, mount như NFS). S3 = internet-accessible, EFS = mount to EC2 instances.

**Key Concept:** S3 = Object storage | EFS = File storage
</details>

---

## Question 20
**Which feature allows you to automatically delete S3 objects after a certain period?**

A. Lifecycle policies  
B. Versioning  
C. Cross-Region Replication  
D. Transfer Acceleration

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** Lifecycle policies = automatically transition hoặc delete objects dựa trên age. Ví dụ: delete objects sau 365 ngày. Giúp tự động quản lý objects và giảm costs.

**Key Concept:** Lifecycle policies = Automatic deletion/transition based on age
</details>

---

## 📊 Tự đánh giá

- **18-20 câu đúng**: ✅ Excellent!
- **15-17 câu đúng**: ✅ Good!
- **Dưới 15 câu**: 📚 Review notes.md

---

## 💡 Tips

1. S3 = Object storage (unlimited, internet-accessible)
2. EBS = Block storage (EC2 volumes, persistent)
3. EFS = File storage (shared, NFS interface)
4. Storage classes = Cost optimization
5. Lifecycle policies = Automatic management

