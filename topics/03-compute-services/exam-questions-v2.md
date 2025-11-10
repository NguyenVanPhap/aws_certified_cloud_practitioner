# Compute Services - Exam Questions V2

> 🧠 Mục tiêu: Ôn tập chuyên sâu Compute services cho kỳ thi AWS Certified Cloud Practitioner  
> 📦 Nội dung: 50 câu nền tảng + 30 câu khó (tổng 80 câu) dạng multiple-choice/multiple-response

---

## Phần A - Câu hỏi nền tảng (50 câu)

### Question 1
Dịch vụ nào cung cấp máy chủ ảo trong AWS?

A. Amazon RDS  
B. Amazon EC2  
C. Amazon S3  
D. AWS Glue

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** EC2 (Elastic Compute Cloud) cung cấp máy chủ ảo có thể tùy biến cấu hình, hệ điều hành và cách triển khai.
</details>

---

### Question 2
Dịch vụ nào cho phép chạy code mà không quản lý máy chủ?

A. Amazon ECS  
B. AWS Lambda  
C. Amazon Lightsail  
D. AWS Batch

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Lambda là mô hình serverless, AWS quản lý máy chủ, scaling và hệ điều hành, bạn chỉ triển khai function.
</details>

---

### Question 3
Loại giá EC2 nào phù hợp cho workload ngắn hạn, không đoán trước được?

A. On-Demand  
B. Reserved Instances  
C. Savings Plans  
D. Dedicated Hosts

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** On-Demand cho phép trả theo giây với tính linh hoạt cao, không cần cam kết dài hạn.
</details>

---

### Question 4
Cảnh báo 2 phút trước khi thu hồi năng lực là đặc điểm của mô hình giá nào?

A. Dedicated Hosts  
B. Spot Instances  
C. On-Demand  
D. Savings Plans

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Spot Instances rẻ nhất nhưng có thể bị thu hồi, AWS cung cấp cảnh báo 2 phút trước khi kết thúc.
</details>

---

### Question 5
AWS Fargate được mô tả đúng nhất là gì?

A. Dịch vụ cơ sở dữ liệu không máy chủ  
B. Compute engine serverless cho container  
C. Hệ thống caching phân tán  
D. Persistent block storage

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Fargate cho phép chạy container với ECS/EKS mà không phải quản lý EC2 instances.
</details>

---

### Question 6
Giới hạn thời gian tối đa cho một function Lambda là bao lâu?

A. 5 phút  
B. 10 phút  
C. 15 phút  
D. 30 phút

<details>
<summary><strong>Answer: C</strong></summary>

**Giải thích:** Lambda có timeout tối đa 15 phút cho mỗi lần chạy.
</details>

---

### Question 7
Elastic Beanstalk cung cấp lợi ích nào?

A. Quản lý toàn bộ hạ tầng, triển khai ứng dụng PaaS  
B. Lưu trữ đối tượng với độ bền 11 số 9  
C. Quản lý secrets cho ứng dụng  
D. Dịch vụ streaming dữ liệu real-time

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Elastic Beanstalk là PaaS giúp triển khai, scale, theo dõi ứng dụng mà không cần quản trị chi tiết hạ tầng.
</details>

---

### Question 8
AMI (Amazon Machine Image) dùng để làm gì?

A. Lưu trữ log ứng dụng  
B. Template khởi tạo EC2 instance  
C. Mã hóa lưu lượng mạng  
D. Tạo VPC mới

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** AMI chứa hệ điều hành, cấu hình và phần mềm cần thiết để khởi động EC2 instance.
</details>

---

### Question 9
Dịch vụ nào hỗ trợ chạy container với Kubernetes được quản lý?

A. AWS Lambda  
B. Amazon EKS  
C. AWS Batch  
D. Amazon Lightsail

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Amazon EKS (Elastic Kubernetes Service) là dịch vụ Kubernetes managed trên AWS.
</details>

---

### Question 10
EC2 Auto Scaling giúp đạt điều gì?

A. Phân phối traffic giữa các VPC  
B. Tăng giảm số lượng EC2 theo nhu cầu  
C. Sao lưu dữ liệu lên S3  
D. Nâng cấp phiên bản Lambda tự động

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Auto Scaling theo dõi các chỉ số (như CPU) để scale in/out EC2 instances đảm bảo hiệu năng và chi phí.
</details>

