# Networking Services - Exam Questions V2

> 🧠 Mục tiêu: Ôn tập toàn diện Networking services cho AWS Certified Cloud Practitioner  
> 🌐 Nội dung: 50 câu nền tảng + 30 câu khó (tổng 80 câu) dạng multiple-choice/multiple-response

---

## Phần A - Câu hỏi nền tảng (50 câu)

### Question 1
Dịch vụ nào cho phép định nghĩa mạng ảo riêng trong AWS?

A. Amazon Route 53  
B. Amazon VPC  
C. AWS CloudFront  
D. AWS Firewall Manager

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Amazon Virtual Private Cloud (VPC) cho phép tạo mạng logic riêng, định nghĩa subnets, route table, security.
</details>

---

### Question 2
Subnet công khai (public subnet) trong VPC yêu cầu gì để truy cập Internet?

A. Internet Gateway gắn với VPC và route 0.0.0.0/0 tới IGW  
B. NAT Gateway  
C. AWS Direct Connect  
D. VPC Peering

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Public subnet cần route default tới Internet Gateway và instances phải có public IP/Elastic IP.
</details>

---

### Question 3
NAT Gateway dùng cho mục đích nào?

A. Cho phép inbound traffic vào private subnet  
B. Cho phép outbound internet access từ private subnet  
C. Tạo VPN site-to-site  
D. Tạo DNS record

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** NAT Gateway cho phép instances trong private subnet truy cập Internet outgoing mà vẫn giữ private IP.
</details>

---

### Question 4
Security Group có đặc điểm?

A. Stateless, áp dụng ở mức subnet  
B. Stateful, áp dụng ở mức instance/ENI  
C. Stateless, mức VPC  
D. Chỉ outbound

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Security Group là firewall stateful, gắn vào ENI/instance, tự động cho phép traffic phản hồi.
</details>

---

### Question 5
Network ACL có đặc điểm gì so với Security Group?

A. Stateful  
B. Áp dụng cho VPC  
C. Stateless, áp dụng ở mức subnet, cho phép rule theo thứ tự  
D. Chỉ outbound

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** NACL là stateless, áp dụng cho subnet, đánh giá rule từ số nhỏ tới lớn, cần rule inbound và outbound riêng.
</details>

---

### Question 6
Route 53 là dịch vụ gì?

A. CDN  
B. DNS managed service  
C. Firewall  
D. VPN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Amazon Route 53 là dịch vụ DNS có hỗ trợ routing policies, health checks, domain registration.
</details>

---

### Question 7
CloudFront là gì?

A. Dịch vụ DNS  
B. Content Delivery Network (CDN)  
C. VPN  
D. Load Balancer

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** CloudFront phân phối nội dung qua edge locations, giảm latency, cải thiện bảo mật.
</details>

---

### Question 8
Loại Elastic Load Balancer nào hoạt động ở Layer 7?

A. Application Load Balancer (ALB)  
B. Network Load Balancer (NLB)  
C. Gateway Load Balancer (GWLB)  
D. Classic Load Balancer (CLB)

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** ALB hoạt động ở layer 7 (HTTP/HTTPS), hỗ trợ path-based, host-based routing.
</details>

---

### Question 9
Direct Connect mang lại lợi ích?

A. Kết nối rộng rãi Internet  
B. Kết nối dedicated private tới AWS, latency thấp, băng thông ổn định  
C. DNS management  
D. Firewall

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Direct Connect tạo link mạng riêng giữa trung tâm dữ liệu và AWS, bypass Internet.
</details>

---

### Question 10
Site-to-Site VPN trên AWS kết nối thông qua?

A. Internet Gateway  
B. Virtual Private Gateway và Customer Gateway  
C. Transit Gateway  
D. NAT Gateway

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** VPN site-to-site cần Virtual Private Gateway (AWS side) và Customer Gateway (on-prem) qua Internet.
</details>

---

### Question 11
Endpoint type nào hỗ trợ truy cập riêng tới S3/DynamoDB không qua Internet?

A. Interface Endpoint  
B. Gateway Endpoint  
C. Gateway Load Balancer Endpoint  
D. NAT Endpoint

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Gateway Endpoint hỗ trợ S3 và DynamoDB, giúp private subnet truy cập mà không dùng Internet Gateway.
</details>

---

### Question 12
VPC Peering cho phép?

A. Kết nối VPC một cách private point-to-point  
B. VPN  
C. CDN  
D. Load balancing global

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** VPC Peering cho phép route traffic giữa hai VPC như một mạng private, không qua Internet.
</details>

---

### Question 13
AWS Global Accelerator cung cấp?

A. Content caching  
B. Địa chỉ IP tĩnh toàn cầu, tối ưu routing đến endpoint ở nhiều region  
C. Mã hóa data  
D. DNS hosting

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Global Accelerator cấp IP tĩnh, dùng mạng AWS để tối ưu latency, failover giữa endpoint region.
</details>

---

### Question 14
Khi nào nên dùng Network Load Balancer?

A. Khi cần xử lý HTTP  
B. Khi cần TCP/UDP high performance, latency thấp, static IP  
C. Khi cần content-based routing  
D. Khi cần WebSocket

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** NLB ở layer 4, hỗ trợ TCP/UDP, static IP, throughput cao, phù hợp ứng dụng latency thấp.
</details>

---

### Question 15
Amazon CloudFront kết hợp dịch vụ nào để bảo vệ DDoS?

A. AWS Shield Standard tích hợp mặc định  
B. AWS IAM  
C. AWS Config  
D. AWS Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CloudFront đi kèm bảo vệ DDoS cơ bản từ AWS Shield Standard, có thể nâng cấp Shield Advanced.
</details>

---

### Question 16
CIDR /24 tương đương?

A. 16 địa chỉ IP  
B. 32 địa chỉ IP  
C. 256 địa chỉ IP  
D. 1024 địa chỉ IP

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** /24 có 2^(32-24) = 256 địa chỉ, trong VPC usable ít hơn 5 do AWS reserve.
</details>

---

### Question 17
Elastic IP là?

A. IP dynamic  
B. IP tĩnh public có thể gán lại giữa instances  
C. IP private  
D. DNS record

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Elastic IP là địa chỉ IPv4 tĩnh do AWS cấp, có thể remap cho tăng HA.
</details>

---

### Question 18
Phần tử nào giúp chia traffic layer 7 based vào URL path?

A. Route 53  
B. Application Load Balancer  
C. Network Load Balancer  
D. NAT Gateway

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** ALB hỗ trợ listener rule theo path/host header, chuyển traffic đến target group tương ứng.
</details>

---

### Question 19
Transit Gateway dùng để?

A. Chia sẻ file  
B. Kết nối nhiều VPC và on-premises network thông qua hub-and-spoke  
C. CDN  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Transit Gateway là hub kết nối VPC, Direct Connect, VPN, giảm phức tạp so với peering mesh.
</details>

---

### Question 20
AWS PrivateLink cung cấp?

A. Endpoint riêng truy cập dịch vụ AWS/third-party qua interface endpoint  
B. VPN site-to-site  
C. CDN  
D. IAM roles

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** PrivateLink cho phép truy cập dịch vụ qua interface endpoint trong VPC, traffic không đi qua Internet.
</details>

---

### Question 21
Route 53 health check có thể dùng để?

A. Kiểm tra sức khỏe endpoint và thực hiện failover routing  
B. Mã hóa dữ liệu  
C. Backup dữ liệu  
D. VPC peering

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Health check monitor endpoint, kết hợp routing policy (failover) để chuyển traffic khi endpoint unhealthy.
</details>

