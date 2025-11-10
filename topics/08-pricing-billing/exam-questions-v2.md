# Pricing & Billing - Exam Questions V2

> 🧠 Mục tiêu: Hiểu mô hình giá, tối ưu chi phí, dự toán và theo dõi chi phí trên AWS: On-Demand/RI/Savings Plans/Spot, Cost Explorer, Budgets, CUR, Compute Optimizer, Trusted Advisor, Consolidated Billing.  
> 📦 Nội dung: 50 câu nền tảng + 30 câu khó (tổng 80 câu) dạng multiple-choice/multiple-response

---

## Phần A - Câu hỏi nền tảng (50 câu)

### Question 1
On-Demand pricing đặc trưng?

A. Trả theo giây/giờ, không cam kết  
B. Cam kết 1-3 năm  
C. Rẻ nhất nhưng có thể bị thu hồi  
D. Trả trước toàn bộ

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** On-Demand linh hoạt nhất, không cam kết.
</details>

---

### Question 2
Reserved Instances/Savings Plans ưu điểm chính?

A. Không cam kết  
B. Giảm chi phí đáng kể khi cam kết sử dụng  
C. Tăng tính đàn hồi  
D. Miễn phí

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Cam kết thời gian/chi tiêu giúp giảm giá so với On-Demand.
</details>

---

### Question 3
Spot Instances?

A. Năng lực dư thừa, giảm giá lớn, có thể bị thu hồi với cảnh báo  
B. Luôn luôn đảm bảo  
C. Đắt nhất  
D. Chỉ cho Windows

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Phù hợp workload chịu gián đoạn (batch, stateless, flexible).
</details>

---

### Question 4
Compute Savings Plans áp dụng cho?

A. Chỉ EC2 một loại  
B. Linh hoạt EC2/Fargate/Lambda theo USD/giờ cam kết  
C. Chỉ Lambda  
D. Chỉ Fargate

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Compute SP linh hoạt nhất, vượt trội so với EC2 Instance SP về phạm vi.
</details>

---

### Question 5
Cost Explorer dùng để?

A. Phân tích chi phí, xu hướng, dự báo  
B. Mã hóa  
C. DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Cost Explorer là công cụ phân tích chi phí trực quan.
</details>

---

### Question 6
AWS Budgets cho phép?

A. Đặt ngân sách chi phí/usage/RI/SP và cảnh báo khi vượt ngưỡng  
B. Mã hóa  
C. CDN  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Budgets cảnh báo pro-active qua Email/SNS/Chatbot.
</details>

---

### Question 7
AWS Free Tier gồm?

A. 12-month Free, Always Free, Trials  
B. Chỉ 12 tháng  
C. Không có  
D. Trả trước

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Free Tier chia 3 nhóm theo tính năng/dịch vụ.
</details>

---

### Question 8
Consolidated Billing (Organizations) lợi ích?

A. Hóa đơn gộp, chia sẻ RI/SP discounts giữa accounts đủ điều kiện  
B. Không giảm chi phí  
C. Chỉ một hóa đơn, không chia sẻ  
D. Không hỗ trợ

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu chi phí toàn tổ chức nhờ pooling.
</details>

---

### Question 9
Cost Allocation Tags dùng để?

A. Gắn thẻ tài nguyên/chi phí theo dự án/đội/ứng dụng  
B. Mã hóa  
C. DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tagging là nền tảng cho chargeback/showback.
</details>

---

### Question 10
Cost and Usage Report (CUR) là?

A. Báo cáo chi tiết nhất về chi phí/usage xuất ra S3  
B. Báo cáo tổng quát  
C. Không có  
D. Chỉ EC2

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CUR là nguồn chuẩn cho phân tích chi tiết (Athena/Redshift/QuickSight).
</details>

---

### Question 11
Compute Optimizer giúp?

A. Đề xuất downsizing/rightsizing EC2/EBS/Lambda dựa trên metrics  
B. DNS  
C. Backup  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Công cụ tối ưu chi phí dựa số liệu thực tế.
</details>

---

### Question 12
TCO Calculator dùng để?

A. Ước tính tổng chi phí sở hữu khi chuyển lên AWS so với on-prem  
B. Backup  
C. DNS  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** TCO giúp business case cho migration.
</details>