---

### Question 11
EC2 Instance Store có đặc điểm nào?

A. Dữ liệu bền vững sau khi dừng instance  
B. Dữ liệu mất khi instance stop hoặc terminate  
C. Phải trả phí riêng như EBS  
D. Dùng được cho mọi loại instance

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Instance Store là lưu trữ tạm, dữ liệu sẽ mất khi dừng/terminate instance.
</details>

---

### Question 12
Elastic Load Balancer hỗ trợ lợi ích nào?

A. Mã hóa dữ liệu ở trạng thái nghỉ  
B. Phân phối traffic đến nhiều EC2 để tăng HA  
C. Sao lưu dữ liệu EC2  
D. Tạo snapshot tự động

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** ELB phân phối traffic để nâng cao fault tolerance và availability.
</details>

---

### Question 13
Tính năng nào của Lambda giúp tích hợp sự kiện?

A. Lambda Layers  
B. Custom runtime  
C. Event source mapping  
D. SnapStart

<details>
<summary><strong>Answer: C</strong></summary>

**Giải thích:** Event source mapping cho phép Lambda nhận sự kiện từ SQS, Kinesis, DynamoDB Streams một cách tự động.
</details>

---

### Question 14
Dịch vụ compute nào phù hợp cho game backend cần session dài và cấu hình tùy chỉnh?

A. AWS Lambda  
B. Amazon EC2  
C. AWS Fargate  
D. Amazon SQS

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** EC2 cung cấp toàn quyền kiểm soát hệ điều hành, phiên lâu dài, thích hợp workload stateful.
</details>

---

### Question 15
Phát biểu nào đúng về Reserved Instances (RI)?

A. Không cần cam kết thời gian  
B. Có thể tiết kiệm đến 72% so với On-Demand  
C. Bị giới hạn vùng sử dụng  
D. Không chuyển nhượng được

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** RI yêu cầu cam kết 1 hoặc 3 năm, đổi lại giảm giá đáng kể so với On-Demand.
</details>

---

### Question 16
Elastic Beanstalk hỗ trợ những ngôn ngữ nào sau đây? (Chọn hai)

A. Node.js  
B. Go  
C. COBOL  
D. Swift  
E. Ruby

<details>
<summary><strong>Answer: A, E</strong></summary>

**Giải thích:** Beanstalk hỗ trợ Node.js, Ruby, Python, Java, .NET, Go, PHP. COBOL và Swift không nằm trong danh sách mặc định.
</details>

---

### Question 17
Lightsail phù hợp nhất cho trường hợp nào?

A. Workload doanh nghiệp cần tùy biến sâu  
B. Website đơn giản hoặc ứng dụng nhỏ cần triển khai nhanh  
C. Ứng dụng máy học real-time  
D. Workload HPC

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Lightsail cung cấp gói đơn giản, giá cố định, thích hợp cho website nhỏ và ứng dụng đơn giản.
</details>

---

### Question 18
AWS Batch hỗ trợ điều gì?

A. Chạy batch computing jobs ở quy mô lớn  
B. Triển khai ứng dụng web serverless  
C. Quản lý luồng dữ liệu thời gian thực  
D. Cung cấp môi trường no-code

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** AWS Batch lên lịch và quản lý batch jobs sử dụng EC2 hoặc Fargate.
</details>

---

### Question 19
Elastic Beanstalk sử dụng dịch vụ AWS nào để lưu cấu hình môi trường?

A. AWS S3  
B. AWS Config  
C. AWS Systems Manager Parameter Store  
D. AWS CloudFormation

<details>
<summary><strong>Answer: D</strong></summary>

**Giải thích:** Beanstalk sử dụng CloudFormation để triển khai và quản lý tài nguyên môi trường.
</details>

---

### Question 20
Tùy chọn compute nào cung cấp GPU cho workloads ML?

A. C5 instances  
B. T3 instances  
C. P4 instances  
D. M5 instances

<details>
<summary><strong>Answer: C</strong></summary>