---

### Question 22
VPC Flow Logs ghi lại gì?

A. API call  
B. Traffic metadata (accept/reject) ở mức ENI, subnet, VPC  
C. DNS query  
D. IAM policy

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Flow Logs ghi metadata traffic (source/dest IP, port, action) để phân tích network/security.
</details>

---

### Question 23
AWS Client VPN dùng để?

A. Kết nối site-to-site  
B. Kết nối người dùng từ xa (client) đến VPC  
C. Tạo CDN  
D. Định danh người dùng

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Client VPN là dịch vụ VPN manage, cho phép người dùng truy cập VPC thông qua OpenVPN-based client.
</details>

---

### Question 24
Sự khác biệt chính giữa Internet Gateway và NAT Gateway?

A. IGW hỗ trợ inbound/outbound public, NAT chỉ outbound cho private subnet  
B. NAT hỗ trợ inbound  
C. IGW là dịch vụ trả phí cao  
D. NAT dùng cho DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** IGW cho phép traffic internet 2 chiều cho public subnet; NAT cho phép private subnet truy cập outbound Internet.
</details>

---

### Question 25
Route 53 hỗ trợ kiểu routing nào? (Chọn hai)

A. Weighted routing  
B. Simple routing  
C. VPN routing  
D. ECS routing  
E. Latency-based routing

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A, E  
**Giải thích:** Route 53 hỗ trợ simple, weighted, latency-based, failover, geolocation, geoproximity, multi-value.
</details>

---

### Question 26
CloudFront có thể kết hợp OAI (Origin Access Identity) để?

A. Cấm truy cập origin trực tiếp, chỉ cho CloudFront truy cập S3  
B. Bật IPv6  
C. Mã hóa SSL  
D. Tăng TTL

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** OAI cho phép S3 bucket chỉ cho phép CloudFront truy cập, ngăn truy cập trực tiếp.
</details>

---

### Question 27
AWS WAF thường được triển khai với?

A. Application Load Balancer hoặc CloudFront  
B. NAT Gateway  
C. Route 53  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** WAF có thể gắn vào ALB, CloudFront, API Gateway để lọc request, block OWASP attacks.
</details>

---

### Question 28
Transit Gateway hỗ trợ chức năng nào?

A. VPC peering tự động  
B. Attach VPN, Direct Connect và VPC vào cùng hub  
C. DNS hosting  
D. CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** TGW kết nối nhiều VPC, VPN, Direct Connect, centralize routing.
</details>

---

### Question 29
AWS Network Firewall cung cấp?

A. Firewall stateful managed ở cấp VPC  
B. IAM policy  
C. CDN  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** AWS Network Firewall là dịch vụ firewall managed, triển khai trong VPC, hỗ trợ rule stateful, intrusion prevention.
</details>

---

### Question 30
Route 53 Resolver inbound endpoint dùng để?

A. Cho phép DNS query từ on-prem vào VPC resolver  
B. Query public domain  
C. Mã hóa traffic  
D. CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Inbound endpoint cho phép hệ thống on-prem gửi DNS query vào resolver trong VPC, hỗ trợ hybrid.
</details>

---

### Question 31
Khi nào nên sử dụng Multi-Value Answer routing?

A. Cần direct routing duy nhất  
B. Muốn trả về nhiều IP kèm health check, tác dụng như basic load balancing  
C. Muốn route theo latency  
D. Muốn geo routing

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Multi-Value Answer trả về nhiều healthy IP, giúp phân phối traffic đơn giản.
</details>

---

### Question 32
AWS Shield Advanced khác Shield Standard ở điểm?

A. Shield Advanced mất phí, cung cấp bảo vệ DDoS nâng cao, SLA và hỗ trợ 24/7  
B. Shield Standard mất phí  
C. Shield Advanced không hỗ trợ CloudFront  
D. Shield Standard không tồn tại

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Shield Advanced là dịch vụ trả phí, cung cấp advanced DDoS protection, cost protection, metrics, hỗ trợ.
</details>

---

### Question 33
AWS Firewall Manager giúp?

A. Quản lý tập trung policy WAF, Shield, Network Firewall cho nhiều account  
B. DNS  
C. Backup  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Firewall Manager cho phép quản lý firewall policy đa tài khoản bằng AWS Organizations.
</details>

---

### Question 34
AWS Outposts về networking yêu cầu?

A. Kết nối Internet tốc độ cao  
B. VPN site-to-site  
C. Direct Connect hoặc VPN để kết nối region AWS quản lý control plane  
D. Không cần kết nối

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** Outposts cần kết nối mạng ổn định tới region AWS qua DX hoặc VPN để kết nối control plane.
</details>

---

### Question 35
Private Hosted Zone của Route 53 dùng khi?

A. Cần DNS public  
B. Cần DNS internal cho VPC  
C. Cần CDN  
D. Cần backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Private Hosted Zone cung cấp DNS cho tài nguyên trong VPC, không public.
</details>

---

### Question 36
CloudFront hỗ trợ edge functions nào để tùy biến request/response?

A. Lambda@Edge  
B. AWS Batch  
C.AWS Step Functions  
D. AWS Glue

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Lambda@Edge chạy function tại edge location, tùy biến request/response CloudFront.
</details>

---

### Question 37
Elastic Load Balancing hỗ trợ cross-zone load balancing nghĩa là?

A. Phân phối traffic đều giữa AZ trong region  
B. Chỉ một AZ  
C. CDN  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Cross-zone cho phép LB phân phối request đến targets ở tất cả AZ đã enable, giảm mất cân bằng.
</details>

---

### Question 38
AWS VPN CloudHub dùng khi?

A. Kết nối nhiều site (VPN) tới Virtual Private Gateway, chia sẻ routing  
B. CDN  
C. Backup  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CloudHub cho phép site-to-site VPN đa site, share routing qua Virtual Private Gateway.
</details>

---

### Question 39
Amazon Route 53 Resolver DNS Firewall dùng để?

A. Chặn domain độc hại ở cấp DNS  
B. Mã hóa dữ liệu  
C. Backup  
D. CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Resolver DNS Firewall cho phép tạo danh sách domain allow/deny để bảo vệ DNS outbound.
</details>

---

### Question 40
AWS Site-to-Site VPN có SLA 99.9%. Để tăng cao availability nên?

A. Sử dụng một tunnel  
B. Triển khai VPN dự phòng (hai tunnel) và/hoặc Direct Connect với VPN backup  
C. Dùng NAT  
D. S3 replication

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Site-to-Site cung cấp hai tunnel, nên cấu hình cả hai và kết hợp DX cho HA.
</details>

---

### Question 41
Khi cần expose dịch vụ nội bộ tới đối tác qua PrivateLink, cần?

A. Tạo VPC Endpoint Service và cho phép đối tác kết nối qua Interface Endpoint  
B. Public IP  
C. NAT  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** VPC Endpoint Service cho phép chia sẻ dịch vụ qua PrivateLink, đối tác tạo Interface Endpoint để truy cập.
</details>

---

### Question 42
Elastic Load Balancer health check nếu target unhealthy sẽ?

A. Tự động terminate instance  
B. Ngừng gửi traffic tới target unhealthy  
C. Scale in  
D. Gửi email

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** LB health check remove target khỏi rotation cho tới khi healthy trở lại.
</details>

---

### Question 43
Route 53 geolocation routing dùng để?

A. Route traffic dựa trên vị trí địa lý của user  
B. Dựa trên latency  
C. Dựa trên weight  
D. Failover

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Geolocation routing cho phép phân phối theo location (continent, country, state).
</details>

---

