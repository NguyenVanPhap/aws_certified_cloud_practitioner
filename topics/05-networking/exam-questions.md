# Networking - Exam Style Questions

---

## Question 1
What is Amazon VPC?

A. A compute service  
B. A virtual private cloud that lets you provision a logically isolated network  
C. A storage service  
D. A database service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** VPC = Virtual Private Cloud = logically isolated network section trong AWS. Control IP ranges, subnets, routing, security.

**Exam Tip:** VPC = Isolated network trong AWS.
</details>

---

## Question 2
What is CloudFront?

A. A compute service  
B. A Content Delivery Network (CDN) service  
C. A storage service  
D. A database service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** CloudFront = CDN distribute content globally với low latency. Cache content ở Edge Locations gần users. Tích hợp với S3, EC2.

**Exam Tip:** CloudFront = CDN, Edge Locations, low latency.
</details>

---

## Question 3
What is Route 53?

A. A networking service  
B. A Domain Name System (DNS) web service  
C. A load balancer  
D. A VPN service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Route 53 = DNS web service. Translate domain names thành IP addresses. Also domain registration, health checking, routing policies.

**Exam Tip:** Route 53 = DNS service.
</details>

---

## Question 4
What is a subnet in VPC?

A. A network segment within a VPC  
B. A security group  
C. A load balancer  
D. A firewall

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** Subnet = network segment trong VPC, contained trong một Availability Zone. Public subnet = route to Internet Gateway, Private = no direct internet.

**Exam Tip:** Subnet = Network segment, within one AZ.
</details>

---

## Question 5
What is the difference between a public subnet and a private subnet?

A. Public subnets are larger  
B. Public subnets have a route to the Internet Gateway, private subnets do not  
C. Private subnets are faster  
D. They are the same

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Public = route to Internet Gateway → direct internet access. Private = no direct internet → need NAT Gateway cho outbound.

**Exam Tip:** Public = IGW | Private = NAT Gateway for outbound.
</details>

---

## Question 6
What is an Internet Gateway used for?

A. To connect VPCs  
B. To provide internet connectivity for VPC resources  
C. To load balance traffic  
D. To cache content

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Internet Gateway = allows VPC resources ↔ Internet communication. Attach to VPC, used bởi public subnets. Two-way traffic.

**Exam Tip:** Internet Gateway = VPC ↔ Internet.
</details>

---

## Question 7
What is a NAT Gateway used for?

A. To connect VPCs  
B. To allow private subnets to access the internet  
C. To load balance traffic  
D. To cache content

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** NAT Gateway = allows resources trong private subnets to access internet (outbound only). Không cho phép inbound từ internet.

**Exam Tip:** NAT Gateway = Private subnet → Internet (outbound only).
</details>

---

## Question 8
What is CloudFront Edge Location used for?

A. To store databases  
B. To cache content closer to users  
C. To run compute instances  
D. To store backups

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Edge Locations = locations gần users để cache content. CloudFront serve từ Edge Location gần nhất → lower latency.

**Exam Tip:** Edge Locations = Cache closer to users, nhiều hơn AZs.
</details>

---

## Question 9
What is the difference between Security Groups and NACLs (Network ACLs)?

A. They are the same  
B. Security Groups are instance-level, NACLs are subnet-level  
C. NACLs are instance-level, Security Groups are subnet-level  
D. Security Groups are for databases only

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Security Groups = instance-level firewall, stateful. NACLs = subnet-level firewall, stateless. Security Groups được recommend.

**Exam Tip:** Security Groups = Instance-level | NACLs = Subnet-level.
</details>

---

## Question 10
What is Direct Connect?

A. A VPN service  
B. A dedicated network connection from on-premises to AWS  
C. A CDN service  
D. A DNS service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Direct Connect = dedicated network connection từ on-premises tới AWS. Private connection, không đi qua public internet. Lower latency.

**Exam Tip:** Direct Connect = Dedicated connection, private.
</details>

---

## Question 11
What is AWS VPN?

A. A dedicated connection  
B. A secure connection between on-premises and AWS over the internet  
C. A CDN service  
D. A DNS service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** VPN = Virtual Private Network, secure connection over public internet. Site-to-Site VPN hoặc Client VPN.

**Exam Tip:** VPN = Secure over internet | Direct Connect = Dedicated.
</details>

---

## Question 12
What does CDN stand for and what is its purpose?

A. Content Distribution Network - to distribute content globally with low latency  
B. Cloud Data Network - to store data  
C. Compute Distribution Network - to run applications  
D. Cache Distribution Network - to cache databases

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** CDN = Content Delivery Network. Purpose = distribute content globally với low latency bằng cách cache ở Edge Locations.

**Exam Tip:** CDN = Global distribution, low latency.
</details>

---

## Question 13
What is API Gateway?

A. A database service  
B. A service to create, publish, and manage APIs  
C. A storage service  
D. A compute service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** API Gateway = fully managed service để create, publish, maintain APIs. Tích hợp với Lambda, EC2. Handles authentication, throttling.

**Exam Tip:** API Gateway = Manage and expose APIs.
</details>

---

## Question 14
Which of the following are Route 53 routing policies? (Select THREE)

A. Simple  
B. Weighted  
C. Latency-based  
D. Failover  
E. Network-based

<details>
<summary><strong>Answer: A, B, C, D</strong></summary>

**Explanation:** Route 53 routing policies: Simple, Weighted, Latency-based, Failover, Geolocation. Network-based không phải routing policy.

**Exam Tip:** Route 53 policies: Simple, Weighted, Latency, Failover, Geolocation.
</details>

---

## Question 15
What is a Security Group in VPC?

A. A group of users  
B. A virtual firewall that controls traffic for EC2 instances  
C. A subnet  
D. A load balancer

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Security Groups = virtual firewall cho EC2 instances. Control inbound và outbound traffic. Stateful (auto allow return traffic).

**Exam Tip:** Security Groups = Virtual firewall, stateful.
</details>

---

## 📊 Exam Simulation

Làm 15 câu trong **23 phút**:
- **14-15 đúng**: ✅ Excellent!
- **12-13 đúng**: ✅ Good!
- **Dưới 12 đúng**: 📚 Review

---

## 💡 Exam Tips

1. **VPC** = Isolated network, subnets (public/private)
2. **CloudFront** = CDN, Edge Locations
3. **Route 53** = DNS service, routing policies
4. **Security Groups** = Instance-level firewall
5. **NAT Gateway** = Private subnet outbound access

---

## 🔄 Review Schedule

- Lần 1: Sau notes
- Lần 2: Sau 2 ngày
- Lần 3: Sau 5 ngày
- Lần 4: 1 tuần trước thi

Mục tiêu: 100%!

