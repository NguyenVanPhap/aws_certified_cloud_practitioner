# Security & Compliance - Exam Style Questions

> 📝 **Format đề thi thật**: Multiple choice và multiple response. Làm như đang thi thật!

---

## Question 1
Which AWS service is used to manage user access and permissions?

A. AWS Config  
B. AWS IAM  
C. AWS CloudTrail  
D. AWS Shield

<details>
<summary><strong>Answer: B - AWS IAM</strong></summary>

**Explanation:** IAM (Identity and Access Management) = quản lý users, groups, roles, permissions. Config = compliance tracking, CloudTrail = logging, Shield = DDoS protection.

**Exam Tip:** IAM là service security quan trọng nhất - xuất hiện nhiều trong exam.
</details>

---

## Question 2
Which of the following are components of AWS IAM? (Select THREE)

A. Users  
B. Groups  
C. Roles  
D. Policies  
E. Buckets

<details>
<summary><strong>Answer: A, B, C</strong></summary>

**Explanation:** IAM components: Users (people), Groups (collections of users), Roles (services/temporary access), Policies (permissions documents). Buckets = S3, không phải IAM.

**Exam Tip:** IAM có 4 components chính: Users, Groups, Roles, Policies. Nhớ cả 4.
</details>

---

## Question 3
What is the principle of least privilege?

A. Granting maximum permissions to all users  
B. Granting only the minimum permissions necessary to perform a task  
C. Removing all permissions  
D. Sharing credentials between users

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Principle of least privilege = security best practice, chỉ grant minimum permissions cần thiết. Giảm risk nếu credentials bị compromise.

**Exam Tip:** Least privilege = Security best practice, xuất hiện nhiều trong exam.
</details>

---

## Question 4
Which AWS service provides protection against DDoS attacks?

A. AWS WAF  
B. AWS Shield  
C. AWS GuardDuty  
D. AWS Macie

<details>
<summary><strong>Answer: B - AWS Shield</strong></summary>

**Explanation:** Shield = DDoS protection (Standard = free, Advanced = paid). WAF = Web Application Firewall (layer 7), GuardDuty = threat detection, Macie = sensitive data protection.

**Exam Tip:** Shield = DDoS. WAF = Web app exploits. GuardDuty = Threats. Macie = Data.
</details>

---

## Question 5
What does MFA stand for and what does it provide?

A. Multiple File Access; enables file sharing  
B. Multi-Factor Authentication; provides an additional layer of security  
C. Maximum File Allocation; limits storage  
D. Manual File Access; requires manual approval

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** MFA = Multi-Factor Authentication = something you know (password) + something you have (device). Thêm layer security, recommended cho root account và privileged users.

**Exam Tip:** MFA = Password + Device, là best practice bắt buộc cho root account.
</details>

---

## Question 6
Which AWS service provides logging and monitoring of API calls made to AWS services?

A. AWS CloudWatch  
B. AWS CloudTrail  
C. AWS Config  
D. AWS X-Ray

<details>
<summary><strong>Answer: B - AWS CloudTrail</strong></summary>

**Explanation:** CloudTrail = logging service ghi lại tất cả API calls. CloudWatch = monitoring metrics, Config = resource configuration tracking, X-Ray = application tracing.

**Exam Tip:** CloudTrail = API logging. CloudWatch = Metrics. Config = Compliance.
</details>

---

## Question 7
What is AWS KMS used for?

A. Key Migration Service  
B. Key Management Service - manages encryption keys  
C. Key Monitoring Service  
D. Key Maintenance Service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** KMS = Key Management Service để tạo, quản lý, control encryption keys. Dùng để encrypt data at rest trong S3, EBS, RDS. Fully managed.

**Exam Tip:** KMS = Encryption key management, xuất hiện trong questions về encryption.
</details>

---

## Question 8
Which AWS service helps protect web applications from common web exploits such as SQL injection and XSS?

A. AWS Shield  
B. AWS WAF  
C. AWS GuardDuty  
D. AWS Security Hub

<details>
<summary><strong>Answer: B - AWS WAF</strong></summary>

**Explanation:** WAF (Web Application Firewall) = bảo vệ web apps từ SQL injection, XSS, và common exploits. Layer 7 protection. Tích hợp với CloudFront và ALB.