### Question 44
CloudFront Origin Shield là gì?

A. Tầng cache trung gian giảm tải origin  
B. ACL  
C. DNS  
D. Tường lửa

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Origin Shield thêm layer cache, tối ưu request đến origin, giảm tải và cải thiện cache hit ratio.
</details>

---

### Question 45
Amazon Route 53 registrar dùng để?

A. Đăng ký tên miền  
B. CDN  
C. Firewall  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Route 53 Registrar cho phép đăng ký, quản lý domain trực tiếp từ AWS.
</details>

---

### Question 46
AWS App Mesh liên quan networking thế nào?

A. Service mesh quản lý traffic giữa microservices  
B. CDN  
C. DNS  
D. VPN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** App Mesh cung cấp service mesh, kiểm soát routing, retry, observability giữa microservices.
</details>

---

### Question 47
Khi nào nên dùng Elastic Fabric Adapter (EFA)?

A. Cho web server  
B. Cho HPC/ML cần low-latency, high-throughput networking giữa instances  
C. Cho CDN  
D. Cho database relational

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** EFA là network interface cho HPC, ML, hỗ trợ OS-bypass giảm latency, tăng throughput.
</details>

---

### Question 48
AWS Proton liên quan networking?

A. Quản lý template triển khai microservices, bao gồm cấu hình networking chuẩn hóa  
B. CDN  
C. DNS  
D. Firewall

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Proton quản lý template environment/service, trong đó chuẩn hóa network (VPC, load balancer) cho team dev.
</details>

---

### Question 49
Route 53 Resolver query logging gửi log tới?

A. CloudWatch Logs, S3, hoặc Kinesis Data Firehose  
B. DynamoDB  
C. CloudFront  
D. SNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Resolver query logging hỗ trợ gửi logs tới CloudWatch Logs, S3, Kinesis.
</details>

---

### Question 50
AWS Transit Gateway hỗ trợ phân tách mạng bằng?

A. Route domain  
B. Route table cho mỗi attachment  
C. IAM  
D. ACL

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** TGW có thể tạo nhiều route table, attach VPC/VPN vào route table riêng để tách traffic.
</details>

---

## Phần B - Câu hỏi khó (30 câu)

### Question 51
Bạn có 50 VPC cần kết nối mesh với nhau và với on-prem. Giải pháp tối ưu?

A. Tạo VPC peering cho từng cặp  
B. Dùng Transit Gateway làm hub kết nối VPC và VPN/Direct Connect  
C. Dùng NAT Gateway  
D. Dùng Route 53

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Transit Gateway giảm phức tạp, hỗ trợ hàng nghìn attachments, route tập trung.
</details>

---

### Question 52
Bạn cần route traffic từ nhiều account tới firewall appliance của bên thứ ba. Dịch vụ phù hợp?

A. Application Load Balancer  
B. Gateway Load Balancer kết hợp appliance  
C. NAT Gateway  
D. VPC Peering

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Gateway Load Balancer cung cấp load balancing cho appliance layer 3/4, kết hợp endpoint cross-account.
</details>

---

### Question 53
Yêu cầu: API multi-region cần IP cố định, failover tự động, latency thấp. Giải pháp?

A. Route 53 weighted  
B. Global Accelerator với endpoint ALB/EC2 ở nhiều region  
C. CloudFront  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Global Accelerator cung cấp static IP, routing tối ưu, health check failover xuyên region.
</details>

---

### Question 54
Bạn cần expose dịch vụ nội bộ (NLB) cho đối tác ở tài khoản khác qua PrivateLink. Bước nào cần thiết?

A. Tạo Endpoint Service gắn NLB, cấp quyền principal, đối tác tạo Interface Endpoint  
B. Mở public IP  
C. Dùng NAT  
D. Dùng CloudFront

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Endpoint Service + Interface Endpoint (PrivateLink) cho phép kết nối private cross-account.
</details>

---

### Question 55
Bạn cần hybrid DNS: on-prem muốn resolve tên nội bộ trong VPC và ngược lại. Giải pháp?

A. Route 53 Resolver inbound/outbound endpoint + rules  
B. CloudFront  
C. NAT Gateway  
D. S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Resolver endpoints cho phép DNS query hai chiều giữa on-prem và VPC, cấu hình forwarding rules.
</details>

---

### Question 56
Ứng dụng cần failover giữa Direct Connect và VPN khi mất kết nối. Thiết kế?

A. Dùng Direct Connect một mình  
B. Kết hợp Direct Connect + VPN (AWS Site-to-Site) dùng BGP để failover  
C. Dùng CloudFront  
D. Dùng NAT Gateway

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** DX và VPN có thể cấu hình BGP failover, AWS khuyến nghị kết hợp DX với VPN backup.
</details>

---

### Question 57
VPC cần truy cập API của dịch vụ SaaS (PrivateLink) mà không có Internet. Làm sao?

A. Tạo Interface Endpoint cho dịch vụ SaaS nếu nhà cung cấp hỗ trợ PrivateLink  
B. Dùng NAT Gateway  
C. Dùng VPC Peering  
D. Dùng Route 53

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** PrivateLink cho phép truy cập dịch vụ SaaS qua interface endpoint trong VPC mà không ra Internet.
</details>

---

### Question 58
Bạn muốn log mọi truy cập DNS ra Internet để phân tích bảo mật. Công cụ?

A. Route 53 Resolver Query Logging  
B. CloudWatch Logs  
C. IAM  
D. AWS Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Query Logging ghi DNS query từ VPC resolver, xuất sang S3/CloudWatch/Kinesis để phân tích.
</details>

---

### Question 59
Thiết kế multi-account, cần đảm bảo mọi VPC mới tạo có guardrail network (NACL, SG) chuẩn. Giải pháp?

A. AWS Control Tower + Firewall Manager, Service Catalog hoặc IaC baseline  
B. Tạo bằng tay  
C. Không cần guardrail  
D. S3 bucket policy

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Control Tower đặt guardrail, Firewall Manager áp dụng policy SG/NACL, Service Catalog cung cấp template chuẩn.
</details>

---

### Question 60
Ứng dụng gaming realtime cần latency rất thấp, user toàn cầu, traffic UDP. Giải pháp?

A. CloudFront  
B. Global Accelerator (UDP support) với endpoint gần user  
C. Route 53 weighted  
D. VPN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Global Accelerator hỗ trợ UDP, giảm latency, failover nhanh, phù hợp game real-time.
</details>

---

### Question 61
Bạn cần kiểm soát outbound internet traffic và áp dụng policy domain-based. Dịch vụ?

A. Network ACL  
B. AWS Network Firewall hoặc Route 53 Resolver DNS Firewall  
C. NAT Gateway  
D. S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Network Firewall lọc traffic layer 3/4/7; DNS Firewall chặn domain xấu.
</details>

---

### Question 62
Doanh nghiệp muốn microservices đa account chia sẻ mesh chung. Cách tối ưu?

A. App Mesh multi-account với shared mesh + service discovery (Cloud Map)  
B. VPC peering  
C. NLB  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** App Mesh hỗ trợ multi-account mesh, Cloud Map cung cấp naming, traffic policy unified.
</details>

---

### Question 63
Bạn cần triển khai WebSocket serverless. Networking cần lưu ý gì?

A. API Gateway WebSocket dùng domain riêng, tích hợp với VPC endpoints nếu cần private integration  
B. CloudFront  
C. NAT  
D. S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** API Gateway WebSocket cung cấp endpoint, có thể kết nối Lambda/VPC private integration qua VPC Link.
</details>

---