---

### Question 13
Pricing Calculator?

A. Dự toán chi phí dịch vụ cụ thể theo cấu hình  
B. Không có  
C. Backup  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Lập dự toán chi tiết từng dịch vụ.
</details>

---

### Question 14
S3 chi phí gồm?

A. Lưu trữ, yêu cầu, data transfer out, tính năng (INT-tiering, replication)  
B. Chỉ lưu trữ  
C. Chỉ transfer  
D. Chỉ requests

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** S3 pricing gồm nhiều thành phần.
</details>

---

### Question 15
Data transfer nội vùng (same AZ) EC2->EC2?

A. Miễn phí nếu private IP cùng AZ/subnet (tùy trường hợp)  
B. Tính phí cao  
C. Luôn miễn phí mọi nơi  
D. Không có

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Transfer pricing phụ thuộc đường đi, AZ, public/private, cross-AZ/region.
</details>

---

### Question 16
Cross-AZ data transfer thường?

A. Có phí, cần cân nhắc kiến trúc (ALB, replication)  
B. Miễn phí  
C. Không tồn tại  
D. Chỉ S3 có phí

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Cross-AZ thường tính phí, tối ưu placement để giảm.
</details>

---

### Question 17
RI Convertible cho phép?

A. Đổi giữa instance family/OS/tenancy trong kỳ hạn  
B. Không đổi được  
C. Đổi region thoải mái không điều kiện  
D. Đổi sang Spot

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Convertible RI linh hoạt hơn Standard RI.
</details>

---

### Question 18
Savings Plans loại nào bị giới hạn loại instance?

A. Compute SP  
B. EC2 Instance SP (ràng buộc family/region/OS/tenancy)  
C. Không loại nào  
D. DynamoDB SP

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** EC2 Instance SP ràng buộc hơn Compute SP.
</details>

---

### Question 19
Trusted Advisor categories gồm?

A. Cost Optimization, Performance, Security, Fault Tolerance, Service Limits  
B. DNS  
C. Backup  
D. CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Năm nhóm khuyến nghị chính.
</details>

---

### Question 20
Consolidated Billing: ai trả tiền?

A. Management/Payer account nhận hóa đơn, member account không trả riêng  
B. Từng account trả riêng  
C. Không có  
D. S3 trả

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Payer account thanh toán cho cả tổ chức.
</details>

---

### Question 21
CUR tích hợp Athena?

A. Lưu CUR vào S3, dùng Athena/Glue để query chi phí bằng SQL  
B. Không thể  
C. Dùng DynamoDB  
D. Dùng NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Đây là cách phân tích chi tiết chi phí phổ biến.
</details>

---

### Question 22
Cost Anomaly Detection?

A. ML phát hiện chi phí bất thường theo service/link/account/tag  
B. DNS  
C. Backup  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Nhận cảnh báo sớm khi chi phí tăng bất thường.
</details>

---

### Question 23
Compute Optimizer yêu cầu?

A. Bật chia sẻ dữ liệu CloudWatch metrics  
B. Không cần metrics  
C. DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Dùng metrics để đưa khuyến nghị.
</details>

---

### Question 24
Rightsizing EC2 là gì?

A. Điều chỉnh loại/kích cỡ instance phù hợp sử dụng để tối ưu chi phí  
B. Tăng số lượng  
C. Giảm số lượng  
D. Đổi region

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Mục tiêu giảm lãng phí tài nguyên.
</details>

---

### Question 25
Chargeback/Showback?

A. Phân bổ chi phí theo team/dự án để minh bạch/thu hồi chi phí nội bộ  
B. Backup  
C. DNS  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Thực hiện dựa trên tagging và CUR.
</details>

---

### Question 26
S3 Intelligent-Tiering có phí quản lý nhỏ. Khi nào hợp lý?

A. Khi pattern truy cập khó dự báo, nhiều object  
B. Khi luôn nóng  
C. Khi luôn archive  
D. Không bao giờ

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Phí giám sát bù lại tiết kiệm do chuyển tier tự động.
</details>

---

### Question 27
Data transfer out to Internet là chi phí?

