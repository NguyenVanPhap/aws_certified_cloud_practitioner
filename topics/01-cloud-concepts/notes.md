# Cloud Concepts - Tóm tắt kiến thức

## 1. Cloud Computing là gì?

**Định nghĩa:** Cloud computing = on-demand delivery của computing resources (servers, storage, databases, networking, software) qua internet với pay-as-you-go pricing.

### 5 đặc điểm chính của Cloud (NIST):

1. **On-demand self-service**: Tự động provision resources qua console/API
2. **Broad network access**: Truy cập từ mọi nơi qua internet
3. **Resource pooling**: Tài nguyên được chia sẻ (multi-tenant)
4. **Rapid elasticity**: Tự động scale nhanh theo demand
5. **Measured service**: Trả tiền theo usage (metered billing)

---

## 2. Lợi ích của Cloud Computing

### Chi phí (Cost)
- ✅ **Giảm CapEx** (Capital Expenditure) - Không cần mua hardware trước
- ✅ **Tăng OpEx** (Operational Expenditure) - Pay-as-you-go
- ✅ **Không có upfront costs** - Không cần đầu tư ban đầu
- ✅ **Variable costs** - Chỉ trả cho những gì dùng

### Tốc độ (Speed)
- ✅ **Agility** - Deploy applications nhanh (vài phút vs vài tuần)
- ✅ **Faster time to market** - Ra mắt sản phẩm nhanh hơn
- ✅ **On-demand resources** - Provision ngay lập tức

### Scale (Quy mô)
- ✅ **Scalability** - Khả năng xử lý tăng trưởng
  - Horizontal scaling (scale out) = Thêm nhiều servers
  - Vertical scaling (scale up) = Tăng power cho server
- ✅ **Elasticity** - Tự động scale up/down theo demand
- ✅ **Unlimited capacity** - Gần như không giới hạn

### Hiệu suất (Performance)
- ✅ **Global infrastructure** - Đặt resources gần users
- ✅ **High availability** - Uptime cao
- ✅ **Fault tolerance** - Vẫn hoạt động khi có lỗi

### Bảo mật (Security)
- ✅ **AWS managed security** - AWS chịu trách nhiệm infrastructure security
- ✅ **Compliance certifications** - Đạt nhiều chuẩn bảo mật

---

## 3. Mô hình triển khai (Deployment Models)

### Public Cloud
- **Định nghĩa**: Cloud services được cung cấp bởi third-party qua internet
- **Ví dụ**: AWS, Azure, GCP
- **Đặc điểm**: Shared infrastructure, pay-as-you-go
- **Use case**: Hầu hết các tổ chức

### Private Cloud
- **Định nghĩa**: Cloud infrastructure dành riêng cho một organization
- **Đặc điểm**: Highest control & security, nhưng nhiều management hơn
- **Use case**: Organizations cần strict compliance (banking, healthcare)

### Hybrid Cloud
- **Định nghĩa**: Kết hợp on-premises + cloud services
- **Đặc điểm**: Kết nối giữa 2 môi trường, flexibility
- **Use case**: Migrate dần từ on-premises, sensitive data ở on-premises

### Multi-Cloud
- **Định nghĩa**: Sử dụng nhiều cloud providers (AWS + Azure + GCP)
- **Use case**: Avoid vendor lock-in, best of breed services

---

## 4. Mô hình dịch vụ (Service Models)

### IaaS - Infrastructure as a Service
- **AWS quản lý**: Hardware, networking, virtualization
- **Bạn quản lý**: OS, applications, data, runtime
- **Ví dụ AWS**: EC2, EBS, VPC

**Analog**: Bạn thuê đất trống, tự xây nhà

### PaaS - Platform as a Service
- **AWS quản lý**: Hardware, networking, virtualization, OS, runtime
- **Bạn quản lý**: Applications, data
- **Ví dụ AWS**: Elastic Beanstalk, RDS (managed database)

**Analog**: Bạn thuê nhà đã xây sẵn, chỉ cần vào ở

### SaaS - Software as a Service
- **AWS quản lý**: Everything
- **Bạn quản lý**: Chỉ sử dụng
- **Ví dụ**: Gmail, Office 365, Salesforce