**Giải thích:** P-series là GPU instances tối ưu cho machine learning và HPC.
</details>

---

### Question 21
Dịch vụ nào cung cấp môi trường phát triển đám mây tích hợp sẵn compute?

A. AWS Cloud9  
B. Amazon WorkSpaces  
C. AWS Lambda  
D. AWS Batch

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Cloud9 là IDE dựa trên cloud, chạy trên EC2 và có terminal, editor tích hợp.
</details>

---

### Question 22
Chức năng Elastic IP trong EC2 nhằm?

A. Cung cấp địa chỉ IP tĩnh có thể gán cho instances  
B. Tạo VPC mới  
C. Mã hóa lưu lượng giữa instances  
D. Tạo DNS riêng cho S3

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Elastic IP là địa chỉ IPv4 tĩnh, có thể remap giữa instances để tăng HA.
</details>

---

### Question 23
AWS Outposts cung cấp lợi ích nào?

A. Mang dịch vụ AWS xuống on-premises  
B. Sao lưu dữ liệu sang Glacier  
C. Cung cấp firewall on-premises  
D. Quản lý CI/CD pipeline

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Outposts đưa hạ tầng AWS tới trung tâm dữ liệu của khách hàng để chạy dịch vụ AWS tại chỗ.
</details>

---

### Question 24
Dịch vụ nào giúp chạy container bằng cách sử dụng API Docker thuần?

A. AWS Lambda  
B. Amazon ECS  
C. Amazon EFS  
D. AWS Step Functions

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** ECS hỗ trợ Docker CLI, API để quản lý container trên AWS.
</details>

---

### Question 25
So với On-Demand, Savings Plans mang lại lợi ích gì?

A. Không cần cam kết  
B. Linh hoạt giữa các dịch vụ compute (ví dụ EC2, Fargate, Lambda)  
C. Chi phí cao hơn  
D. Chỉ dùng được cho một loại instance

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Compute Savings Plans tiết kiệm chi phí khi cam kết sử dụng (USD/giờ) và linh hoạt giữa các dịch vụ compute.
</details>

---

### Question 26
OpenSearch Managed Service thuộc nhóm dịch vụ nào?

A. Compute  
B. Database chuyên dụng  
C. Analytics/Streaming  
D. AI/ML

<details>
<summary><strong>Answer: C</strong></summary>

**Giải thích:** Amazon OpenSearch Service là dịch vụ tìm kiếm và phân tích, không thuộc compute.
</details>

---

### Question 27
Dịch vụ nào cung cấp orchestrator container tương thích Kubernetes?

A. Amazon ECS  
B. Amazon EKS  
C. AWS Batch  
D. AWS Glue

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Amazon EKS vận hành cụm Kubernetes được quản lý, hỗ trợ các API chuẩn Kubernetes.
</details>

---

### Question 28
Lifecycle hook trong Auto Scaling Group dùng để?

A. Bảo vệ secrets  
B. Thực thi hành động tùy chỉnh trước khi instance đưa vào/ra phục vụ  
C. Sao lưu EBS  
D. Tạo snapshot RDS

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Lifecycle hooks cho phép chạy script hoặc thông báo trước khi instance chuyển trạng thái InService hoặc Terminating.
</details>

---

### Question 29
Instance profile gắn với EC2 nhằm mục đích nào?

A. Cấp quyền IAM cho instance truy cập tài nguyên AWS  
B. Mã hóa lưu lượng VPC  
C. Quản lý user đăng nhập  
D. Tạo backup tự động

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Instance profile chứa IAM role, cung cấp credentials tạm thời cho ứng dụng trên EC2 truy cập AWS APIs.
</details>

---

### Question 30
Khi nào nên chọn Dedicated Host?

A. Khi cần giá rẻ nhất  
B. Khi cần tuân thủ license hoặc yêu cầu audit về placement  
C. Khi workload stateless  
D. Khi cần serverless

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Dedicated Host cung cấp phần cứng dành riêng đáp ứng yêu cầu về license hoặc tuân thủ.
</details>

---

### Question 31
Tính năng nào giúp EC2 giảm downtime khi deployment?

