# Storage Services - Tóm tắt kiến thức

## 1. Amazon S3 (Simple Storage Service)

### Khái niệm
S3 = Object storage service, store và retrieve any amount of data từ anywhere. Unlimited scalability.

### Đặc điểm:
- **Object storage**: Files stored as objects với metadata
- **99.999999999% (11 nines) durability**
- **99.99% availability** (Standard)
- **Unlimited storage**
- **Object size**: Max 5TB (multipart upload cho files lớn)
- **Buckets**: Containers cho objects, global unique name

### S3 Storage Classes:

#### **S3 Standard**
- Frequent access
- 99.99% availability
- Dùng cho: Production workloads, active data

#### **S3 Standard-IA (Infrequent Access)**
- Infrequent access
- Lower storage cost, retrieval fee
- 99.9% availability
- Dùng cho: Backups, disaster recovery

#### **S3 One Zone-IA**
- Infrequent access, single AZ
- Cheapest (trong IA classes)
- Lower durability (single AZ)
- Dùng cho: Secondary backups có backup ở nơi khác

#### **S3 Glacier**
- Archival storage
- Retrieval: 1-5 minutes (Expedited), 3-5 hours (Standard), 5-12 hours (Bulk)
- Cheapest storage
- Dùng cho: Long-term archives, compliance

#### **S3 Glacier Deep Archive**
- Longest-term archival
- Retrieval: 12 hours
- Lowest cost
- Dùng cho: Data rarely accessed, 7-10 year retention

### S3 Features:

#### **Versioning**
- Keep multiple versions của objects
- Restore previous versions
- Dùng cho: Backup và recovery

#### **Lifecycle Policies**
- Automatically transition objects giữa storage classes
- Automatically delete objects
- Dựa trên age hoặc prefix

#### **Cross-Region Replication**
- Automatically replicate objects sang region khác
- Dùng cho: Disaster recovery, compliance, latency reduction

#### **Static Website Hosting**
- Host static websites trên S3
- Combine với CloudFront cho performance

#### **Encryption**
- SSE-S3: AWS-managed keys
- SSE-KMS: Customer-managed keys
- SSE-C: Customer-provided keys

---

## 2. Amazon EBS (Elastic Block Store)

### Khái niệm
EBS = Persistent block storage volumes cho EC2 instances.

### Đặc điểm:
- **Block storage**: Raw storage blocks
- **Persistent**: Data persists independently của instance lifecycle
- **Attach/detach**: Có thể attach/detach volumes
- **Snapshots**: Point-in-time backups (incremental, stored on S3)

### EBS Volume Types:

#### **gp2 (General Purpose SSD)**
- Balanced price/performance
- Baseline 3 IOPS/GB, burst up to 3000 IOPS
- Dùng cho: Most workloads

#### **gp3 (General Purpose SSD)**
- Next generation gp2
- Baseline 3000 IOPS, can provision up to 16,000 IOPS
- 20% cheaper than gp2

#### **io1/io2 (Provisioned IOPS SSD)**
- Highest IOPS (up to 64,000 IOPS)
- Dùng cho: I/O-intensive workloads (databases)

#### **st1 (Throughput Optimized HDD)**
- High throughput, low IOPS
- Dùng cho: Big data, data warehouses

#### **sc1 (Cold HDD)**
- Lowest cost HDD
- Dùng cho: Infrequently accessed data

### EBS Snapshots:
- Incremental backups (chỉ changed blocks)
- Stored on S3
- Copy across regions
- Create volumes từ snapshots

---

## 3. Amazon EFS (Elastic File System)

### Khái niệm
EFS = Fully managed file system với NFS interface.

### Đặc điểm:
- **File storage**: File system interface
- **Shared storage**: Multiple EC2 instances mount cùng một EFS
- **Scalable**: Automatically scale
- **NFS**: Standard Network File System protocol
- **Use cases**: Shared storage, content management, web serving

### Performance Modes:
- **General Purpose**: Low latency
- **Max I/O**: High throughput

---

## 4. So sánh Storage Services

| Service | Type | Use Case | Access |
|---------|------|----------|--------|
| **S3** | Object | Files, backups, static websites | Internet (API) |
| **EBS** | Block | EC2 volumes | Attached to EC2 |
| **EFS** | File | Shared file storage | Mount to EC2 (NFS) |
| **Instance Store** | Block | Temporary storage | Ephemeral (lost on stop) |

---

## 📚 Key Concepts

- **S3** = Object storage, unlimited, 11 nines durability
- **Storage classes** = Cost optimization based on access
- **EBS** = Block storage cho EC2, persistent
- **EFS** = File storage, shared across instances
- **Lifecycle policies** = Automatic management
- **Versioning** = Multiple versions
- **Snapshots** = EBS backups

---

## ✅ Checklist

- [ ] Hiểu S3 storage classes và khi nào dùng
- [ ] Biết S3 features: versioning, lifecycle, replication
- [ ] Hiểu EBS volume types
- [ ] Biết EFS và use cases
- [ ] So sánh được S3, EBS, EFS

