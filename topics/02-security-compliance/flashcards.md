# Security & Compliance - Flashcards

---

## Q: IAM là gì?
**A:** Identity and Access Management - quản lý users, groups, roles, permissions

---

## Q: IAM Users vs Roles?
**A:** 
- **Users** = People (long-term credentials)
- **Roles** = AWS services/temporary access (no long-term credentials)

---

## Q: Principle of least privilege?
**A:** Chỉ grant minimum permissions cần thiết để thực hiện task

---

## Q: MFA là gì?
**A:** Multi-Factor Authentication = Password + Device, thêm layer security

---

## Q: Encryption at rest vs in transit?
**A:** 
- **At rest** = Khi data đang stored (S3, EBS, databases)
- **In transit** = Khi data đang transmitted qua network

---

## Q: AWS KMS là gì?
**A:** Key Management Service - quản lý encryption keys

---

## Q: AWS Shield là gì?
**A:** DDoS protection service (Standard = free, Advanced = paid)

---

## Q: AWS WAF là gì?
**A:** Web Application Firewall - bảo vệ web apps từ SQL injection, XSS (Layer 7)

---

## Q: AWS CloudTrail là gì?
**A:** Logging service ghi lại tất cả API calls để audit và compliance

---

## Q: AWS Config là gì?
**A:** Service để record và evaluate resource configurations cho compliance

---

## Q: AWS GuardDuty là gì?
**A:** Threat detection service dùng machine learning để detect malicious activity

---

## Q: AWS Security Hub là gì?
**A:** Centralized security management, aggregates findings từ nhiều security tools

---

## Q: AWS Inspector là gì?
**A:** Automated security assessment cho EC2 instances - vulnerability scanning

---

## Q: AWS Macie là gì?
**A:** Data security service dùng ML để discover, classify, protect sensitive data trong S3

---

## Q: AWS Artifact là gì?
**A:** On-demand access to AWS compliance reports (SOC, PCI, ISO)

---

## Q: Shared Responsibility - AWS chịu trách nhiệm gì?
**A:** Security **OF** the cloud - Infrastructure, hardware, networking, physical security

---

## Q: Shared Responsibility - Customer chịu trách nhiệm gì?
**A:** Security **IN** the cloud - Data, applications, OS (tùy service model), access control

---

## Q: HIPAA là gì?
**A:** Healthcare compliance framework cho Protected Health Information

---

## Q: GDPR là gì?
**A:** European data protection regulation

---

## Q: PCI DSS là gì?
**A:** Payment Card Industry standard cho credit card data security

---

## Q: Root account best practices?
**A:** Enable MFA, chỉ dùng cho account management, daily ops dùng IAM users

---

## Q: Best practice cho programmatic access?
**A:** Dùng IAM roles với temporary credentials, không dùng long-term access keys trong code

---

## Q: IAM Groups dùng để làm gì?
**A:** Manage permissions cho nhiều users cùng lúc - assign permissions to groups

---

## Q: IAM Policies là gì?
**A:** JSON documents định nghĩa permissions, có thể attach vào Users/Groups/Roles/Resources

---

## 🎯 Quick Reference

### IAM Components:
- **Users** = People
- **Groups** = Collections of users
- **Roles** = Services/Temporary access
- **Policies** = Permissions documents

### Security Services:
- **Shield** = DDoS
- **WAF** = Web app protection
- **GuardDuty** = Threat detection
- **Inspector** = Vulnerability scanning
- **Macie** = Sensitive data
- **CloudTrail** = API logging
- **Config** = Compliance tracking
- **Security Hub** = Centralized view

### Encryption:
- **At rest** = When stored
- **In transit** = When transmitted
- **KMS** = Key management

### Compliance:
- **HIPAA** = Healthcare
- **GDPR** = European data
- **PCI DSS** = Payment cards
- **Artifact** = Reports on-demand