A. Placement Groups  
B. Blue/Green deployment  
C. Route 53 health checks  
D. Elastic Fabric Adapter

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Blue/Green deployment tạo hai môi trường song song, chuyển traffic khi môi trường mới sẵn sàng.
</details>

---

### Question 32
Amazon Machine Learning căn bản cho compute là?

A. EC2 DLAMI  
B. Amazon Lex  
C. Amazon Polly  
D. Amazon Forecast

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Deep Learning AMI (DLAMI) là AMI được tối ưu cho ML/DL, chứa frameworks và drivers.
</details>

---

### Question 33
Scaling theo lịch trình (scheduled scaling) nên dùng khi?

A. Có pattern sử dụng dự đoán trước  
B. Workload hoàn toàn bất ngờ  
C. Không muốn scale  
D. Cần batch job theo event

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Scheduled scaling cấu hình trước thời điểm scale dựa vào pattern thời gian.
</details>

---

### Question 34
Chọn hai dịch vụ compute có thể chạy container.

A. AWS Lambda  
B. AWS Batch  
C. Amazon ECS  
D. Amazon SQS  
E. Amazon Aurora

<details>
<summary><strong>Answer: B, C</strong></summary>

**Giải thích:** AWS Batch và Amazon ECS cả hai đều chạy container; Lambda không phải nền tảng container tổng quát; SQS/Aurora không phải compute.
</details>

---

### Question 35
EC2 Launch Template cung cấp gì so với Launch Configuration?

A. Hỗ trợ nhiều phiên bản, versioning  
B. Giảm chi phí  
C. Cho phép chạy Lambda  
D. Yêu cầu ít quyền IAM hơn

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Launch Template hỗ trợ version, tùy biến mới như T2/T3 Unlimited, tagging instance.
</details>

---

### Question 36
Khả năng scale của Lambda dựa trên?

A. Số lượng subnet trong VPC  
B. Số lượng request incoming (concurrency)  
C. Số lượng AZ  
D. Kích thước AMI

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Lambda scale theo nhu cầu concurrency, AWS tự động bổ sung instance ảo cho mỗi request mới.
</details>

---

### Question 37
Tính năng nào giảm cold start cho Lambda Java?

A. Provisioned Concurrency  
B. Lambda Layers  
C. CloudWatch Logs  
D. Alias

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Provisioned Concurrency giữ sẵn instance thực thi, giảm cold start cho runtime nặng như Java.
</details>

---

### Question 38
S3 Event có thể kích hoạt Lambda qua cơ chế nào?

A. S3 lifecycle rule  
B. S3 event notification  
C. S3 cross-region replication  
D. S3 inventory report

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** S3 Event Notifications cấu hình để gọi Lambda khi có PUT/POST/DELETE.
</details>

---

### Question 39
EC2 Spot Fleet là gì?

A. Nhóm EC2 chạy Dedicated Hosts  
B. Tập hợp Spot Instances được quản lý tập trung  
C. Dịch vụ caching  
D. Chương trình khuyến mãi

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Spot Fleet cho phép quản lý nhiều Spot instances, đặt mục tiêu công suất, đa dạng hóa loại instance.
</details>

---

### Question 40
Sự khác nhau giữa ECS EC2 launch type và Fargate launch type?

A. EC2 launch type dùng máy chủ vật lý  
B. Fargate launch type không cần quản lý EC2, trả theo CPU/RAM   
C. Fargate yêu cầu mua Reserved Instances  
D. EC2 launch type không hỗ trợ scaling

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** ECS EC2 launch type cần quản lý EC2 cluster, Fargate thì serverless trả phí theo tài nguyên container.
</details>

---

### Question 41
Elastic Inference giúp gì cho workload ML?

A. Tự động điều chỉnh learning rate  
B. Gắn gia tốc phần inference vào EC2/EKS  
C. Tối ưu pipeline CI/CD  
D. Phân tích log

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Elastic Inference cung cấp GPU inference accelerator rẻ hơn so với dùng GPU lớn toàn phần.
</details>

---

### Question 42
Chức năng chính của AWS Step Functions trong kiến trúc serverless?

A. Dịch vụ compute độc lập  
B. Orchestrator điều phối nhiều Lambda và dịch vụ khác  
C. Dịch vụ caching  
D. Dịch vụ messaging

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Step Functions xây dựng workflow serverless, kết nối Lambda, ECS, DynamoDB, SQS...
</details>

