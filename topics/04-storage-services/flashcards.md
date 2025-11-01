# Storage Services - Flashcards

---

## Q: S3 là gì?
**A:** Simple Storage Service - Object storage, unlimited scalability

---

## Q: S3 durability?
**A:** 99.999999999% (11 nines)

---

## Q: S3 object max size?
**A:** 5TB (dùng multipart upload cho files lớn)

---

## Q: S3 Storage Classes?
**A:** 
- **Standard** = Frequent access
- **Standard-IA** = Infrequent access
- **One Zone-IA** = Single AZ, infrequent
- **Glacier** = Archive (retrieval 1-12 hours)

---

## Q: Glacier dùng để làm gì?
**A:** Long-term archival storage, retrieval 1-12 hours, cheapest

---

## Q: S3 Lifecycle Policies?
**A:** Automatically transition/delete objects dựa trên age

---

## Q: S3 Versioning?
**A:** Keep multiple versions của objects, restore previous versions

---

## Q: S3 Cross-Region Replication?
**A:** Automatically replicate objects sang region khác

---

## Q: EBS là gì?
**A:** Elastic Block Store - Persistent block storage cho EC2

---

## Q: EBS volume types?
**A:** 
- **gp2/gp3** = General purpose
- **io1/io2** = Highest IOPS (databases)
- **st1** = Throughput optimized
- **sc1** = Cold HDD

---

## Q: EBS Snapshots?
**A:** Point-in-time backups của EBS volumes, incremental, stored on S3

---

## Q: EFS là gì?
**A:** Elastic File System - File storage, shared across multiple EC2 instances

---

## Q: S3 vs EBS vs EFS?
**A:** 
- **S3** = Object storage (internet-accessible)
- **EBS** = Block storage (attached to EC2)
- **EFS** = File storage (shared, NFS)

---

## Q: Instance Store?
**A:** Ephemeral block storage, lost khi instance stop/terminate

---

## Q: S3 Static Website Hosting?
**A:** Host static websites (HTML, CSS, JS) trên S3

---

## 🎯 Quick Reference

### S3:
- **Object storage** = Unlimited, 11 nines durability
- **Classes** = Cost optimization
- **Lifecycle** = Auto management
- **Versioning** = Multiple versions

### EBS:
- **Block storage** = EC2 volumes
- **Persistent** = Survive instance termination
- **Snapshots** = Backups

### EFS:
- **File storage** = Shared, NFS interface

