# Security & Compliance - Practice Questions

> 💡 **Cách học**: Tự trả lời trước khi xem đáp án. Đọc kỹ giải thích về security best practices.

---

## Question 1
**Which AWS service allows you to manage user access and permissions?**

A. AWS Config  
B. AWS IAM  
C. AWS CloudTrail  
D. AWS Shield

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** IAM (Identity and Access Management) là service để quản lý users, groups, roles, và permissions. Config = compliance tracking, CloudTrail = logging, Shield = DDoS protection.

**Key Concept:** IAM = Identity and Access Management
</details>

---

## Question 2
**What is the principle of least privilege?**

A. Granting maximum permissions to all users  
B. Granting only the minimum permissions necessary to perform a task  
C. Removing all permissions  
D. Sharing credentials between users

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Principle of least privilege = chỉ grant minimum permissions cần thiết để thực hiện task. Đây là security best practice để giảm risk nếu credentials bị compromise.

**Key Concept:** Least privilege = Minimum necessary permissions only
</details>

---

## Question 3
**Which AWS service provides protection against DDoS attacks?**

A. AWS WAF  
B. AWS Shield  
C. AWS GuardDuty  
D. AWS Macie

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** AWS Shield = DDoS protection service. Shield Standard (free) và Shield Advanced (paid). WAF = Web Application Firewall (layer 7), GuardDuty = threat detection, Macie = data security.

**Key Concept:** Shield = DDoS protection
</details>

---

## Question 4
**What does MFA stand for and why is it important?**

A. Multi-Factor Authentication; provides an additional layer of security  
B. Multiple File Access; enables file sharing  
C. Maximum File Allocation; limits storage  
D. Manual File Access; requires manual approval

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** MFA = Multi-Factor Authentication = something you know (password) + something you have (device). Thêm layer security, ngay cả khi password bị lộ, attacker vẫn cần physical device.

**Key Concept:** MFA = Password + Device authentication
</details>

---

## Question 5
**Which AWS service provides logging and monitoring of API calls made to AWS services?**

A. AWS CloudWatch  
B. AWS CloudTrail  
C. AWS Config  
D. AWS X-Ray

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** CloudTrail = logging service ghi lại tất cả API calls tới AWS services. Giúp audit, compliance, security analysis. CloudWatch = monitoring metrics, Config = resource configuration tracking, X-Ray = application tracing.

**Key Concept:** CloudTrail = API call logging
</details>

---

## Question 6
**What is AWS KMS used for?**

A. Key Management Service - manages encryption keys  
B. Key Monitoring Service - monitors key usage  
C. Key Migration Service - migrates keys between regions  
D. Key Maintenance Service - maintains key infrastructure

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** KMS = Key Management Service để tạo, quản lý, và control encryption keys. Dùng để encrypt data at rest trong S3, EBS, RDS, etc. Fully managed service.

**Key Concept:** KMS = Encryption key management
</details>

---

## Question 7
**Which AWS service helps protect web applications from common web exploits?**

A. AWS Shield  
B. AWS WAF  
C. AWS GuardDuty  
D. AWS Security Hub

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** WAF (Web Application Firewall) = bảo vệ web apps khỏi common exploits như SQL injection, XSS. Layer 7 protection, tích hợp với CloudFront và ALB.

**Key Concept:** WAF = Web application protection (Layer 7)
</details>

---

## Question 8
**What is encryption at rest?**

A. Encrypting data while it is being transmitted  
B. Encrypting data when it is stored  
C. Encrypting passwords only  
D. Encrypting network traffic

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Encryption at rest = mã hóa data khi đang stored (trong S3, EBS, database). Khác với encryption in transit = mã hóa khi đang transmitted qua network.

**Key Concept:** At rest = When stored | In transit = When transmitted
</details>

---

## Question 9
**Which statement about AWS Shared Responsibility Model is correct?**

A. AWS is responsible for securing customer data  
B. Customer is responsible for physical security of data centers  
C. AWS is responsible for security OF the cloud, customer is responsible for security IN the cloud  
D. AWS and customer share equal responsibility for all security aspects

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** AWS Shared Responsibility: AWS = security OF cloud (infrastructure), Customer = security IN cloud (data, apps, OS - tùy service model). Customer data luôn là responsibility của customer.

**Key Concept:** AWS = OF cloud | Customer = IN cloud
</details>

---

## Question 10
**What is AWS Artifact?**

A. A service for storing artifacts  
B. A service that provides on-demand access to AWS security and compliance reports  
C. A service for artifact migration  
D. A service for artifact backup

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** AWS Artifact = service cung cấp on-demand access tới AWS security và compliance reports (SOC, PCI, ISO certifications). Giúp customers hiểu AWS compliance posture.

**Key Concept:** Artifact = Compliance reports on-demand
</details>

---

## Question 11
**Which IAM component allows you to grant permissions to AWS services?**

A. Users  
B. Groups  
C. Roles  
D. Policies

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** IAM Roles = dùng để grant permissions cho AWS services (EC2, Lambda, etc.). Services assume roles để có permissions. Users = people, Groups = collections of users, Policies = permissions documents.

**Key Concept:** Roles = Permissions for AWS services
</details>