A. Thường lớn, cần tối ưu qua CloudFront/edge caching/architecting  
B. Không đáng kể  
C. Không tính phí  
D. Chỉ S3 tính

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu egress bằng CDN, nén, cache.
</details>

---

### Question 28
Compute cost giảm bằng?

A. Kết hợp RI/SP cho baseline + Spot cho burst + Auto Scaling + Compute Optimizer  
B. Chỉ On-Demand  
C. Chỉ Spot  
D. Chỉ RI

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Chiến lược lai giúp tối ưu chi phí/độ tin cậy.
</details>

---

### Question 29
EBS gp3 so với gp2?

A. Chi phí thấp hơn, cấu hình IOPS/Throughput độc lập với dung lượng  
B. Đắt hơn  
C. Không khác  
D. Không hỗ trợ

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** gp3 linh hoạt và chi phí tốt hơn.
</details>

---

### Question 30
ElastiCache pricing?

A. Tính theo node type/giờ + data transfer + backup (Redis)  
B. Miễn phí  
C. Chỉ data transfer  
D. Chỉ backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** ElastiCache tính theo node/time, backup Redis tính phí bổ sung.
</details>

---

### Question 31
Aurora vs RDS chi phí?

A. Aurora tính theo ACU (Serverless v2) hoặc instance + IO, storage, backup; RDS theo instance + storage + IO tùy engine  
B. Aurora luôn rẻ  
C. RDS luôn rẻ  
D. Không khác

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Cấu phần giá khác nhau cần so sánh theo workload.
</details>

---

### Question 32
Lambda pricing?

A. Theo số request và GB-seconds, plus provisioned concurrency nếu bật  
B. Theo giờ  
C. Miễn phí  
D. Theo storage

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu bằng giảm thời gian/ram, bundling, tránh cold start.
</details>

---

### Question 33
Athena pricing?

A. Theo dữ liệu quét (per TB), tối ưu bằng partition + compression + columnar  
B. Miễn phí  
C. Theo giờ  
D. Theo requests

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu schema S3 để giảm dữ liệu scan.
</details>

---

### Question 34
Redshift Serverless pricing?

A. Theo RPU giờ chạy query  
B. Theo node  
C. Miễn phí  
D. Theo storage

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Trả theo compute sử dụng.
</details>

---

### Question 35
CloudFront pricing?

A. Theo data transfer out, requests, price class, tính năng add-on (Function/Lambda@Edge)  
B. Miễn phí  
C. Chỉ requests  
D. Chỉ transfer

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Có free data transfer từ S3->CloudFront (origin fetch trong cùng region).
</details>

---

### Question 36
Consolidated Billing và sharing discount: hạn chế?

A. Cần cùng payer, RI/SP sharing phải bật, có quy tắc ưu tiên áp dụng  
B. Luôn chia sẻ  
C. Không chia sẻ  
D. Chỉ Spot

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Governance phải kiểm soát sharing để công bằng.
</details>

---

### Question 37
Budgets vs Cost Anomaly Detection?

A. Budgets theo ngưỡng cố định/dự báo; Anomaly phát hiện bất thường bằng ML  
B. Giống nhau  
C. Đều ML  
D. Không liên quan chi phí

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Hai công cụ bổ sung nhau.
</details>

---

### Question 38
EC2 Spot Advisor?

A. Gợi ý pools Spot có lịch sử gián đoạn thấp  
B. Không có  
C. DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Chọn pool phù hợp giảm gián đoạn.
</details>

---

### Question 39
Block Public Access ảnh hưởng chi phí?

A. Gián tiếp: giảm rủi ro data leakage dẫn tới chi phí vi phạm; không ảnh hưởng phí dịch vụ  
B. Giảm giá lưu trữ  
C. Tăng phí  
D. Không liên quan

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Control bảo mật không thay đổi cấu phần giá.
</details>

---

### Question 40
Right-tier S3?

A. Chọn storage class phù hợp pattern truy cập và yêu cầu truy xuất  
B. Luôn Standard  
C. Luôn IA  
D. Luôn Glacier

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tiering đúng giúp tiết kiệm đáng kể.
</details>

---

### Question 41
EC2 hạ chi phí network egress?

A. Dùng CloudFront, PrivateLink, interface/gateway endpoint, co-location region  
B. Dùng NAT nhiều  
C. Luôn public  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu egress và private connectivity giảm chi phí.
</details>