**Exam Tip:** WAF = Web app protection (Layer 7). Shield = Network layer (DDoS).
</details>

---

## Question 9
What is the difference between encryption at rest and encryption in transit?

A. At rest encrypts data during transmission, in transit encrypts stored data  
B. At rest encrypts stored data, in transit encrypts data during transmission  
C. They are the same  
D. At rest is for databases, in transit is for files

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Encryption at rest = mã hóa data khi stored (S3, EBS, databases). Encryption in transit = mã hóa data khi transmitted qua network (HTTPS, TLS).

**Exam Tip:** At rest = When stored | In transit = When transmitted. Cả hai đều quan trọng!
</details>

---

## Question 10
Which statement about AWS Shared Responsibility Model is correct?

A. AWS is responsible for securing customer data  
B. Customer is responsible for physical security of data centers  
C. AWS is responsible for security OF the cloud, customer is responsible for security IN the cloud  
D. AWS and customer share equal responsibility for all security aspects

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** AWS = Security OF cloud (infrastructure, hardware, physical). Customer = Security IN cloud (data, apps, OS - tùy service model). Customer data luôn là responsibility của customer.

**Exam Tip:** Shared Responsibility = AWS: OF cloud | Customer: IN cloud. Rất quan trọng!
</details>

---

## Question 11
Which IAM component allows you to grant permissions to AWS services such as EC2 instances?

A. Users  
B. Groups  
C. Roles  
D. Policies

<details>
<summary><strong>Answer: C - Roles</strong></summary>

**Explanation:** IAM Roles = dùng để grant permissions cho AWS services (EC2, Lambda). Services assume roles để có permissions. Users = people, Groups = collections of users, Policies = permissions documents.

**Exam Tip:** Roles = For AWS services. Users = For people.
</details>

---

## Question 12
What is the difference between IAM Users and IAM Roles?

A. Users are for people, Roles are for AWS services  
B. Users are for AWS services, Roles are for people  
C. They are the same thing  
D. Users are temporary, Roles are permanent

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** Users = people với long-term credentials. Roles = AWS services hoặc temporary access, no long-term credentials. Best practice: dùng roles cho services.

**Exam Tip:** Users = People | Roles = Services/Temporary. Nhớ phân biệt rõ!
</details>

---

## Question 13
Which AWS service helps you assess security posture and identify security gaps across your AWS accounts?

A. AWS GuardDuty  
B. AWS Security Hub  
C. AWS Inspector  
D. AWS Macie

<details>
<summary><strong>Answer: B - AWS Security Hub</strong></summary>

**Explanation:** Security Hub = centralized security management, aggregates findings từ GuardDuty, Inspector, Macie, third-party tools. Provides overall security posture view.

**Exam Tip:** Security Hub = Centralized security view. Aggregates từ nhiều security tools.
</details>

---

## Question 14
Which compliance framework is related to healthcare data protection in the United States?

A. GDPR  
B. HIPAA  
C. PCI DSS  
D. SOC 2

<details>
<summary><strong>Answer: B - HIPAA</strong></summary>

**Explanation:** HIPAA = Health Insurance Portability and Accountability Act, dùng cho healthcare data (Protected Health Information). GDPR = European data protection, PCI DSS = payment cards, SOC 2 = security audits.

**Exam Tip:** HIPAA = Healthcare (US). GDPR = European. PCI DSS = Payment cards.
</details>

---

## Question 15
What is AWS Config used for?

A. Configuring EC2 instances  
B. Recording and evaluating resource configurations for compliance  
C. Configuring network settings  
D. Configuring databases

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** AWS Config = service để record và evaluate resource configurations. Tracks changes over time, helps với compliance và audit. Không phải để configure services.

**Exam Tip:** Config = Compliance tracking, not configuration tool.
</details>

---

## Question 16
Which best practice should you follow for IAM passwords?

A. Use simple passwords  
B. Enable password policy with complexity requirements  
C. Share passwords between users  
D. Never change passwords

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Best practice = enable password policy với complexity (length, mixed case, numbers, symbols), expiration, prevent reuse. Giảm risk của weak passwords.

