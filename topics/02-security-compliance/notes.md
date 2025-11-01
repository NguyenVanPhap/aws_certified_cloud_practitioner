# Security & Compliance - Tóm tắt kiến thức

## 1. AWS IAM (Identity and Access Management)

### Khái niệm
IAM = service để quản lý users, groups, roles, và permissions trong AWS.

### Các thành phần IAM:

#### **IAM Users**
- Đại diện cho **people** (developers, admins)
- Có **long-term credentials** (username/password, access keys)
- **Use case**: Individual developers, admins

#### **IAM Groups**
- Collection của users
- Dùng để **manage permissions** cho nhiều users cùng lúc
- **Best practice**: Assign permissions to groups, add users to groups

#### **IAM Roles**
- Dùng cho **AWS services** hoặc **temporary access**
- **No long-term credentials**
- Services **assume roles** để có permissions
- **Use case**: EC2 instances, Lambda functions, cross-account access

#### **IAM Policies**
- Documents định nghĩa **permissions**
- JSON format
- Có thể attach vào Users, Groups, Roles, Resources
- **Policy types**:
  - **Managed policies** (AWS managed hoặc Customer managed)
  - **Inline policies** (attach trực tiếp)

### Best Practices IAM:

1. **Principle of Least Privilege**
   - Chỉ grant minimum permissions cần thiết

2. **Enable MFA** (Multi-Factor Authentication)
   - Thêm layer security
   - Bắt buộc cho root account và privileged users

3. **Use Roles instead of Users for AWS services**
   - Roles có temporary credentials
   - Không có long-term credentials risk

4. **Regular credential rotation**
   - Thay đổi passwords và access keys định kỳ

5. **Password policy**
   - Minimum length, complexity
   - Expiration, prevent reuse

6. **Root account**
   - Enable MFA
   - Chỉ dùng cho account management
   - Daily operations dùng IAM users

---

## 2. Encryption

### Encryption at Rest
- **Định nghĩa**: Mã hóa data khi đang **stored** (S3, EBS, databases)
- **Services**: 
  - **S3**: Server-side encryption (SSE-S3, SSE-KMS, SSE-C)
  - **EBS**: Encryption khi tạo volume
  - **RDS**: Encryption at rest với KMS
- **AWS KMS**: Service để manage encryption keys

### Encryption in Transit
- **Định nghĩa**: Mã hóa data khi đang **transmitted** qua network
- **Protocols**: HTTPS, TLS/SSL
- **Use case**: Client ↔ AWS, services ↔ services

### AWS KMS (Key Management Service)
- **Fully managed** service để tạo, quản lý, control encryption keys
- **Key types**: 
  - **AWS managed keys**: AWS quản lý
  - **Customer managed keys**: Customer quản lý, more control
- **Use cases**: Encrypt S3, EBS, RDS, etc.

---

## 3. Security Services

### AWS Shield
- **Purpose**: **DDoS protection**
- **Types**:
  - **Shield Standard**: Free, automatic protection
  - **Shield Advanced**: Paid, additional features, 24/7 support

### AWS WAF (Web Application Firewall)
- **Purpose**: Protect **web applications** từ common exploits
- **Protection**: SQL injection, XSS, etc.
- **Layer**: Layer 7 (application layer)
- **Integration**: CloudFront, ALB, API Gateway

### AWS CloudTrail
- **Purpose**: **Logging service** ghi lại tất cả API calls
- **Use cases**: 
  - Audit trail
  - Compliance
  - Security analysis
- **Logs**: Who, what, when, where

### AWS Config
- **Purpose**: **Record and evaluate** resource configurations
- **Use cases**:
  - Compliance tracking
  - Change management
  - Audit
- **Tracks**: Configuration changes over time

### AWS GuardDuty
- **Purpose**: **Threat detection** service
- **Method**: Machine learning
- **Monitors**: CloudTrail logs, VPC Flow Logs, DNS logs
- **Detects**: Unusual activity, potential threats