---

### Question 42
CUR partition S3 để query rẻ?

A. Partition theo `year=`, `month=`, `day=` và dùng Athena  
B. Không cần  
C. Luôn full scan  
D. Dùng NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Partition giảm dung lượng scan -> giảm chi phí.
</details>

---

### Question 43
Tagging strategy tốt gồm?

A. Chuẩn hóa key/values, bắt buộc khi provision, kiểm tra bằng Tag Policies/SCP  
B. Tùy hứng  
C. Không cần  
D. Chỉ vài dịch vụ

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tagging là nền tảng quản trị chi phí/quyền.
</details>

---

### Question 44
Khi nào dùng Savings Plans thay RI?

A. Khi cần linh hoạt giữa nhiều dịch vụ compute và thay đổi loại instance  
B. Khi cố định instance chỉ 1 loại  
C. Khi không muốn cam kết  
D. Khi chỉ dùng Lambda

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** SP linh hoạt hơn cho môi trường biến động.
</details>

---

### Question 45
RI Marketplace?

A. Nơi mua/bán lại RI Standard giữa khách hàng  
B. DNS  
C. Backup  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Giúp tối ưu khi nhu cầu thay đổi.
</details>

---

### Question 46
Reduce cost Lambda?

A. Giảm thời gian/ram phù hợp, tái sử dụng connection, provisioned concurrency có kiểm soát  
B. Luôn tăng RAM  
C. Không logging  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu thực thi giúp giảm GB-seconds.
</details>

---

### Question 47
Kinesis Data Firehose pricing?

A. Theo GB ingest và transformation/compression/encryption options  
B. Miễn phí  
C. Theo giờ  
D. Theo requests

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tính phí theo dữ liệu qua pipeline.
</details>

---

### Question 48
QuickSight editions?

A. Standard, Enterprise; pricing theo user/session (SPICE tính riêng)  
B. Miễn phí  
C. Chỉ theo giờ  
D. Theo node

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** SPICE lưu trữ in-memory tính phí riêng.
</details>

---

### Question 49
Cost-aware architecture?

A. Thiết kế tính đến pattern truy cập, scale-to-zero, dùng dịch vụ managed/serverless, đo lường liên tục  
B. Không quan tâm  
C. Luôn over-provision  
D. Không đo lường

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Pillar Cost Optimization trong Well-Architected.
</details>

---

### Question 50
Công cụ cộng đồng phổ biến để phân tích CUR?

A. Athena + QuickSight, open-source dashboards, Cloud Intelligence Dashboards  
B. Không có  
C. DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CID là tập dashboard mẫu miễn phí do AWS/community cung cấp.
</details>

---

## Phần B - Câu hỏi khó (30 câu)

### Question 51
Bạn có baseline workload 24/7 và phần burst không dự báo. Chiến lược tối ưu?

A. EC2 RI/SP cho baseline + Spot/On-Demand cho burst + Auto Scaling  
B. 100% On-Demand  
C. 100% Spot  
D. 100% RI

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kết hợp phù hợp tính ổn định/chi phí.
</details>

---

### Question 52
Chi phí tăng đột biến do NAT Gateway. Hướng xử lý?

A. Dùng VPC endpoints (Gateway/Interface), PrivateLink, NAT instance khi phù hợp, egress VPC  
B. Tăng thêm NAT Gateway  
C. Không thể  
D. Đổi region

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Giảm traffic qua NAT bằng private connectivity.
</details>

---

### Question 53
Bạn muốn dự báo chi phí 3-6 tháng theo xu hướng. Công cụ?

A. Cost Explorer forecasting + Budgets  
B. CloudTrail  
C. WAF  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CE có tính năng forecast dựa trên lịch sử.
</details>

---

### Question 54
Tối ưu chi phí Athena query?

A. Dùng định dạng cột (Parquet/ORC), nén, partition, projection, filter pushdown  
B. CSV không nén  
C. Không partition  
D. Quét full bucket

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Giảm bytes scanned -> giảm chi phí.
</details>

---

### Question 55
Tối ưu chi phí S3 replication?