---

### Question 43
Lambda có thể truy cập tài nguyên trong VPC bằng cách nào?

A. Gán Subnet và Security Group cho function  
B. Sử dụng API Gateway  
C. Không thể  
D. Tạo IAM user riêng

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Có thể cấu hình Lambda chạy trong VPC bằng cách gán subnet & security group, AWS sẽ tạo ENI.
</details>

---

### Question 44
AWS Global Accelerator có thể dùng cho trường hợp nào kết hợp compute?

A. Tăng tốc truy cập ứng dụng chạy trên EC2 ở nhiều Region  
B. Sao lưu Lambda  
C. Tối ưu chi phí Fargate  
D. Tạo AMI

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Global Accelerator cung cấp địa chỉ IP tĩnh toàn cầu, định tuyến lưu lượng tối ưu đến các endpoint (EC2, ALB).
</details>

---

### Question 45
Đâu là lựa chọn đúng khi cần script automation thao tác với EC2?

A. AWS CLI hoặc SDK  
B. AWS IQ  
C. AWS Artifact  
D. Amazon WorkMail

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** AWS CLI/SDK cho phép script automation thao tác với EC2 và các dịch vụ khác.
</details>

---

### Question 46
Thông số nào của EC2 giúp tăng thông lượng mạng?

A. Elastic Fabric Adapter (EFA)  
B. Placement Group loại Spread  
C. CloudFormation Stack  
D. IAM Policy

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** EFA cung cấp low latency, high throughput networking, thích hợp HPC và ML.
</details>

---

### Question 47
Sử dụng AWS Budgets cho compute nhằm?

A. Tự động scale EC2  
B. Giám sát và cảnh báo chi phí compute vượt ngưỡng  
C. Mã hóa EBS  
D. Quản lý AMI

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** AWS Budgets thiết lập ngưỡng chi phí/usage, cảnh báo khi vượt cho compute và dịch vụ khác.
</details>

---

### Question 48
Khi nào nên dùng Lambda@Edge?

A. Khi cần chạy function gần CloudFront edge location  
B. Khi muốn truy cập GPU  
C. Khi cần batch jobs dài  
D. Khi cần backup dữ liệu

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Lambda@Edge chạy function tại edge để xử lý request/response CloudFront với độ trễ thấp.
</details>

---

### Question 49
AWS Serverless Application Model (SAM) dùng để?

A. Viết ứng dụng serverless với template YAML  
B. Quản lý container ECS  
C. Tạo AMI  
D. Quản lý RI

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** SAM mở rộng CloudFormation để định nghĩa và triển khai ứng dụng serverless (Lambda, API Gateway, Step Functions).
</details>

---

### Question 50
Phần nào trong compute yêu cầu quản lý patches hệ điều hành?

A. Lambda  
B. Fargate  
C. EC2  
D. Step Functions

<details>
<summary><strong>Answer: C</strong></summary>

**Giải thích:** Với EC2, khách hàng chịu trách nhiệm quản lý hệ điều hành, cập nhật bảo mật và patches.
</details>

---

## Phần B - Câu hỏi khó (30 câu)

### Question 51
Bạn cần batch job chạy hàng đêm, thời gian 2 giờ, vẫn phải hoàn thành trước 6h sáng nhưng có thể bị gián đoạn. Cách tối ưu chi phí nhất?

A. Chạy On-Demand EC2 trong Auto Scaling Group  
B. Dùng AWS Batch với Spot Instances và thiết lập retry  
C. Dùng Lambda với Provisioned Concurrency  
D. Dùng Lightsail

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** AWS Batch với Spot Instances giảm chi phí, job có thể retry nếu bị gián đoạn, đảm bảo hoàn thành theo lịch.
</details>

---

### Question 52
Workload cần socket UDP tùy chỉnh, throughput cao, độ trễ thấp (HPC). Placement Group nào phù hợp?

A. Spread Placement Group  
B. Cluster Placement Group  
C. Partition Placement Group  
D. Không cần placement group

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Cluster Placement Group đặt instances gần nhau trong cùng AZ, tối ưu low-latency networking cho HPC.
</details>