### AWS Security Hub
- **Purpose**: **Centralized security management**
- **Aggregates**: Findings từ GuardDuty, Inspector, Macie, third-party tools
- **Provides**: Overall security posture view

### AWS Inspector
- **Purpose**: **Automated security assessment** cho EC2 instances
- **Scans**: Vulnerabilities, network exposure, best practices
- **Reports**: Security findings with recommendations

### AWS Macie
- **Purpose**: **Data security** - discover, classify, protect sensitive data
- **Focus**: S3 buckets
- **Detects**: PII, credentials, etc.
- **Method**: Machine learning

---

## 4. AWS Shared Responsibility Model

### AWS chịu trách nhiệm: **Security OF the Cloud**

- Infrastructure security (hardware, software, networking)
- Physical security của data centers
- Regions, Availability Zones, Edge locations
- Service availability
- Compliance của infrastructure layer

### Customer chịu trách nhiệm: **Security IN the Cloud**

Tùy service model:

#### **IaaS (EC2)**
- Operating system patches và updates
- Application security
- Network security (security groups, NACLs)
- Data encryption (customer-managed keys)
- Access control

#### **PaaS (RDS, Elastic Beanstalk)**
- Application security
- Data encryption settings
- Access control

#### **SaaS**
- Customer data
- Access control

#### **Always Customer Responsibility:**
- Data
- Access control
- Encryption settings
- Network traffic protection

---

## 5. Compliance

### Compliance Frameworks:

#### **HIPAA** (Health Insurance Portability and Accountability Act)
- **Use case**: Healthcare data
- **Requirements**: Protected Health Information (PHI)

#### **GDPR** (General Data Protection Regulation)
- **Use case**: European data protection
- **Requirements**: Data privacy, right to deletion

#### **PCI DSS** (Payment Card Industry Data Security Standard)
- **Use case**: Payment card data
- **Requirements**: Secure handling of credit card info

#### **SOC 2** (Service Organization Control 2)
- **Use case**: Security audits
- **Requirements**: Security, availability, confidentiality

### AWS Artifact
- **Purpose**: On-demand access to AWS **compliance reports**
- **Contains**: SOC, PCI, ISO certifications
- **Use case**: Customers cần proof AWS compliance posture

---

## 6. Security Best Practices

### General:
1. **Enable MFA** cho root account và privileged users
2. **Use strong passwords** với password policy
3. **Regular security audits** với Config, CloudTrail
4. **Encrypt sensitive data** (at rest và in transit)
5. **Monitor** với GuardDuty, Security Hub

### IAM:
1. **Least privilege** - minimum permissions
2. **Use roles** cho AWS services (không phải users)
3. **Rotate credentials** regularly
4. **Remove unused credentials**
5. **Review permissions** định kỳ

### Network:
1. **Use VPC** với proper security groups
2. **Private subnets** cho sensitive resources
3. **Use WAF** cho web applications
4. **Enable Shield** cho DDoS protection

### Data:
1. **Enable encryption** at rest và in transit
2. **Use KMS** để manage keys
3. **Regular backups** với encryption
4. **Use Macie** để discover sensitive data

---

## 📚 Key Services Summary

| Service | Purpose |
|---------|---------|
| **IAM** | Identity and Access Management |
| **KMS** | Encryption key management |
| **CloudTrail** | API call logging |
| **Config** | Configuration compliance |
| **Shield** | DDoS protection |
| **WAF** | Web application firewall |
| **GuardDuty** | Threat detection |
| **Security Hub** | Centralized security |
| **Inspector** | Vulnerability scanning |
| **Macie** | Sensitive data protection |
| **Artifact** | Compliance reports |

---

## ✅ Checklist hiểu biết

- [ ] Hiểu IAM Users, Groups, Roles, Policies
- [ ] Biết khi nào dùng Users vs Roles
- [ ] Hiểu Encryption at rest vs in transit
- [ ] Biết các security services và mục đích của chúng
- [ ] Nắm vững Shared Responsibility Model
- [ ] Hiểu các compliance frameworks
- [ ] Biết security best practices