A. Replicate có chọn lọc theo prefix/tag, bật RTC khi cần SLA, đánh giá storage class ở bucket đích  
B. Replicate tất cả  
C. Không replicate  
D. Luôn RTC

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Lựa chọn phù hợp nhu cầu, tránh chi phí không cần thiết.
</details>

---

### Question 56
Bạn muốn áp chính sách chi phí đa tài khoản theo OU. Làm sao?

A. Organizations + SCP giới hạn dịch vụ/region; Budget Actions; Compute Optimizer org-level  
B. Không thể  
C. WAF  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kết hợp governance và công cụ chi phí ở cấp tổ chức.
</details>

---

### Question 57
Chi phí EBS cao do snapshots. Giải pháp?

A. Lifecycle policy xóa snapshot cũ, archive snapshot, đánh giá mức độ redundancy  
B. Giữ hết  
C. Không snapshot  
D. Sao chép thêm

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Lifecycle + archive tiết kiệm đáng kể.
</details>

---

### Question 58
Bạn có data transfer giữa regions lớn. Giải pháp?

A. Thiết kế multi-region hợp lý, dùng CloudFront, giảm cross-region replication không cần thiết  
B. Không thể  
C. Tăng NAT  
D. Dùng DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Giảm egress giữa vùng bằng kiến trúc phù hợp.
</details>

---

### Question 59
EC2 instance oversize nhiều. Hành động?

A. Compute Optimizer/Trusted Advisor -> rightsizing -> ASG policy mới -> theo dõi  
B. Bỏ qua  
C. Tăng kích cỡ  
D. Chuyển hết sang Spot

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Quy trình chuẩn rightsizing liên tục.
</details>

---

### Question 60
Bạn muốn chargeback chi phí S3 theo bucket owner (multi-account). Làm sao?

A. Sử dụng CUR + cost allocation tag `owner` ở bucket và object, phân tích bằng Athena/QuickSight  
B. Không thể  
C. WAF  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tagging + CUR là nền tảng chargeback.
</details>

---

### Question 61
Chính sách giảm chi phí Lambda@Edge?

A. Logic ngắn gọn, tránh payload lớn, dùng CloudFront Functions khi đủ, test region gần edge  
B. Dùng luôn Lambda chuẩn  
C. Không caching  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CloudFront Functions rẻ/nhanh cho use case đơn giản.
</details>

---

### Question 62
Nâng cao minh bạch chi phí cho team dev?

A. Tạo dashboard QuickSight/Cost Explorer theo tag/team, gửi Budgets alert tới Slack qua Chatbot  
B. Không cần  
C. Chỉ email  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Minh bạch chi phí thúc đẩy tối ưu từ đầu.
</details>

---

### Question 63
Glue/Spark chi phí tăng vì shuffle lớn. Giải pháp?

A. Tối ưu partitioning, predicate pushdown, broadcast join khi phù hợp, spot cho workers  
B. Tăng executor vô hạn  
C. Không tối ưu  
D. Dùng NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu job giảm runtime/chi phí.
</details>

---

### Question 64
Aurora Serverless v2 chi phí tăng?

A. Giới hạn ACU, connection pooling, tách workload analytic sang Redshift (zero-ETL)  
B. Mặc kệ  
C. Tăng ACU  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kiểm soát scale và workload tách rời.
</details>

---

### Question 65
Budgets Actions có thể?

A. Thay đổi trạng thái tài nguyên (ví dụ dừng EC2) khi vượt ngưỡng  
B. Chỉ gửi email  
C. Không hành động  
D. Chỉ chat

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Budgets có thể trigger hành động tự động (cần thận trọng).
</details>

---

### Question 66
Khi nào nên chọn RI Standard thay Convertible?

A. Khi workload ổn định, ít thay đổi, muốn discount cao hơn  
B. Khi thường xuyên thay đổi loại instance  
C. Khi không muốn cam kết  
D. Khi chỉ dùng Lambda

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Standard RI discount cao nhất nhưng kém linh hoạt.
</details>

---

### Question 67
Chi phí cross-account KMS?

A. Có thể phát sinh phí request KMS và data key, quản lý key policy và sharing hợp lý  
B. Miễn phí  
C. Không thể  
D. Chỉ S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** KMS có pricing theo request/quản lý key.
</details>