### Question 64
Workflow cần di chuyển 200TB logs hàng ngày từ on-prem lên S3. Băng thông 1 Gbps. Phương án?

A. Direct Connect hoặc DataSync để tối ưu throughput, kết hợp chuyển incremental  
B. S3 Transfer Acceleration  
C. Snowball  
D. Email

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** DX cung cấp băng thông ổn định, DataSync tối ưu transfer, incremental daily transfer feasible.
</details>

---

### Question 65
Route 53 geoproximity routing giúp làm gì?

A. Điều chỉnh traffic bằng bias dựa trên vị trí, não? yes  
B. Weighted? no  
C. CDN  
D. Firewall

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Geoproximity routing dựa vào vị trí địa lý và có bias để điều chỉnh phạm vi phân phối.
</details>

---

### Question 66
Bạn muốn centralize outbound Internet access từ nhiều VPC qua một VPC firewall. Thiết kế?

A. Sử dụng Transit Gateway + Firewall Appliance VPC + egress VPC pattern  
B. Tạo NAT trong từng VPC  
C. Cho phép Internet Gateway trực tiếp  
D. Route 53

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Mô hình egress VPC: TGW chuyển traffic ra firewall/NAT chung, áp dụng policy tập trung.
</details>

---

### Question 67
Muốn streaming video low latency global. Chọn?

A. CloudFront với RTMP/HTTP streaming, edge cache  
B. Route 53  
C. S3 website hosting  
D. CloudWatch

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CloudFront hỗ trợ live streaming, low latency content distribution global.
</details>

---

### Question 68
DNSSEC trong Route 53 dùng để?

A. Ký DNS record đảm bảo tính toàn vẹn, chống giả mạo  
B. Mã hóa HTTP  
C. CDN  
D. Firewall

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** DNSSEC ký cryptographic records, chống tampering, tăng bảo mật DNS.
</details>

---

### Question 69
Bạn muốn kiểm soát traffic giữa microservices trong ECS cluster mà không thay đổi code. Giải pháp?

A. AWS App Mesh với Envoy proxy sidecar  
B. Security Group  
C. NAT  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** App Mesh dùng Envoy sidecar để điều khiển traffic, retry, circuit breaking mà không đổi code.
</details>

---

### Question 70
Doanh nghiệp muốn theo dõi và tối ưu chi phí NAT Gateway. Gợi ý?

A. Dùng NAT instance cho traffic thấp, hoặc phân vùng private subnet theo AZ, xem xét PrivateLink  
B. Giữ nguyên  
C. Dùng IGW  
D. Dùng S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** NAT Gateway tính phí theo giờ và dữ liệu; NAT instance (tự quản lý) rẻ hơn traffic thấp; sử dụng PrivateLink/endpoint giảm traffic qua NAT.
</details>

---

### Question 71
Bạn muốn kiểm soát băng thông outbound từ VPC đến on-prem thông qua Direct Connect. Cách tiếp cận?

A. DX không hỗ trợ giới hạn băng thông  
B. Thiết lập QoS/traffic shaping trên router on-prem hoặc thiết bị DX, kết hợp Network Firewall nếu cần lọc  
C. Dùng Security Group  
D. Dùng Route 53

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Direct Connect không có throttling native; cần cấu hình QoS/traffic shaping trên thiết bị của khách hàng hoặc firewall để giới hạn lưu lượng.
</details>

---

### Question 72
Bạn cần publish API nội bộ sử dụng PrivateLink nhưng vẫn muốn kiểm soát truy cập bằng authorizer. Giải pháp?

A. API Gateway Private REST API + VPC Endpoint (Interface) + IAM/Lambda authorizer  
B. Public API Gateway  
C. CloudFront  
D. Route 53

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** API Gateway Private cho phép expose qua PrivateLink, sử dụng VPC endpoint policies và authorizer để kiểm soát truy cập.
</details>

---

### Question 73
Muốn chặn truy cập từ một quốc gia tới ứng dụng. Thực hiện?

A. Route 53 failover  
B. CloudFront Geo Restriction hoặc WAF GeoMatch rule  
C. Direct Connect  
D. NAT Gateway

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** CloudFront hỗ trợ geo restriction; WAF GeoMatch rule block phép theo country code.
</details>

---

### Question 74
Bạn cần publish dịch vụ nội bộ đồng thời cho on-prem (qua VPN) và đối tác (qua Internet) nhưng vẫn giữ private. Thiết kế?

A. Sử dụng Network Load Balancer + PrivateLink cho đối tác, VPN/Direct Connect cho on-prem, kết hợp Security Group/NACL  
B. Public Load Balancer  
C. CloudFront  
D. S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** NLB có thể phục vụ endpoint service cho PrivateLink và đồng thời route từ VPN/Direct Connect qua private IP.
</details>

---

### Question 75
Hệ thống IoT gửi dữ liệu MQTT toàn cầu cần latency thấp, kết nối bảo mật. Chọn kiến trúc?

A. AWS IoT Core với multi-region endpoint và AWS IoT Core Device Defender  
B. CloudFront  
C. Route 53 weighted  
D. NAT Gateway

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** AWS IoT Core cung cấp MQTT endpoint bảo mật, có thể dùng multi-region để giảm latency và Device Defender để giám sát bảo mật.
</details>

---

### Question 76
Bạn muốn giám sát trải nghiệm người dùng từ nhiều địa điểm khác nhau tới ứng dụng HTTP. Dịch vụ phù hợp?

A. Amazon CloudWatch Synthetics Canary kết hợp CloudWatch RUM  
B. CloudFront  
C. VPC Flow Logs  
D. AWS Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CloudWatch Synthetics tạo canary mô phỏng request từ nhiều region; CloudWatch RUM thu thập số liệu thực tế từ client.
</details>

---

### Question 77
Bạn cần chia sẻ Route 53 private hosted zone cho nhiều account trong cùng tổ chức. Cách?

A. AWS RAM (Resource Access Manager) share private hosted zone  
B. Tạo bản ghi public  
C. Dùng NAT  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** RAM cho phép chia sẻ private hosted zone giữa account trong AWS Organizations.
</details>

---

### Question 78
Bạn muốn kiểm soát traffic east-west giữa subnet trong cùng VPC bằng thiết bị firewall ảo. Giải pháp?

A. Sử dụng AWS Gateway Load Balancer + Appliance trong VPC, route traffic qua appliance  
B. NAT Gateway  
C. Route 53  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** GWLB kết hợp appliance cho phép đưa traffic nội bộ qua firewall một cách scale và HA.
</details>

---

### Question 79
Muốn tối ưu HTTP/2, TLS 1.3 và edge caching cho API. Gợi ý?

A. Đặt CloudFront trước API Gateway hoặc ALB, bật HTTP/2/TLS 1.3  
B. Sử dụng NAT  
C. Dùng Route 53  
D. Không cần

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CloudFront hỗ trợ HTTP/2, TLS 1.3 và caching, giảm latency trên toàn cầu khi proxy API.
</details>

---

### Question 80
Bạn muốn tự động phát hiện cấu hình VPC không tuân thủ (route public, SG mở 0.0.0.0/0). Công cụ?

A. AWS Config với managed rules (như `restricted-ssh`, `vpc-sg-open-only-to-authorized-ports`)  
B. CloudFront  
C. Route 53  
D. AWS Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** AWS Config cung cấp managed rule kiểm tra cấu hình mạng, có thể kết hợp remediation tự động.
</details>

---

### Question 76
Bạn cần kiểm tra độ trễ giữa user và ứng dụng trên AWS. Công cụ?