**Analog**: Bạn vào khách sạn, mọi thứ đã sẵn sàng

### FaaS - Function as a Service (Serverless)
- **AWS quản lý**: Everything
- **Bạn quản lý**: Chỉ code (function)
- **Ví dụ AWS**: Lambda
- **Đặc điểm**: Pay-per-execution, no servers to manage

---

## 5. AWS Global Infrastructure

### Regions
- **Định nghĩa**: Geographic area chứa multiple Availability Zones
- **Ví dụ**: us-east-1 (N. Virginia), ap-southeast-1 (Singapore)
- **Lưu ý**: Chọn region dựa trên:
  - Vị trí users (để giảm latency)
  - Compliance requirements (data residency)
  - Service availability (không phải service nào cũng có ở mọi region)

### Availability Zones (AZs)
- **Định nghĩa**: Một hoặc nhiều data centers riêng biệt với redundant power, networking, connectivity
- **Đặc điểm**: Isolated từ AZ khác, kết nối với low-latency
- **Best practice**: Deploy across multiple AZs để đảm bảo high availability

### Data Centers
- **Định nghĩa**: Physical facility chứa servers
- **Lưu ý**: Customer không bao giờ truy cập trực tiếp data centers

### Edge Locations
- **Định nghĩa**: Locations gần users để cache content (cho CloudFront)
- **Số lượng**: Nhiều hơn AZs rất nhiều
- **Mục đích**: Giảm latency cho static/dynamic content

---

## 6. AWS Shared Responsibility Model

### AWS chịu trách nhiệm: **Security OF the Cloud**
- Infrastructure security (hardware, software, networking)
- Regions, Availability Zones, Edge locations
- Service availability
- Compliance of infrastructure

### Customer chịu trách nhiệm: **Security IN the Cloud**
- **IaaS (EC2)**: OS, applications, data, security groups, firewall rules
- **PaaS (RDS)**: Applications, data, database configurations
- **SaaS**: Customer data, access management
- **Always customer responsibility**: Data, access control, encryption settings

**Key Point**: Tùy service model, customer responsibility khác nhau. Càng lên cao (PaaS, SaaS), customer càng ít phải quản lý.

---

## 7. Key Terms

### Scalability vs Elasticity
- **Scalability**: Khả năng xử lý tăng trưởng (growth), có thể manual hoặc automatic
- **Elasticity**: Tự động scale up/down theo demand (automatic)

### High Availability vs Fault Tolerance
- **High Availability**: System vẫn hoạt động với minimal downtime khi có failure
- **Fault Tolerance**: System tiếp tục hoạt động hoàn toàn khi có component failure (zero downtime)

### Agility
- Khả năng phát triển và deploy applications nhanh chóng
- Cloud cho phép provision resources trong vài phút vs vài tuần on-premises

---

## 8. AWS Use Cases

- **Web hosting**: Static websites trên S3 + CloudFront
- **Mobile backends**: API Gateway + Lambda
- **Data processing**: Kinesis, EMR
- **Backup & disaster recovery**: S3, Glacier
- **Big data analytics**: Redshift, Athena
- **IoT**: IoT Core
- **Machine Learning**: SageMaker

---

## 📚 Tài nguyên bổ sung

1. **AWS Cloud Practitioner Essentials** (AWS Training - FREE)
2. **AWS Whitepapers**: 
   - AWS Overview Whitepaper
   - AWS Well-Architected Framework
3. **AWS Documentation**: AWS Global Infrastructure
4. **Thực hành**: Tạo AWS Free Tier account, explore Console

---

## ✅ Checklist hiểu biết

Sau khi đọc notes này, bạn nên:
- [ ] Giải thích được 5 đặc điểm của cloud (NIST)
- [ ] So sánh được IaaS, PaaS, SaaS
- [ ] Hiểu sự khác biệt giữa Regions, AZs, Edge Locations
- [ ] Giải thích được Shared Responsibility Model
- [ ] Phân biệt được Scalability vs Elasticity
- [ ] Hiểu các lợi ích chính của cloud computing

