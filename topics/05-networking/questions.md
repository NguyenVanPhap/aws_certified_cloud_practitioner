# Networking - Practice Questions

> 💡 **Cách học**: Tự trả lời trước, đọc kỹ giải thích về VPC, CloudFront, Route 53.

---

## Question 1
**What is Amazon VPC?**

A. A compute service  
B. A virtual private cloud that lets you provision a logically isolated network  
C. A storage service  
D. A database service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** VPC (Virtual Private Cloud) = logically isolated network section trong AWS cloud. Bạn có thể control IP ranges, subnets, routing, security. Mỗi AWS account có default VPC.

**Key Concept:** VPC = Isolated network section trong AWS
</details>

---

## Question 2
**What is CloudFront?**

A. A compute service  
B. A Content Delivery Network (CDN) service  
C. A storage service  
D. A database service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** CloudFront = CDN (Content Delivery Network) distribute content globally với low latency. Cache content ở Edge Locations gần users. Tích hợp với S3, EC2, Lambda@Edge.

**Key Concept:** CloudFront = CDN, Edge Locations, low latency
</details>

---

## Question 3
**What is Route 53?**

A. A networking service  
B. A Domain Name System (DNS) web service  
C. A load balancer  
D. A VPN service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Route 53 = DNS web service. Translate domain names thành IP addresses, route traffic. Also provides domain registration, health checking, routing policies.

**Key Concept:** Route 53 = DNS service
</details>

---

## Question 4
**What is a subnet in VPC?**

A. A network segment within a VPC  
B. A security group  
C. A load balancer  
D. A firewall

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** Subnet = network segment trong VPC, contained trong một Availability Zone. Public subnet = có route to Internet Gateway, Private subnet = không có direct internet access.

**Key Concept:** Subnet = Network segment in VPC, within one AZ
</details>

---

## Question 5
**What is the difference between a public subnet and a private subnet?**

A. Public subnets are larger  
B. Public subnets have a route to the Internet Gateway, private subnets do not  
C. Private subnets are faster  
D. They are the same

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Public subnet = có route to Internet Gateway → resources có public IP và direct internet access. Private subnet = không có route to Internet Gateway → resources chỉ có private IP, no direct internet access (need NAT).

**Key Concept:** Public = Internet Gateway | Private = No direct internet
</details>

---

## Question 6
**What is an Internet Gateway used for?**

A. To connect VPCs  
B. To provide internet connectivity for VPC resources  
C. To load balance traffic  
D. To cache content

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Internet Gateway = allows communication giữa resources trong VPC và internet. Attach to VPC, used bởi public subnets. Enables two-way traffic: inbound và outbound.

**Key Concept:** Internet Gateway = VPC ↔ Internet connectivity
</details>

---

## Question 7
**What is a NAT Gateway used for?**

A. To connect VPCs  
B. To allow private subnets to access the internet  
C. To load balance traffic  
D. To cache content

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** NAT Gateway = allows resources trong private subnets to access internet (outbound) nhưng không cho phép inbound traffic từ internet. Dùng để download updates, access APIs, etc.

**Key Concept:** NAT Gateway = Private subnet → Internet (outbound only)
</details>

---

## Question 8
**What is CloudFront Edge Location used for?**

A. To store databases  
B. To cache content closer to users  
C. To run compute instances  
D. To store backups

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Edge Locations = locations gần users để cache content. Khi user request, CloudFront serve từ Edge Location gần nhất → lower latency. Có nhiều hơn Availability Zones.

**Key Concept:** Edge Locations = Cache content closer to users
</details>

---

## Question 9
**What is Route 53's primary function?**

A. To provide load balancing  
B. To translate domain names to IP addresses (DNS resolution)  
C. To cache content  
D. To encrypt traffic

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Route 53 = DNS service, translate domain names (example.com) thành IP addresses (192.0.2.1). Also provides routing policies (failover, weighted, latency-based).

**Key Concept:** Route 53 = DNS resolution (domain → IP)
</details>

---

## Question 10
**What is an API Gateway?**

A. A database service  
B. A service to create, publish, and manage APIs  
C. A storage service  
D. A compute service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** API Gateway = fully managed service để create, publish, maintain APIs. Tích hợp với Lambda, EC2, services. Handles authentication, throttling, caching, monitoring.

**Key Concept:** API Gateway = Manage and expose APIs
</details>

---

## Question 11
**What is a Security Group in VPC?**

A. A group of users  
B. A virtual firewall that controls traffic for EC2 instances  
C. A subnet  
D. A load balancer

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Security Groups = virtual firewall cho EC2 instances, control inbound và outbound traffic. Stateful (allow return traffic automatically), default deny all.

**Key Concept:** Security Groups = Virtual firewall for instances
</details>

---

## Question 12
**What is the difference between Security Groups and NACLs (Network ACLs)?**

A. They are the same  
B. Security Groups are instance-level, NACLs are subnet-level  
C. NACLs are instance-level, Security Groups are subnet-level  
D. Security Groups are for databases only

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Security Groups = instance-level firewall, stateful. NACLs (Network ACLs) = subnet-level firewall, stateless (must allow both directions). Security Groups được recommend cho most use cases.

**Key Concept:** Security Groups = Instance-level | NACLs = Subnet-level
</details>

---

## Question 13
**What is Direct Connect?**

A. A VPN service  
B. A dedicated network connection from on-premises to AWS  
C. A CDN service  
D. A DNS service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Direct Connect = dedicated network connection từ on-premises data center tới AWS. Private connection, không đi qua public internet. Lower latency, more consistent network experience.

**Key Concept:** Direct Connect = Dedicated connection on-premises ↔ AWS
</details>

---

## Question 14
**What is AWS VPN?**

A. A dedicated connection  
B. A secure connection between on-premises and AWS over the internet  
C. A CDN service  
D. A DNS service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** VPN = Virtual Private Network, secure connection over public internet. Site-to-Site VPN = connect on-premises network tới VPC. Client VPN = connect individual devices tới VPC.

**Key Concept:** VPN = Secure connection over internet
</details>

---

## Question 15
**What does CDN stand for and what is its purpose?**

A. Content Distribution Network - to distribute content globally with low latency  
B. Cloud Data Network - to store data  
C. Compute Distribution Network - to run applications  
D. Cache Distribution Network - to cache databases

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** CDN = Content Delivery Network. Purpose = distribute content (images, videos, static files) globally với low latency bằng cách cache content ở Edge Locations gần users.

**Key Concept:** CDN = Global content distribution với low latency
</details>

---

## 📊 Tự đánh giá

- **13-15 câu đúng**: ✅ Excellent!
- **10-12 câu đúng**: ✅ Good!
- **Dưới 10 câu**: 📚 Review notes.md

---

## 💡 Tips

1. VPC = Isolated network trong AWS
2. Subnets = Network segments (public/private)
3. CloudFront = CDN (Edge Locations)
4. Route 53 = DNS service
5. Security Groups = Instance-level firewall