---

## Question 12
**What is the difference between IAM Users and IAM Roles?**

A. Users are for people, Roles are for AWS services  
B. Users are for AWS services, Roles are for people  
C. They are the same thing  
D. Users are temporary, Roles are permanent

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** IAM Users = cho people (developers, admins) với long-term credentials. IAM Roles = cho AWS services hoặc temporary access, không có long-term credentials.

**Key Concept:** Users = People | Roles = Services/Temporary access
</details>

---

## Question 13
**Which AWS service helps you assess security posture and identify security gaps?**

A. AWS GuardDuty  
B. AWS Security Hub  
C. AWS Inspector  
D. AWS Macie

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Security Hub = centralized security management, aggregates findings từ GuardDuty, Inspector, Macie, và third-party tools. Giúp assess overall security posture.

**Key Concept:** Security Hub = Centralized security management
</details>

---

## Question 14
**What does encryption in transit protect?**

A. Data stored in S3  
B. Data being transmitted over the network  
C. Data in databases  
D. Data in backups

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Encryption in transit = mã hóa data khi đang transmitted qua network (HTTPS, TLS/SSL). Bảo vệ data khỏi man-in-the-middle attacks.

**Key Concept:** In transit = Data traveling over network
</details>

---

## Question 15
**Which compliance framework is related to healthcare data protection?**

A. GDPR  
B. HIPAA  
C. PCI DSS  
D. SOC 2

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** HIPAA = Health Insurance Portability and Accountability Act, dùng cho healthcare data. GDPR = European data protection, PCI DSS = payment card data, SOC 2 = general security audits.

**Key Concept:** HIPAA = Healthcare compliance
</details>

---

## Question 16
**What is AWS Config used for?**

A. Configuring EC2 instances  
B. Recording and evaluating resource configurations for compliance  
C. Configuring network settings  
D. Configuring databases

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** AWS Config = service để record và evaluate resource configurations. Giúp compliance, audit, change management. Tracks changes to resources over time.

**Key Concept:** Config = Configuration compliance tracking
</details>

---

## Question 17
**Which best practice should you follow for IAM passwords?**

A. Use simple passwords  
B. Enable password policy with complexity requirements  
C. Share passwords between users  
D. Never change passwords

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Best practice = enable password policy với complexity requirements (min length, mixed case, numbers, symbols), expiration, prevent reuse. Giảm risk của weak passwords.

**Key Concept:** Password policy = Complexity + Expiration + Reuse prevention
</details>

---

## Question 18
**What is the purpose of AWS GuardDuty?**

A. Managing firewall rules  
B. Threat detection service that monitors for malicious activity  
C. Managing access control  
D. Managing encryption keys

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** GuardDuty = intelligent threat detection service, sử dụng machine learning để detect malicious activity trong AWS accounts. Monitors CloudTrail, VPC Flow Logs, DNS logs.

**Key Concept:** GuardDuty = ML-based threat detection
</details>

---

## Question 19
**Which service helps protect sensitive data stored in S3?**

A. AWS Macie  
B. AWS GuardDuty  
C. AWS WAF  
D. AWS Shield

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** Macie = data security service dùng machine learning để discover, classify, và protect sensitive data trong S3. Phát hiện PII, credentials, etc.

**Key Concept:** Macie = Sensitive data discovery and protection
</details>

---

## Question 20
**What should you do with root account credentials?**

A. Share them with team members  
B. Use them for daily operations  
C. Enable MFA and only use for account management tasks  
D. Store them in code

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Root account = highest privilege, nên enable MFA và chỉ dùng cho account management tasks. Daily operations nên dùng IAM users/roles với least privilege.

**Key Concept:** Root account = Enable MFA, use sparingly, create IAM users for daily use
</details>

---

## Question 21
**Which AWS service provides vulnerability scanning for EC2 instances?**

A. AWS Inspector  
B. AWS Security Hub  
C. AWS GuardDuty  
D. AWS Macie

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** Inspector = automated security assessment service, scans EC2 instances cho vulnerabilities, network exposure, best practice deviations.

**Key Concept:** Inspector = EC2 vulnerability scanning
</details>

---

## Question 22
**What is the recommended way to access AWS resources programmatically?**

A. Root account credentials  
B. IAM user access keys stored in code  
C. IAM roles with temporary credentials  
D. Shared credentials file

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Best practice = dùng IAM roles với temporary credentials (STS). Không nên dùng long-term access keys trong code. Roles provide temporary credentials automatically.

**Key Concept:** Use IAM roles (temporary credentials) for programmatic access
</details>

---

## 📊 Tự đánh giá

- **18-22 câu đúng**: ✅ Excellent! Nắm vững Security & Compliance
- **15-17 câu đúng**: ✅ Good! Ôn lại câu sai
- **Dưới 15 câu**: 📚 Review notes.md và flashcards.md

---

## 💡 Tips

1. Security là rất quan trọng trong AWS exam (18%)
2. Hiểu rõ Shared Responsibility Model
3. Ghi nhớ các services: IAM, CloudTrail, Config, Shield, WAF, KMS
4. Best practices: MFA, least privilege, encryption