A. AWS Global Accelerator Flow Logs  
B. AWS CloudWatch Synthetics hoặc CloudFront measuring? Maybe answer: CloudFront? Hmm question maybe refer to CloudWatch Synthetics or CloudFront Real User Monitoring? alternative: CloudWatch Synthetics & CloudWatch RUM. We'll choose CloudWatch Synthetics.


### Question 75
Hệ thống IoT gửi dữ liệu MQTT cần xử lý global, latency thấp. Dịch vụ?

A. AWS IoT Core + CloudFront  
B. AWS IoT Core + Global Accelerator? (IoT core global endpoints). choose A with explanation core.

Need refine: IoT Core provides MQTT endpoints global; to reduce latency use IoT Core multi-region + accelerator maybe? simpler: AWS IoT Core multi-region endpoint. We'll craft.


### Question 71
Bạn cần giới hạn băng thông giữa VPC và on-prem. Công cụ?

A. QoS on-prem router  
B. AWS trực tiếp? For Direct Connect, use traffic shaping on CPE.  

Need answer: Use Traffic shaping on network (on-prem). maybe mention AWS Network Firewall? but question? maybe Data? We'll craft better question.

# Networking Services - Exam Questions V2

> 🧠 Mục tiêu: Ôn tập chuyên sâu Networking & Content Delivery cho kỳ thi AWS Certified Cloud Practitioner  
> 📦 Nội dung: 50 câu nền tảng + 30 câu khó (tổng 80 câu) dạng multiple-choice/multiple-response

---

## Phần A - Câu hỏi nền tảng (50 câu)

### Question 1
Amazon VPC giúp bạn làm gì?

A. Tạo mạng riêng biệt trong đám mây AWS  
B. Lưu trữ object  
C. Triển khai serverless function  
D. Quản lý hóa đơn

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** VPC (Virtual Private Cloud) cho phép bạn tạo mạng logic riêng, cấu hình IP range, subnet, routing, security.
</details>

---

### Question 2
Subnet công khai (public subnet) cần gì để truy cập Internet?

A. Route tới Internet Gateway  
B. Route tới NAT Gateway  
C. Route tới Transit Gateway  
D. Route tới Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Public subnet phải có default route (0.0.0.0/0) tới Internet Gateway và instance có public IP/Elastic IP.
</details>

---

### Question 3
Security Group trong VPC hoạt động kiểu?

A. Stateless, áp dụng theo subnet  
B. Stateful, áp dụng theo instance/ENI  
C. Stateless, áp dụng theo VPC  
D. Stateful, áp dụng theo route table

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Security Group là firewall stateful cài trên ENI/instance. Traffic trả về tự động được phép.
</details>

---

### Question 4
Network ACL có đặc điểm nào?

A. Stateful  
B. Áp dụng cho cụm load balancer  
C. Stateless, đánh giá theo thứ tự rule  
D. Chỉ inbound

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** NACL là firewall stateless áp dụng cho subnet, rule được đánh giá tuần tự.
</details>

---

### Question 5
Route 53 là dịch vụ gì?

A. CDN  
B. DNS quản lý và service discovery  
C. Firewall  
D. VPN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Amazon Route 53 là dịch vụ DNS có hỗ trợ routing policy, health checks và service discovery.
</details>

---

### Question 6
CloudFront là?

A. Dịch vụ VPN  
B. Dịch vụ CDN phân phối nội dung qua edge location  
C. Dịch vụ IoT  
D. Dịch vụ monitoring

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Amazon CloudFront là CDN giúp cache và phân phối nội dung với độ trễ thấp.
</details>

---

### Question 7
ELB (Elastic Load Balancer) gồm loại nào dưới đây?

A. Application, Network, Gateway Load Balancer  
B. Public, Private, Hybrid  
C. Standard, Premium  
D. Basic, Advanced

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** AWS có Application LB (Layer 7), Network LB (Layer 4), Gateway LB (appliance), Classic LB (legacy).
</details>

---

### Question 8
Internet Gateway gắn vào đâu?

A. Subnet  
B. Route Table  
C. VPC  
D. Instance

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** Internet Gateway gắn với VPC để cho phép traffic internet khi có route.
</details>

---

### Question 9
VPN Site-to-Site cần thành phần nào ở phía AWS?

A. Internet Gateway  
B. Virtual Private Gateway hoặc Transit Gateway  
C. NAT Gateway  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Site-to-Site VPN thiết lập giữa virtual private gateway (hoặc TGW) và thiết bị VPN on-prem.
</details>

---

### Question 10
NAT Gateway dùng để?

A. Cho phép instance trong private subnet truy cập internet outbound  
B. Nhận inbound từ internet  
C. Tạo VPN  
D. Phân phối CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** NAT Gateway dịch địa chỉ private thành public outbound, cho phép update gói, tải về, nhưng không nhận inbound.
</details>

---

### Question 11
Amazon Global Accelerator khác CloudFront ở điểm nào?

A. Global Accelerator phân phối nội dung tĩnh  
B. Global Accelerator cung cấp IP tĩnh và định tuyến traffic đến endpoint vùng optimised  
C. Global Accelerator chỉ cho IoT  
D. Không khác nhau

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Global Accelerator dùng Anycast IP tĩnh, tối ưu routing layer 4 đến nhiều endpoint (ALB, NLB, EC2).
</details>

---

### Question 12
AWS Direct Connect cung cấp?

A. Kết nối mạng riêng chuyên dụng từ on-prem tới AWS  
B. DNS server  
C. Firewall  
D. CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Direct Connect cung cấp đường truyền vật lý, băng thông ổn định và latency thấp hơn VPN.
</details>

---

### Question 13
Endpoint loại Interface Endpoint (PrivateLink) dùng để?

A. Truy cập dịch vụ AWS qua mạng riêng trong VPC  
B. Tạo route public  
C. Tạo NAT  
D. Quản lý IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Interface Endpoint tạo ENI trong subnet, kết nối riêng tư với dịch vụ AWS/partner thông qua PrivateLink.
</details>

---

### Question 14
Gateway Endpoint hỗ trợ dịch vụ nào?

A. S3 và DynamoDB  
B. RDS và Redshift  
C. Lambda và SNS  
D. EC2 và EKS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Gateway Endpoint chỉ có cho S3 và DynamoDB, giúp truy cập private mà không qua internet.
</details>

---

### Question 15
Transit Gateway dùng để?

A. Kết nối nhiều VPC và on-premises theo mô hình hub-and-spoke  
B. Tạo NAT  
C. Phân phối CDN  
D. Quản lý DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Transit Gateway là hub trung tâm để kết nối hàng trăm VPC, VPN, Direct Connect đơn giản hóa routing.
</details>

---

### Question 16
VPC Peering có hạn chế?

A. Không thể giữa cùng region  
B. Không hỗ trợ chuyển tiếp (transitive) routing  
C. Bắt buộc cùng account  
D. Cần Internet Gateway

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** VPC Peering không hỗ trợ transitive routing; traffic chỉ đi giữa hai VPC peered.
</details>

---

### Question 17
Route 53 health check dùng để?

A. Mã hóa dữ liệu  
B. Giám sát endpoint và kết hợp routing policy failover  
C. Quản lý IAM  
D. Tạo VPC

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Health check kiểm tra endpoint (HTTP, TCP) và kết hợp routing policy để failover khi endpoint unhealthy.
</details>

---

### Question 18
ACM (AWS Certificate Manager) cung cấp?

A. Provision & quản lý SSL/TLS certificates miễn phí sử dụng với CloudFront, ELB, API Gateway  
B. Tạo DNS record  
C. Mã hóa EBS  
D. Quản lý IAM user

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** ACM phát hành certificate miễn phí (public), quản lý renew tự động cho dịch vụ AWS được hỗ trợ.
</details>