**Exam Tip:** Password policy = Security best practice. Complexity + Expiration + Reuse prevention.
</details>

---

## Question 17
What is the purpose of AWS GuardDuty?

A. Managing firewall rules  
B. Threat detection service that monitors for malicious activity  
C. Managing access control  
D. Managing encryption keys

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** GuardDuty = intelligent threat detection, dùng machine learning để detect malicious activity. Monitors CloudTrail logs, VPC Flow Logs, DNS logs.

**Exam Tip:** GuardDuty = ML-based threat detection. Monitors logs.
</details>

---

## Question 18
Which service helps protect sensitive data stored in S3 buckets?

A. AWS Macie  
B. AWS GuardDuty  
C. AWS WAF  
D. AWS Shield

<details>
<summary><strong>Answer: A - AWS Macie</strong></summary>

**Explanation:** Macie = data security service dùng ML để discover, classify, protect sensitive data trong S3. Phát hiện PII, credentials. GuardDuty = threats, WAF = web apps, Shield = DDoS.

**Exam Tip:** Macie = Sensitive data discovery trong S3.
</details>

---

## Question 19
What should you do with root account credentials? (Select TWO)

A. Share them with team members  
B. Enable MFA  
C. Use them for daily operations  
D. Only use for account management tasks  
E. Store them in code

<details>
<summary><strong>Answer: B, D</strong></summary>

**Explanation:** Root account best practices: Enable MFA, chỉ dùng cho account management tasks. Daily operations nên dùng IAM users/roles. Không share, không store trong code.

**Exam Tip:** Root account = Enable MFA, use sparingly. Create IAM users cho daily use.
</details>

---

## Question 20
Which AWS service provides automated security assessment for EC2 instances?

A. AWS Inspector  
B. AWS Security Hub  
C. AWS GuardDuty  
D. AWS Macie

<details>
<summary><strong>Answer: A - AWS Inspector</strong></summary>

**Explanation:** Inspector = automated security assessment cho EC2 instances. Scans cho vulnerabilities, network exposure, best practice deviations. Security Hub = aggregates findings, GuardDuty = threats, Macie = data.

**Exam Tip:** Inspector = EC2 vulnerability scanning. Automated security assessment.
</details>

---

## Question 21
What is the recommended way to access AWS resources programmatically?

A. Root account credentials  
B. IAM user access keys stored in code  
C. IAM roles with temporary credentials  
D. Shared credentials file

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Best practice = dùng IAM roles với temporary credentials (STS). Không nên dùng long-term access keys trong code. Roles provide temporary credentials automatically.

**Exam Tip:** Programmatic access = Use IAM roles (temporary credentials), not long-term keys.
</details>

---

## Question 22
Which of the following are security best practices? (Select THREE)

A. Enable MFA for root account  
B. Use principle of least privilege  
C. Share credentials between team members  
D. Encrypt data at rest and in transit  
E. Use simple passwords

<details>
<summary><strong>Answer: A, B, D</strong></summary>

**Explanation:** Security best practices: Enable MFA, least privilege, encryption. Sharing credentials và simple passwords là BAD practices, không phải best practices.

**Exam Tip:** Best practices: MFA, least privilege, encryption, regular audits.
</details>

---

## 📊 Exam Simulation

Làm 22 câu trong **33 phút** (1.5 phút/câu):
- **18-22 đúng**: ✅ Excellent, ready!
- **15-17 đúng**: ✅ Good, review weak areas
- **Dưới 15 đúng**: 📚 Review notes và flashcards

---

## 💡 Exam Tips

1. **Security services**: IAM, CloudTrail, Config, Shield, WAF, GuardDuty, Macie, Security Hub, Inspector
2. **Shared Responsibility**: AWS = OF cloud, Customer = IN cloud
3. **IAM**: Users (people), Roles (services), Groups, Policies
4. **Encryption**: At rest (stored) vs In transit (transmitted)
5. **Best practices**: MFA, least privilege, encryption, roles cho services

---

## 🔄 Review Schedule

- **Lần 1**: Sau khi học notes
- **Lần 2**: Sau 2 ngày
- **Lần 3**: Sau 5 ngày
- **Lần 4**: 1 tuần trước khi thi

Mục tiêu: 100% trong lần cuối!