---

### Question 68
Compute savings cho container?

A. ECS/EKS + Fargate SP/Compute SP, EC2 RI/SP cho node groups, Spot cho workloads linh hoạt  
B. Chỉ On-Demand  
C. Chỉ RI  
D. Chỉ Spot

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kết hợp công cụ tiết kiệm tương ứng layer compute.
</details>

---

### Question 69
Giảm chi phí dữ liệu phân tích lâu dài?

A. Lưu thô trên S3 (data lake), query bằng Athena/Redshift Spectrum thay vì cluster lớn luôn-on  
B. Luôn Redshift on  
C. Luôn EMR on  
D. Dùng NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Lake-first approach tiết kiệm đáng kể.
</details>

---

### Question 70
Giảm chi phí API Gateway?

A. Dùng HTTP API khi phù hợp (rẻ hơn REST API), CloudFront cache, payload nhỏ  
B. Luôn REST API  
C. Không cache  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** HTTP API rẻ/nhẹ cho use case đơn giản.
</details>

---

### Question 71
Phân tích CUR ở quy mô lớn, tự động dashboard?

A. Cloud Intelligence Dashboards (CID) triển khai bằng CloudFormation  
B. Làm tay  
C. Không có  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CID cung cấp dashboard mẫu cho FinOps.
</details>

---

### Question 72
Lifecycle FinOps theo chu kỳ?

A. Measure -> Optimize -> Operate -> Repeat (liên tục)  
B. Một lần  
C. Không cần  
D. Chỉ tối ưu

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** FinOps là hành trình liên tục.
</details>

---

### Question 73
Khi nào dùng BYOL?

A. Khi có license sẵn và cần tận dụng, có thể yêu cầu Dedicated Host/Placement  
B. Luôn luôn  
C. Không bao giờ  
D. Khi on-prem

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** BYOL cần tuân thủ license và hạ tầng phù hợp.
</details>

---

### Question 74
Tối ưu chi phí logs?

A. Sampling, retention hợp lý, chuyển lạnh sang S3, nén, filter trước khi ingest  
B. Log mọi thứ vô hạn  
C. Không log  
D. Không nén

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Cân bằng quan sát và chi phí.
</details>

---

### Question 75
Kiểm soát chi phí Data Transfer ra Internet ở multi-cloud/CDN?

A. Dùng CloudFront/peering, chọn region hợp lý, tối ưu cache/policies  
B. Không thể  
C. Chỉ NAT  
D. Dùng IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kiến trúc egress quan trọng trong chi phí.
</details>

---

### Question 76
Giảm chi phí RDS idle?

A. Stop/start schedule (khi engine hỗ trợ), serverless (Aurora v2), rightsizing, read replica chỉ khi cần  
B. Giữ nguyên  
C. Luôn max size  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu theo pattern sử dụng.
</details>

---

### Question 77
Tối ưu chi phí EKS control plane?

A. EKS control plane tính phí cố định; cân nhắc cluster multi-tenant hợp lý, node groups Spot/RI/SP  
B. Không thể  
C. Luôn 1 cluster mỗi team  
D. Không dùng EKS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Thiết kế tenancy hợp lý giảm chi phí.
</details>

---

### Question 78
Data transfer PrivateLink?

A. Traffic qua backbone AWS, tránh egress Internet; có phí endpoint/hours/data processing  
B. Miễn phí  
C. Chỉ EC2  
D. Không tính phí data

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** PrivateLink tăng bảo mật và có cấu phần chi phí riêng.
</details>

---

### Question 79
FinOps tổ chức nên gồm?

A. Dev, Fin, Ops hợp tác, mục tiêu chung tối ưu chi phí/giá trị  
B. Chỉ Finance  
C. Chỉ Ops  
D. Chỉ Dev

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** FinOps là nỗ lực liên chức năng.
</details>

---

### Question 80
Chiến lược tổng thể giảm chi phí bền vững?

A. Thiết kế cost-aware, đo lường liên tục, tự động hóa tối ưu, governance, nhịp FinOps định kỳ  
B. Làm 1 lần  
C. Cắt dịch vụ  
D. Không đo lường

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Cách tiếp cận hệ thống và liên tục.
</details>

---