---

### Question 53
Bạn vận hành microservices gồm một số service event-driven, số khác cần versioning và rollout dần. Kết hợp nào hiệu quả?

A. Lambda với EventBridge + ECS với CodeDeploy Blue/Green  
B. Lambda với S3 replication  
C. EC2 Reserved Instances + Lightsail  
D. Lambda + DynamoDB global table

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** EventBridge phối hợp events cho Lambda, CodeDeploy Blue/Green hỗ trợ rollout dần cho dịch vụ container ECS.
</details>

---

### Question 54
Ứng dụng legacy cần Windows Server 2012 với license theo core. Cách tối ưu tuân thủ?

A. EC2 On-Demand với Dedicated Host  
B. Lambda  
C. Fargate  
D. Lightsail

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Dedicated Host cho phép gắn license riêng, đảm bảo compliance với license theo core/cpu.
</details>

---

### Question 55
Bạn cần đảm bảo workload 24/7, cost tối ưu, nhưng workload có pattern dự đoán. Giải pháp tốt?

A. 100% On-Demand  
B. Kết hợp Reserved Instances/Savings Plans cho baseline + Auto Scaling On-Demand cho peak  
C. 100% Spot  
D. Chỉ dùng Lambda

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Dùng RI/Savings Plan cho workload cơ bản (steady-state), On-Demand/Spot cho phần biến động.
</details>

---

### Question 56
ECS chạy trên EC2 bị gián đoạn khi rolling update. Tính năng nào của ECS giúp đảm bảo container đủ trước khi stop?

A. Deployment circuit breaker  
B. Service discovery  
C. Task placement strategy  
D. Capacity Providers

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Deployment circuit breaker phát hiện triển khai thất bại, dừng và rollback, đảm bảo dịch vụ không gián đoạn lâu.
</details>

---

### Question 57
Lambda VPC access đột ngột chậm vì số lượng concurrent tăng cao. Nguyên nhân tiềm năng?

A. Thiếu route table  
B. Không đủ Elastic Network Interface (ENI) trong subnet  
C. Không gắn IAM role  
D. Không cấu hình environment variables

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Lambda tạo ENI trong subnet để truy cập VPC, concurrency cao có thể dẫn đến hết địa chỉ IP/ENI, gây throttling.
</details>

---

### Question 58
Bạn cần môi trường phát triển tự động dọn dẹp sau giờ làm để tiết kiệm chi phí EC2. Công cụ nào phù hợp?

A. AWS Budget  
B. Instance Scheduler (Solution) hoặc EventBridge + Systems Manager Automation  
C. AWS Config  
D. Trusted Advisor

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Instance Scheduler hoặc kết hợp EventBridge và SSM Automation giúp start/stop instance theo lịch.
</details>

---

### Question 59
Ứng dụng container cần scaling dựa trên độ trễ request. Với ECS Fargate, nên dùng gì?

A. Application Auto Scaling với custom CloudWatch metric  
B. Lambda scheduled  
C. Manual scaling  
D. AWS Batch

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Application Auto Scaling hỗ trợ ECS services, có thể dùng custom metric latency để scale in/out.
</details>

---

### Question 60
Bạn có workload phân tích dữ liệu, thỉnh thoảng cần hàng trăm vCPU trong vài giờ. Giải pháp chi phí hiệu quả?

A. On-Demand EC2  
B. Spot Fleet với diversified allocation + Auto Scaling  
C. Lambda  
D. Lightsail

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Spot Fleet đa dạng hóa loại instance cung cấp compute lớn với chi phí thấp cho workload tạm thời.
</details>

---

### Question 61
Ứng dụng HPC cần chia sẻ dữ liệu với throughput cao giữa các node. Lựa chọn storage nào đi kèm compute?

A. Amazon S3  
B. Amazon EFS với performance mode phù hợp  
C. Amazon Glacier  
D. AWS Backup

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** EFS cung cấp file system dùng chung, throughput cao, phù hợp HPC khi kết hợp với EC2/EKS.
</details>

---

### Question 62
Lambda đọc file lớn từ EFS khiến hiệu năng giảm. Tối ưu nào khả thi?