---

### Question 19
Elastic IP là?

A. IP tĩnh trong VPC có thể remap giữa instances  
B. IP động  
C. IP private  
D. IP cho S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Elastic IP là IPv4 tĩnh public, có thể gán lại khi instance lỗi để đảm bảo địa chỉ cố định.
</details>

---

### Question 20
Route table trong VPC dùng để?

A. Điều khiển traffic bằng bộ luật inbound/outbound stateful  
B. Xác định hướng đi cho lưu lượng từ subnet đến destination  
C. Quản lý DNS  
D. Lưu log

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Route table mapping destination CIDR tới target (IGW, NAT, VGW, ENI, instance...).
</details>

---

### Question 21
AWS Network Firewall giúp?

A. Dịch vụ tường lửa managed cấp độ VPC, hỗ trợ rule stateful/stateless, inspection layer 3-7  
B. DNS  
C. CDN  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Network Firewall triển khai trong VPC, bảo vệ traffic nội bộ với rule nâng cao (domain, port, IPS).
</details>

---

### Question 22
Private Hosted Zone của Route 53 dùng để?

A. DNS cho internet  
B. DNS nội bộ trong VPC  
C. CDN  
D. VPN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Private Hosted Zone chỉ truy cập được trong VPC được associate, dùng cho DNS nội bộ.
</details>

---

### Question 23
AWS Client VPN dùng để?

A. Kết nối site-to-site  
B. Cung cấp VPN client-based (OpenVPN) cho người dùng truy cập VPC  
C. Quản lý DNS  
D. Mã hóa S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Client VPN là dịch vụ VPN quản lý cho user truy cập VPC qua OpenVPN.
</details>

---

### Question 24
Route 53 Routing Policy nào phân phối lưu lượng dựa trên độ trễ đo được?

A. Simple  
B. Weighted  
C. Latency-based routing  
D. Failover

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** Latency-based routing gửi lưu lượng tới region có độ trễ thấp nhất đo được từ vị trí user.
</details>

---

### Question 25
CloudFront Origin Access Control (OAC) dùng để?

A. Cho phép origin nhận traffic từ mọi nơi  
B. Hạn chế truy cập origin (S3/ALB) chỉ thông qua CloudFront  
C. Mã hóa data  
D. Log traffic

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** OAC/OAI giúp khóa S3/ALB để chỉ CloudFront truy cập, bảo vệ origin khỏi truy cập trực tiếp.
</details>

---

### Question 26
AWS Shield Standard bảo vệ?

A. S3  
B. Dịch vụ public-facing như CloudFront, Route 53, ALB khỏi DDoS cơ bản  
C. IAM  
D. EBS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Shield Standard tự động bảo vệ khỏi DDoS layer 3/4 cho dịch vụ public-facing mà không cần phí.
</details>

---

### Question 27
Access Logs của VPC Flow Logs ghi lại?

A. Log API call  
B. Metadata về traffic (source, dest, port, action) của ENI  
C. Nội dung payload  
D. DNS query

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** VPC Flow Logs ghi nhận metadata mạng của ENI để phân tích traffic, không capture payload.
</details>

---

### Question 28
NAT Instance khác NAT Gateway ở điểm nào?

A. NAT Instance fully managed  
B. NAT Instance yêu cầu tự quản lý, có thể dùng security group, scaling thủ công  
C. NAT Instance rẻ hơn nhưng không hỗ trợ IPv6  
D. Không khác nhau

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** NAT Instance là EC2 tự quản lý; NAT Gateway managed, scale cao, HA. NAT Instance cần bảo trì.
</details>

---

### Question 29
AWS WAF triển khai trên?

A. CloudFront, ALB, API Gateway, App Runner, Cognito, AWS Verified Access  
B. S3  
C. Direct Connect  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** WAF bảo vệ layer 7, gắn vào CloudFront, ALB, API Gateway, AppSync, Cognito, Verified Access.
</details>

---

### Question 30
Elastic Load Balancer hỗ trợ sticky session với?

A. Network Load Balancer  
B. Application Load Balancer dùng cookie  
C. Gateway Load Balancer  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** ALB hỗ trợ sticky session bằng cookie (AWSALB), NLB hỗ trợ bằng source IP (tùy).
</details>

---

### Question 31
AWS PrivateLink giúp?

A. Truy cập dịch vụ public qua internet  
B. Kết nối VPC tới dịch vụ khác thông qua network interface private  
C. Tạo VPN  
D. Lưu log

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** PrivateLink cho phép truy cập cross-VPC/private network tới dịch vụ (AWS/partner/customer) qua ENI private IP.
</details>

---

### Question 32
API Gateway Endpoint type nào phù hợp cho ứng dụng nội bộ?

A. Edge-Optimized  
B. Regional  
C. Private với VPC Endpoint  
D. Public

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** Private endpoint kết hợp VPC endpoint cho phép truy cập API Gateway chỉ trong VPC.
</details>

---

### Question 33
Route 53 Weighted Routing dùng khi?

A. Muốn phân phối traffic theo tỷ lệ (ví dụ 70/30) cho thử nghiệm A/B  
B. Muốn failover  
C. Muốn theo latency  
D. Muốn geolocation

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Weighted routing chọn endpoint theo trọng số, hỗ trợ thử nghiệm, gradual rollout.
</details>

---

### Question 34
AWS Outposts networking cho phép?

A. Sử dụng VPC mở rộng xuống on-prem kết nối qua Direct Connect hoặc VPN  
B. Chỉ chạy offline  
C. Không cần mạng  
D. Mỗi Outposts có Internet Gateway riêng

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Outposts tích hợp VPC, kết nối AWS region qua DX/VPN để mở rộng mạng.
</details>

---

### Question 35
Service nào giúp kiểm tra cấu hình bảo mật VPC?

A. AWS Config với managed rule  
B. CloudFront  
C. CloudWatch  
D. Glacier

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** AWS Config có rule kiểm tra VPC như security group open, flow logs enable, etc.
</details>

---

### Question 36
Amazon Route 53 Resolver DNS Firewall giúp?

A. Lọc DNS query outbound từ VPC dựa trên danh sách cho phép/chặn  
B. Encrypt DNS  
C. Tạo zone mới  
D. Thay thế security group

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** DNS Firewall quản lý domain list, block/allow DNS query từ VPC resolver endpoints.
</details>

---

### Question 37
Để ghi nhật ký truy cập API Gateway, dùng?

A. CloudTrail  
B. Access Logging tới CloudWatch Logs hoặc Kinesis  
C. Route 53  
D. AWS Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** API Gateway access logging gửi log tới CloudWatch Logs/Kinesis/Firehose để phân tích.
</details>

---

### Question 38
Direct Connect kết hợp VPN được gọi là?

A. VPN Gateway  
B. Direct Connect Gateway  
C. VPN over DX (hybrid redundancies)  
D. PrivateLink

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** Kết hợp VPN qua Direct Connect để back up, đảm bảo mã hóa end-to-end.
</details>

---

### Question 39
CloudFront hỗ trợ compress nội dung?

A. Không  
B. Có, hỗ trợ Gzip/Brotli khi client hỗ trợ  
C. Chỉ Gzip  
D. Chỉ Brotli

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** CloudFront tự động nén Gzip/Brotli với header Accept-Encoding phù hợp.
</details>

---

### Question 40
Feature nào của ALB hỗ trợ routing theo path/host?

