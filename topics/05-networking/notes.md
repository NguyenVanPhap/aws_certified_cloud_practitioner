# Networking - Tóm tắt kiến thức

## 1. Amazon VPC (Virtual Private Cloud)

### Khái niệm
VPC = logically isolated network section trong AWS cloud. Control IP ranges, subnets, routing, security.

### Components:

#### **Subnets**
- Network segments trong VPC
- Contained trong một Availability Zone
- **Public subnet**: Có route to Internet Gateway
- **Private subnet**: Không có direct internet access

#### **Internet Gateway**
- Allows VPC resources ↔ Internet communication
- Attach to VPC
- Enables two-way traffic (inbound & outbound)

#### **NAT Gateway**
- Allows private subnets → Internet (outbound only)
- Không cho phép inbound traffic từ internet
- Dùng cho: Updates, API calls từ private resources

#### **Route Tables**
- Control traffic routing trong VPC
- Define routes (destination → target)

#### **Security Groups**
- Virtual firewall cho EC2 instances
- Instance-level
- Stateful (auto allow return traffic)
- Default deny all

#### **NACLs (Network ACLs)**
- Subnet-level firewall
- Stateless (must allow both directions)
- Less commonly used than Security Groups

---

## 2. Amazon CloudFront

### Khái niệm
CloudFront = CDN (Content Delivery Network) distribute content globally với low latency.

### Đặc điểm:
- **Edge Locations**: Cache content gần users
- **Low latency**: Serve từ Edge Location gần nhất
- **Integration**: S3, EC2, Lambda@Edge
- **Use cases**: Static websites, videos, APIs

### Features:
- **Distribution**: Collection of Edge Locations
- **Origin**: Source của content (S3, EC2, etc.)
- **TTL**: Time-to-live cho cached content

---

## 3. Amazon Route 53

### Khái niệm
Route 53 = DNS web service. Translate domain names thành IP addresses.

### Features:
- **DNS resolution**: Domain → IP
- **Domain registration**: Register domains
- **Health checking**: Monitor endpoint health
- **Routing policies**:
  - **Simple**: Standard DNS
  - **Weighted**: Split traffic based on weight
  - **Latency-based**: Route to lowest latency
  - **Failover**: Active-passive
  - **Geolocation**: Route based on location

---

## 4. Amazon API Gateway

### Khái niệm
API Gateway = fully managed service để create, publish, manage APIs.

### Features:
- **REST APIs**: HTTP APIs
- **WebSocket APIs**: Real-time communication
- **Integration**: Lambda, EC2, services
- **Authentication**: IAM, Cognito, custom
- **Throttling**: Rate limiting
- **Caching**: Response caching
- **Monitoring**: CloudWatch integration

---

## 5. AWS Direct Connect

### Khái niệm
Direct Connect = dedicated network connection từ on-premises tới AWS.

### Benefits:
- **Lower latency**: Consistent network
- **Higher bandwidth**: Dedicated connection
- **Cost reduction**: Reduce data transfer costs
- **Private connection**: Không đi qua public internet

---

## 6. AWS VPN

### Khái niệm
VPN = Virtual Private Network, secure connection over public internet.

### Types:
- **Site-to-Site VPN**: Connect on-premises network ↔ VPC
- **Client VPN**: Connect individual devices ↔ VPC

---

## 📚 Key Concepts

### VPC:
- **Subnets** = Network segments
- **Public** = Internet Gateway
- **Private** = NAT Gateway for outbound
- **Security Groups** = Instance-level firewall

### CloudFront:
- **CDN** = Global content distribution
- **Edge Locations** = Cache closer to users

### Route 53:
- **DNS** = Domain name resolution
- **Routing policies** = Traffic routing strategies

---

## ✅ Checklist

- [ ] Hiểu VPC và components
- [ ] Biết Public vs Private subnets
- [ ] Hiểu CloudFront và CDN
- [ ] Biết Route 53 và DNS
- [ ] Hiểu Security Groups vs NACLs