A. Tăng timeout Lambda lên tối đa  
B. Dùng Provisioned Concurrency và phân chia file thành phần nhỏ (parallel processing)  
C. Chuyển sang Lightsail  
D. Dùng EBS

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Provisioned Concurrency giảm cold start, chia nhỏ file để xử lý song song giảm thời gian đọc/ghi trên EFS.
</details>

---

### Question 63
Sự khác nhau giữa Lambda và Fargate về mô hình pricing?

A. Cả hai tính theo thời gian chạy và tài nguyên đã đặt trước  
B. Lambda tính theo số lần invoke + thời gian thực thi; Fargate tính theo vCPU/GB-giờ đã cấp phát  
C. Lambda chỉ tính theo số lần invoke  
D. Fargate miễn phí

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Lambda tính phí dựa trên số request và thời gian thực thi theo GB-second, Fargate tính theo tài nguyên đã cấu hình và thời gian chạy task.
</details>

---

### Question 64
Bạn cần migrate 500 VM on-premises lên AWS, muốn tự động hóa toàn bộ. Dịch vụ nào hỗ trợ giai đoạn compute?

A. AWS Migration Hub phù hợp  
B. AWS Server Migration Service (SMS) / AWS Application Migration Service (MGN)  
C. CloudFormation  
D. AWS Batch

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** AWS Application Migration Service (trước là CloudEndure) tự động hóa rehost VM lên EC2.
</details>

---

### Question 65
Workload container yêu cầu tự động scale xuống 0 khi không có traffic. Lựa chọn nào?

A. ECS Fargate với Application Auto Scaling  
B. ECS Fargate + AWS App Runner hoặc Knative trên EKS  
C. EC2 Auto Scaling  
D. Step Functions

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** App Runner/EKS Knative hỗ trợ scale-to-zero cho container, Fargate native scaling không xuống 0 (yêu cầu dịch vụ vẫn duy trì tối thiểu).
</details>

---

### Question 66
Ứng dụng phân tán cần triển khai đa Region, latency thấp, control traffic theo health checks. Giải pháp?

A. Route 53 latency-based routing + Health checks + Multi-Region EC2  
B. CloudWatch Logs  
C. AWS Backup  
D. DynamoDB

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Route 53 latency-based routing + health checks điều phối lưu lượng đến region tốt nhất, failover khi cần.
</details>

---

### Question 67
Bạn muốn track chi phí cho từng X86 vs ARM instances. Làm sao?

A. Dùng Cost Allocation Tags áp dụng trên Launch Template hoặc Auto Scaling  
B. Dùng CloudWatch Alarm  
C. Dùng IAM Policy  
D. Dùng Systems Manager

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Tag theo kiến trúc, bật cost allocation tags để theo dõi chi phí riêng biệt trong Cost Explorer.
</details>

---

### Question 68
Bạn chạy workload container EKS và muốn tối ưu Spot + On-Demand linh hoạt. Nên dùng?

A. EKS Managed Node Groups + Spot Instance  
B. Karpenter hoặc Cluster Autoscaler với node group đa dạng (Spot + On-Demand)  
C. Lambda  
D. CloudTrail

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Karpenter/Cluster Autoscaler cho phép mix Spot và On-Demand, tối ưu chi phí và độ tin cậy.
</details>

---

### Question 69
Thiết kế API serverless cần auth, caching, compute. Kết hợp nào hợp lý?

A. API Gateway + Lambda + Lambda@Edge  
B. API Gateway + Lambda + Amazon CloudFront + DynamoDB  
C. CloudFront + Lightsail  
D. SQS + SNS

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** API Gateway cung cấp auth, Lambda xử lý logic, CloudFront cache, DynamoDB lưu trữ serverless.
</details>

---

### Question 70
Lambda cần truy cập secrets để gọi RDS. Công cụ nào nên dùng?

A. Hard-code trong code  
B. AWS Secrets Manager hoặc Systems Manager Parameter Store  
C. Environment variables không mã hóa  
D. S3 public bucket

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Secrets Manager/Parameter Store cung cấp bảo mật, rotation, tích hợp với Lambda qua IAM.
</details>

---