A. Listener Rules  
B. Target Group Stickiness  
C. Connection Draining  
D. Cross-Zone Load Balancing

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Listener rules của ALB định tuyến dựa theo path, host, header, method.
</details>

---

### Question 41
AWS VPN CloudHub dùng để?

A. Kết nối nhiều site on-prem với Virtual Private Gateway qua VPN (hub-and-spoke)  
B. Tạo VPC  
C. DNS  
D. CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** VPN CloudHub cho phép nhiều site VPN kết nối qua VGW acting as hub.
</details>

---

### Question 42
Route 53 Geolocation routing dùng khi?

A. Muốn routing theo địa lý người dùng  
B. Muốn failover  
C. Muốn theo latency  
D. Muốn weighted

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Geolocation routing hướng traffic dựa trên vị trí địa lý của user.
</details>

---

### Question 43
AWS Verified Access giúp?

A. Cung cấp Zero Trust access đến ứng dụng nội bộ qua policy dựa trên identity, device, context  
B. Tạo VPC  
C. CDN  
D. Hóa đơn

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Verified Access dùng để cung cấp secure access cho ứng dụng mà không cần VPN truyền thống.
</details>

---

### Question 44
AWS Firewall Manager hỗ trợ?

A. Quản lý tập trung WAF, Shield Advanced, Network Firewall policies across accounts  
B. Mã hóa  
C. Backup  
D. Monitor billing

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Firewall Manager giúp áp dụng policy firewall nhất quán nhiều account qua AWS Organizations.
</details>

---

### Question 45
S3 Static Website kết hợp CloudFront cần lưu ý?

A. Origin phải public hoặc dùng OAC/OAI  
B. Không cần SSL  
C. CloudFront không hỗ trợ HTTPS  
D. Không thể cache

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** S3 static website có thể behind CloudFront, nên dùng Origin Access to bảo vệ S3.
</details>

---

### Question 46
Route 53 Alias record khác CNAME ở chỗ?

A. Alias có thể trỏ tới endpoint AWS (ALB, CloudFront, API Gateway) ở root domain, miễn phí query  
B. Alias không hỗ trợ root domain  
C. Alias không hỗ trợ health check  
D. Giống nhau

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Alias record có thể ở apex domain, trỏ tới resource AWS, không tốn phí truy vấn.
</details>

---

### Question 47
Private DNS cho Interface Endpoint giúp?

A. Cho phép dùng tên dịch vụ AWS thay vì DNS riêng  
B. Bật Internet  
C. Mã hóa  
D. Tạo NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Private DNS map domain service AWS sang private IP endpoint, giúp truy cập như bình thường.
</details>

---

### Question 48
Bạn muốn thu thập log truy cập CloudFront chi tiết. Dùng?

A. CloudWatch Logs  
B. Standard Access Log hoặc Realtime Log (Kinesis Data Streams/Firehose)  
C. CloudTrail  
D. S3 Inventory

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** CloudFront hỗ trợ access log (S3) và real-time log streaming.
</details>

---

### Question 49
AWS App Mesh hỗ trợ?

A. Service mesh quản lý traffic giữa microservices chạy trên ECS, EKS, EC2  
B. CDN  
C. DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** App Mesh là service mesh, cung cấp observability, routing, retry, circuit breaking.
</details>

---

### Question 50
Elastic Load Balancing cross-zone balancing giúp?

A. Chỉ phân phối trong cùng AZ  
B. Phân phối request đều giữa instances ở các AZ khác nhau  
C. Không sử dụng health check  
D. Chỉ dùng cho NLB

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Cross-zone load balancing chuyển traffic giữa AZ để cân bằng, giảm lệ thuộc một AZ.
</details>

---

## Phần B - Câu hỏi khó (30 câu)

### Question 51
Bạn có multi-account architecture muốn chia sẻ VPC central networking. Giải pháp tốt?

A. VPC Peering từng cặp giữa tất cả account  
B. AWS Transit Gateway kết hợp AWS Organizations và Resource Access Manager để share VPC/subnet  
C. CloudFront  
D. Direct Connect gateway

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Transit Gateway làm hub kết nối nhiều VPC/account. RAM chia sẻ TGW và subnets trung tâm.
</details>

---

### Question 52
Bạn cần Zero Trust remote access không VPN, tích hợp kiểm tra thiết bị. Chọn?

A. Client VPN  
B. AWS Verified Access kết hợp IdP và device posture  
C. Direct Connect  
D. Route 53

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Verified Access cung cấp Zero Trust, policy dựa identity/device/context, không yêu cầu VPN truyền thống.
</details>

---

### Question 53
Ứng dụng sử dụng ALB -> ECS Fargate trong private subnet. Làm sao để ALB internet-facing?

A. Mở security group outbound  
B. Đặt ALB trong public subnet (route IGW), ECS trong private, security group cho phép traffic  
C. Đặt ECS public  
D. Dùng NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** ALB cần subnet public với route IGW, target (ECS) private, security group ALB->ECS.
</details>

---

### Question 54
Bạn muốn filter HTTP request dựa trên header tùy chỉnh trước khi vào backend. Giải pháp?

A. Network Load Balancer  
B. Application Load Balancer với listener rule và AWS WAF cho inspection nâng cao  
C. NAT Gateway  
D. Route 53

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** ALB layer 7 có thể route theo header, kết hợp WAF cho rule chi tiết (header inspection).
</details>

---

### Question 55
Dịch vụ nào giúp publish private API mà đối tác truy cập qua PrivateLink?

A. API Gateway Private Endpoint + VPC Endpoint Service (PrivateLink)  
B. CloudFront  
C. Route 53  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** API Gateway Private endpoint + VPC endpoint service cho phép đối tác connect qua PrivateLink.
</details>

---

### Question 56
Bạn cần multi-region active-active cho API, ẩn latency, failover tự động. Kết hợp nào?

A. API Gateway Regional API + Route 53 latency routing + health checks  
B. CloudFront  
C. ALB  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Deploy API ở nhiều region, dùng latency routing và health check failover.
</details>

---

### Question 57
Workload IoT gửi hàng trăm nghìn msg/s tới Kinesis trong VPC riêng, cần giảm latency cross-region. Giải pháp?

A. Sử dụng VPC endpoint + Global Accelerator with TCP endpoint group  
B. CloudFront  
C. NAT  
D. VPN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Global Accelerator cung cấp IP tĩnh, routing edge, chuyển vào VPC endpoint (TCP) giảm latency.
</details>

---

### Question 58
Ứng dụng gaming toàn cầu yêu cầu UDP traffic, latency cực thấp. Bạn chọn?

A. Application Load Balancer  
B. Network Load Balancer kết hợp Global Accelerator  
C. CloudFront  
D. Route 53 simple

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** NLB hỗ trợ UDP, Global Accelerator tối ưu định tuyến toàn cầu, IP tĩnh, failover nhanh.
</details>

---

### Question 59
Bạn cần centralize log truy cập VPC trên nhiều account. Giải pháp?

A. Bật VPC Flow Logs từng account ghi riêng  
B. Dùng VPC Flow Logs gửi sang centralized S3/CloudWatch qua CloudWatch Logs subscription + Kinesis Firehose  
C. CloudTrail  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Dùng tổ chức flow logs và đẩy log tới account trung tâm qua Firehose/S3.
</details>

---

### Question 60
Bạn muốn migrate từ nhiều VPN sang Transit Gateway nhưng vẫn cần IPv6. Lưu ý?

A. TGW chưa hỗ trợ IPv6  
B. TGW hỗ trợ IPv6 cho VPN/attachment, cần bật route table IPv6  
C. Không cần làm gì  
D. Dùng NAT64

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** TGW support IPv6 (trong attachment VPC/VPN) nhưng cần cấu hình route table IPv6.
</details>