### Question 71
Bạn muốn chạy workload GPU không liên tục, giảm chi phí nhưng hạn chế gián đoạn. Chiến lược?

A. Chỉ Spot Instances  
B. Spot Instances với Capacity-Optimized + On-Demand fallback  
C. 100% On-Demand  
D. Lambda

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Dùng Spot với chiến lược capacity-optimized giảm gián đoạn, fallback On-Demand đảm bảo workload tiếp tục.
</details>

---

### Question 72
Service container cần secrets rotation tự động. Giải pháp?

A. Lưu secrets trong EFS  
B. Dùng AWS Secrets Manager + task IAM role  
C. Lưu vào environment variable plain text  
D. Dùng CloudWatch Logs

<details>
<summary><strong>Answer: B</strong></summary>

**Giải thích:** Secrets Manager hỗ trợ rotation, ECS task role truy cập secrets an toàn qua ARNs.
</details>

---

### Question 73
Bạn có workload streaming cần xử lý real-time, latency thấp, scale automatically. Kết hợp compute nào?

A. Amazon Kinesis Data Streams + AWS Lambda + DynamoDB  
B. SQS + Lightsail  
C. Step Functions + EC2  
D. Batch + Athena

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Kinesis ingest data real-time, Lambda xử lý event-driven, DynamoDB lưu trữ nhanh.
</details>

---

### Question 74
Tổ chức muốn enforce policy chỉ dùng instance type được phê duyệt. Dịch vụ nào hỗ trợ?

A. AWS Organizations Service Control Policies (SCP)  
B. CloudWatch  
C. Route 53  
D. EventBridge

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** SCP cho phép giới hạn hành động IAM, có thể cấm tạo instance type không được phép.
</details>

---

### Question 75
Bạn cần serverless backend trả lời dưới 10ms, workload nhỏ và biến động. Giải pháp?

A. Lambda với SnapStart (Java) hoặc runtime nhẹ + Provisioned Concurrency  
B. EC2 Auto Scaling  
C. Lightsail  
D. Batch

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Provisioned Concurrency/SnapStart giảm cold start, đáp ứng latency rất thấp cho serverless.
</details>

---

### Question 76
Chương trình HPC cần xác định placement chính xác của instance. Công cụ?

A. AWS CLI `describe-instances` + `placement` metadata  
B. CloudWatch  
C. Config  
D. Trusted Advisor

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Sử dụng AWS CLI/API để lấy thông tin placement group, host ID, AZ cho HPC.
</details>

---

### Question 77
Bạn muốn zero-downtime deployment cho ứng dụng container với traffic lớn. Cách tiếp cận?

A. ECS + Application Load Balancer + CodeDeploy Blue/Green  
B. EC2 + user data  
C. Lambda versioning  
D. Lightsail

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** CodeDeploy Blue/Green kết hợp ALB chuyển traffic dần, đảm bảo zero-downtime cho ECS service.
</details>

---

### Question 78
Lambda serverless backend cần truy cập Aurora Serverless v2. Kết nối hiệu quả?

A. RDS Proxy để quản lý connection pooling  
B. Truy cập trực tiếp qua JDBC tạo nhiều connection  
C. API Gateway WebSocket  
D. Copy dữ liệu sang S3

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** RDS Proxy quản lý pool connection, giảm overhead, đặc biệt với Aurora Serverless v2 chịu tải bursty.
</details>

---

### Question 79
Ứng dụng container muốn tách biệt workload batch và service. Dùng ECS, nên cấu hình?

A. Hai services riêng với Capacity Provider khác nhau  
B. Một service duy nhất  
C. Lambda  
D. Batch

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** Tách thành hai ECS services, mỗi service gắn Capacity Provider riêng (ví dụ batch dùng Spot, service dùng On-Demand) để tối ưu.
</details>

---

### Question 80
Bạn cần triển khai inferencing ML global, latency thấp, mô hình container. Giải pháp?

A. SageMaker Endpoints multi-region  
B. ECS Anywhere  
C. Batch  
D. Lightsail

<details>
<summary><strong>Answer: A</strong></summary>

**Giải thích:** SageMaker endpoints hỗ trợ multi-region, auto-scaling, tối ưu inference cho container ML.
</details>

---