---

### Question 61
Để chặn tải file độc hại dựa trên danh sách domain xấu cho toàn bộ VPC?

A. WAF  
B. Route 53 Resolver DNS Firewall với danh sách block  
C. CloudFront  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** DNS Firewall chặn domain nguy hiểm, áp dụng cho DNS query outbound.
</details>

---

### Question 62
Bạn muốn gán public IP cho instance trong private subnet? 

A. Không thể  
B. Dùng Elastic IP attach ENI trong private subnet, route qua NAT  
C. Tạo public subnet  
D. Dùng Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Private subnet không có route IGW, public IP không hoạt động; cần đặt instance ở public subnet.
</details>

---

### Question 63
Dự án compliance yêu cầu log DNS nội bộ. Công cụ?

A. Route 53 Resolver Query Logging  
B. CloudTrail  
C. CloudFront Logs  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Query Logging ghi lại DNS query từ VPC resolver.
</details>

---

### Question 64
Ứng dụng hybrid cần on-prem network truy cập S3 private với băng thông cao. Kết hợp?

A. Public Internet  
B. Direct Connect với Transit Gateway + S3 Gateway Endpoint trong VPC  
C. VPN site-to-site  
D. CloudFront

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Sử dụng DX kết nối vào VPC, route tới S3 qua Gateway Endpoint, traffic không ra internet.
</details>

---

### Question 65
Bạn muốn test blue/green DNS cutover an toàn. Route 53 hỗ trợ?

A. Alias  
B. Weighted routing (90/10) chuyển dần traffic  
C. CloudFront  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Weighted routing cho phép phân bổ traffic theo tỷ lệ, chuyển dần.
</details>

---

### Question 66
Workload multi-region cần CDN với geo-restriction. Thiết lập?

A. CloudFront với geo restriction whitelist/blacklist, origin đa region  
B. Route 53  
C. NAT  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CloudFront hỗ trợ geo restriction, kết hợp origin failover multi-region.
</details>

---

### Question 67
Ứng dụng microservices cần service discovery nội bộ. Chọn?

A. Route 53 Private Hosted Zone + Cloud Map  
B. CloudFront  
C. NAT  
D. Shield

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** AWS Cloud Map sử dụng Route 53 để đăng ký dịch vụ, hỗ trợ DNS/HTTP discovery.
</details>

---

### Question 68
Bạn có requirement chặn IP phạm vi lớn (CIDR) và geo-block ngay trên edge. Dịch vụ?

A. CloudFront + AWS WAF (IP sets, geo match)  
B. Security Group  
C. NACL  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** WAF gắn CloudFront áp dụng rule IP set và geo-block ở edge.
</details>

---

### Question 69
Để có HA cao cho Direct Connect, nên?

A. Chỉ dùng một kết nối duy nhất  
B. Thiết lập hai kết nối DX khác location + một VPN backup  
C. Dùng CloudFront  
D. Chỉ VPN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Best practice: hai DX tại location khác nhau, thêm VPN dự phòng.
</details>

---

### Question 70
Bạn muốn terraform hạ tầng networking, track drift. Công cụ?

A. CloudFormation Guard  
B. AWS CloudFormation + Drift Detection hoặc AWS CDK  
C. S3  
D. Route 53

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** CloudFormation/CDK mô tả hạ tầng, drift detection phát hiện khác biệt so với template.
</details>

---

### Question 71
Dịch vụ nào hỗ trợ định tuyến BGP với lưu lượng encrypted toàn phần?

A. Site-to-Site VPN (dynamic routing)  
B. Client VPN  
C. PrivateLink  
D. CloudFront

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** VPN site-to-site hỗ trợ BGP (dynamic), traffic encrypt IPsec.
</details>

---

### Question 72
Muốn logging mọi request đi qua ALB và sẵn sàng phân tích real-time?

A. Enable ALB Access Logs tới S3 + Kinesis Data Firehose + Analytics  
B. CloudTrail  
C. Shield  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** ALB access logs gửi tới S3; kết hợp Firehose/Analytics phân tích real-time/quasi real-time.
</details>

---

### Question 73
Ứng dụng cần private connectivity giữa VPC (Account A) và dịch vụ chạy ECS Fargate ở VPC Account B. Giải pháp?

A. Public internet  
B. PrivateLink (VPC Endpoint Service) expose dịch vụ ở account B, account A tạo interface endpoint  
C. VPC peering  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** PrivateLink cho phép expose service qua NLB endpoint, consumer tạo interface endpoint.
</details>

---

### Question 74
Bạn cần tách traffic API đọc/ghi qua các endpoint khác nhau nhưng cùng tên miền. Route 53 hỗ trợ?

A. Weighted  
B. Geolocation  
C. Multi-Value Answer  
D. Không, cần ALB path-based

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** D  
**Giải thích:** Route 53 không phân biệt method; cần ALB/API Gateway path-based/Stage.
</details>

---

### Question 75
Hybrid network có Direct Connect và VPN. Bạn muốn route ưu tiên DX, fallback VPN. Cách?

A. Route static  
B. BGP thiết lập với DX có số AS path ngắn hơn, VPN longer (VPN làm backup)  
C. Không thể  
D. Dùng CloudFront

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** BGP ưu tiên path với weight/AS path; cấu hình DX primary, VPN secondary.
</details>

---

### Question 76
Bạn có yêu cầu segment traffic giữa microservices trong cùng VPC, kiểm soát east-west. Công cụ?

A. Security Group kết hợp AWS App Mesh và Network Firewall phân tầng  
B. CloudFront  
C. IAM  
D. Route 53

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Dùng SG cho microservice, App Mesh kiểm soát traffic layer 7, Network Firewall chặn subnet-level.
</details>

---

### Question 77
Muốn publish dữ liệu realtime (WebSocket) toàn cầu độ trễ thấp. Kết hợp?

A. API Gateway WebSocket + CloudFront không hỗ trợ  
B. API Gateway WebSocket + AWS Global Accelerator (custom routing) hoặc CloudFront nếu HTTP(S)  
C. Direct Connect  
D. Route 53 Simple

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** API Gateway WebSocket cung cấp endpoint, Global Accelerator tối ưu routing TCP/TLS.
</details>

---

### Question 78
Bạn cần expose dịch vụ nội bộ ra internet qua CloudFront nhưng policy yêu cầu TLS 1.3. Thực hiện?

A. CloudFront hỗ trợ TLS 1.3 khi enable Security Policy phù hợp (TLSv1.2_2021, TLSv1.3_2021...)  
B. Không thể  
C. Dùng ALB  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CloudFront hỗ trợ TLS 1.3 với các security policy mới.
</details>

---

### Question 79
Bạn muốn kiểm soát truy cập dựa trên thiết bị (managed/unmanaged) trước khi vào ứng dụng. Dịch vụ nào?

A. AWS Verified Access  
B. Shield  
C. NAT Gateway  
D. Direct Connect

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Verified Access evaluation dựa identity, device posture, context.
</details>

---

### Question 80
Ứng dụng streaming video toàn cầu yêu cầu cache edge và chuyển đổi protocol. Kết hợp tối ưu?

A. CloudFront với MediaPackage/MediaLive origin, sử dụng RTMP -> HLS/DASH, bảo vệ bằng Signed URL  
B. Direct Connect  
C. S3  
D. VPN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CloudFront + MediaPackage chuyển đổi streaming protocol, cache edge, Signed URL bảo vệ nội dung.
</details>

---

