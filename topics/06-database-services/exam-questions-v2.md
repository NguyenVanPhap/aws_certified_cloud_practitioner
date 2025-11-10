# Database Services - Exam Questions V2

> 🧠 Mục tiêu: Ôn tập toàn diện dịch vụ Cơ sở dữ liệu trên AWS (RDS, Aurora, DynamoDB, Redshift, ElastiCache, DocumentDB, Neptune, Timestream, DMS, RDS Proxy, v.v.).  
> 📦 Nội dung: 50 câu nền tảng + 30 câu khó (tổng 80 câu) dạng multiple-choice/multiple-response.

---

## Phần A - Câu hỏi nền tảng (50 câu)

### Question 1
Dịch vụ nào là managed relational database đa engine (MySQL, PostgreSQL, MariaDB, Oracle, SQL Server)?

A. Amazon RDS  
B. Amazon DynamoDB  
C. Amazon Redshift  
D. Amazon Neptune

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Amazon RDS cung cấp DBaaS cho các engine quan hệ phổ biến với backup, patching, Multi-AZ, Read Replica.
</details>

---

### Question 2
Dịch vụ NoSQL key-value/Document có độ trễ mili-giây đơn và scale vô hạn là?

A. Amazon RDS  
B. Amazon DynamoDB  
C. Amazon Redshift  
D. Amazon Timestream

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** DynamoDB là dịch vụ NoSQL fully managed, hỗ trợ provisioned/on-demand, global tables, TTL, streams.
</details>

---

### Question 3
Redshift phù hợp nhất cho?

A. OLTP giao dịch  
B. Data warehousing và analytics quy mô lớn (OLAP)  
C. Caching in-memory  
D. Time-series IoT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Redshift là DW MPP columnar cho phân tích dữ liệu quy mô lớn, tích hợp Spectrum với S3.
</details>

---

### Question 4
ElastiCache gồm những engine nào?

A. Redis và Memcached  
B. Redis và MongoDB  
C. Memcached và Cassandra  
D. Redis và DynamoDB

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** ElastiCache hỗ trợ Redis (replication, persistence) và Memcached (sharding đơn giản).
</details>

---

### Question 5
Aurora là?

A. CSDL NoSQL  
B. CSDL quan hệ tương thích MySQL/PostgreSQL, hiệu năng cao do AWS xây dựng  
C. Dịch vụ caching  
D. Graph database

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Aurora tương thích MySQL/PG, lưu trữ tách compute, 6-way replication across 3 AZ, hiệu năng/HA cao.
</details>

---

### Question 6
Multi-AZ trong RDS cung cấp?

A. Tăng hiệu năng read  
B. HA/DR: đồng bộ sang standby ở AZ khác, failover tự động  
C. Ghi ra S3  
D. Giảm chi phí

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Multi-AZ cung cấp tính sẵn sàng cao, không nhằm mục đích scale đọc (dùng read replica để đọc).
</details>

---

### Question 7
Read Replica của RDS dùng để?

A. Failover tự động  
B. Scale đọc và phục vụ read-heavy workloads  
C. Sao lưu  
D. Mã hóa

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Read Replica là replication không đồng bộ, tăng khả năng đọc, có thể promote khi cần.
</details>

---

### Question 8
DynamoDB hỗ trợ hai chế độ capacity:

A. Fixed và Variable  
B. Provisioned và On-Demand  
C. Unlimited và Limited  
D. Batch và Stream

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Provisioned cho phép đặt RCUs/WCUs; On-Demand tự động scale theo nhu cầu, trả theo request.
</details>

---

### Question 9
Global Tables cho DynamoDB cho phép?

A. Replicate dữ liệu đa vùng với multi-active writes  
B. Chỉ replicate 1 chiều  
C. Sao lưu sang S3  
D. Chỉ ở một region

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Global Tables cung cấp multi-region, multi-master replication với latency thấp ở global.
</details>

---

### Question 10
DynamoDB DAX là gì?

A. Analytics service  
B. In-memory cache tương thích DynamoDB API, giảm latency micro-giây  
C. Backup tool  
D. Migration tool

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** DAX là cache in-memory cluster, drop-in replacement cho read-intensive, không thay đổi code nhiều.
</details>

---

### Question 11
RDS Proxy dùng để?

A. Caching query  
B. Connection pooling cho RDS/Aurora, tối ưu kết nối từ Lambda/app server  
C. Sao lưu snapshot  
D. Mã hóa dữ liệu

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** RDS Proxy quản lý pool connection, cải thiện scale và failover, bảo mật IAM authentication.
</details>

---

### Question 12
Aurora Serverless v2 cung cấp?

A. Scale thủ công  
B. Tự động scale capacity mượt mà (ACU), khởi động nhanh, phù hợp workload biến động  
C. Multi-master toàn cầu  
D. Không hỗ trợ Aurora

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Aurora Serverless v2 scale theo nhu cầu với granular ACU, ít gián đoạn.
</details>

---

### Question 13
Neptune là?

A. Graph database managed service  
B. Time-series  
C. Key-value  
D. Columnar DW

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Neptune là graph DB hỗ trợ Gremlin, SPARQL, RDF.
</details>

---

### Question 14
DocumentDB tương thích?

A. PostgreSQL  
B. MongoDB  
C. Oracle  
D. Cassandra

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Amazon DocumentDB (with MongoDB compatibility) tương thích API MongoDB, lưu trữ tách compute.
</details>

---

### Question 15
Timestream phù hợp?

A. Dữ liệu đồ thị  
B. Dữ liệu time-series IoT/ops metrics  
C. Dữ liệu relational OLTP  
D. Dữ liệu văn bản

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Timestream là time-series database managed, auto tiering hot/cold, query SQL-like.
</details>

---

### Question 16
AWS DMS dùng để?

A. Caching  
B. Di chuyển dữ liệu giữa DB engines khác nhau (heterogeneous/homogeneous) với downtime tối thiểu  
C. Sao lưu EBS  
D. ETL nâng cao

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Database Migration Service hỗ trợ CDC, replication liên tục, di chuyển ít downtime.
</details>

---

### Question 17
Backup tự động trong RDS tạo?

A. Snapshot hàng ngày và transaction logs để point-in-time recovery  
B. Chỉ snapshot thủ công  
C. Log vào CloudWatch  
D. Không có

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** RDS tự động backup theo retention, cho phép phục hồi tới thời điểm.
</details>

---

### Question 18
Aurora Global Database cung cấp?

A. Multi-region writes  
B. Primary region write, secondary region read với replication <1s  
C. Chỉ single region  
D. Không HA

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Aurora Global Database tối ưu DR và low-latency read global, replicate storage ở mức thấp.
</details>

---

### Question 19
DynamoDB Streams dùng để?

A. Gửi thông điệp đến SNS  
B. Lưu thay đổi item (insert/update/delete) để xử lý downstream (Lambda, Kinesis)  
C. Sao lưu  
D. Tăng TTL

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Streams ghi lại các thay đổi table theo thứ tự, tích hợp Lambda event-driven.
</details>

---

### Question 20
ElastiCache Redis Multi-AZ with Auto Failover cung cấp?

A. Scale ghi đa leader  
B. Replication primary-replica, failover tự động khi node primary hỏng  
C. Backup S3  
D. DAX

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** ElastiCache Redis hỗ trợ multi-AZ failover để tăng sẵn sàng.
</details>

---

### Question 21
Redshift Spectrum dùng để?

A. Query trực tiếp dữ liệu trên S3 dùng SQL từ Redshift  
B. Sao lưu Redshift  
C. Log query  
D. Machine learning

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Spectrum cho phép Redshift truy vấn data lake trên S3 mà không phải load vào cluster.
</details>

---

### Question 22
Redshift Serverless cung cấp?

A. Phải quản lý node  
B. Tính phí theo RPU (Redshift Processing Unit), không quản lý hạ tầng  
C. Miễn phí  
D. Không hỗ trợ Spectrum

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Redshift Serverless tự quản lý scaling/compute, tính phí theo thời gian sử dụng RPU.
</details>

---

### Question 23
DynamoDB primary key gồm?

A. Partition key và sort key (tùy chọn sort key)  
B. Chỉ sort key  
C. Chỉ hash key  
D. Composite key cố định

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** DynamoDB dùng partition key (bắt buộc) và có thể thêm sort key để tạo composite key.
</details>

---

### Question 24
Local Secondary Index (LSI) khác Global Secondary Index (GSI) ở đâu?

A. LSI có partition key khác, GSI cùng partition key  
B. LSI dùng cùng partition key, sort key khác; GSI cho phép partition key khác  
C. Chúng giống nhau  
D. LSI chỉ cho ghi

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** LSI chia sẻ partition key với bảng, thay sort key; GSI có partition/sort key khác, hỗ trợ truy vấn linh hoạt.
</details>

---

### Question 25
TTL trong DynamoDB dùng để?

A. Tự động xóa item khi quá hạn  
B. Mã hóa item  
C. Sao lưu  
D. Tăng throughput

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** TTL đánh dấu timestamp để hệ thống tự xóa item, giảm chi phí lưu trữ.
</details>

---

### Question 26
RDS Performance Insights giúp?

A. Sao lưu  
B. Phân tích hiệu năng DB (top SQL, waits)  
C. Quản lý IAM  
D. Tạo VPC

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Performance Insights giúp quan sát hiệu năng, xác định bottleneck và câu lệnh nặng.
</details>

---

### Question 27
Redshift distribution style nào giúp cân bằng dữ liệu tốt?

A. ALL  
B. EVEN  
C. KEY (theo cột)  
D. AUTO

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B hoặc D (AUTO để hệ thống chọn tối ưu), cơ bản: EVEN cân bằng khi không có key join nổi trội.  
**Giải thích:** EVEN phân phối round-robin; AUTO để Redshift quyết định tốt nhất. Với join cụ thể nên chọn KEY.
</details>

---

### Question 28
Aurora lưu trữ dữ liệu thế nào?

A. Trên instance EC2  
B. Trên storage cluster tách rời, 6 bản sao across 3 AZ  
C. Trên EBS đơn  
D. Trên S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Aurora storage phân tán, tự healing, tách compute và storage.
</details>

---

### Question 29
ElastiCache Memcached phù hợp khi?

A. Cần persistence snapshot  
B. Cần sharding đơn giản, cache ephemeral, scale out dễ  
C. Cần Pub/Sub và replication  
D. Cần stream

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Memcached đơn giản, scale-out sharding, không có persistence/replication như Redis.
</details>

---

### Question 30
RDS encryption at-rest dùng?

A. KMS keys  
B. S3 SSE-S3  
C. IAM  
D. CloudHSM bắt buộc

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** RDS sử dụng KMS keys để mã hóa at-rest, bao gồm snapshots và read replicas (nếu enable từ đầu).
</details>

---

### Question 31
Redshift Concurrency Scaling dùng để?

A. Thêm node tạm thời phục vụ truy vấn đồng thời cao  
B. Sao lưu  
C. Tăng dung lượng lưu trữ  
D. Kết nối VPN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Concurrency Scaling thêm resources tạm giảm thời gian chờ khi nhiều query đồng thời.
</details>

---

### Question 32
Aurora Read Replica cho phép?

A. Scale đọc với nhiều replicas, reader endpoint phân phối connection  
B. Scale ghi nhiều chủ  
C. Không hỗ trợ  
D. Chỉ 1 replica

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Aurora có thể có nhiều read replicas, reader endpoint tự cân bằng kết nối đọc.
</details>

---

### Question 33
DynamoDB transactional API cung cấp?

A. Không hỗ trợ transaction  
B. Hỗ trợ `TransactWriteItems` và `TransactGetItems` với ACID trong một tài khoản/khu vực  
C. Chỉ eventual consistency  
D. Chỉ 1 item

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** DynamoDB hỗ trợ giao dịch ACID cho nhóm thao tác (tối đa 25 item) trong một region/account.
</details>

---

### Question 34
RDS engines nào hỗ trợ IAM database authentication?

A. MySQL và PostgreSQL (bao gồm Aurora MySQL/PG)  
B. Oracle  
C. SQL Server  
D. MariaDB duy nhất

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** IAM database authentication hỗ trợ MySQL/PG/Aurora, giảm quản lý mật khẩu DB.
</details>

---

### Question 35
Redshift RA3 nodes lợi ích chính?

A. CPU mạnh hơn  
B. Managed Storage tách compute/lưu trữ, scale độc lập, data cache local SSD  
C. Không có lợi ích  
D. Chỉ dùng được Spectrum

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** RA3 tối ưu chi phí nhờ managed storage và cache, scale compute theo nhu cầu.
</details>

---

### Question 36
ElastiCache Redis cluster mode enabled (sharding) dùng để?

A. Tăng HA nhưng không scale  
B. Shard dữ liệu across nhiều node để scale out  
C. Chỉ 1 primary, không replica  
D. Không hỗ trợ persistence

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Cluster mode enabled cho phép nhiều shard, mỗi shard có primary/replica, scale out.
</details>

---

### Question 37
Aurora Backtrack (MySQL) dùng để?

A. Quay về trạng thái trước đó ở cấp phút/giờ mà không phục hồi từ snapshot  
B. Sao lưu S3  
C. Tăng performance  
D. Tạo replica

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Backtrack cho phép tua ngược trạng thái DB mà không cần restore snapshot, hữu ích test/sửa lỗi.
</details>

---

### Question 38
DocumentDB backup như thế nào?

A. Không hỗ trợ  
B. Tự động liên tục sang S3 với retention, point-in-time restore  
C. Chỉ thủ công  
D. Chỉ EBS snapshot

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** DocumentDB cung cấp automated backup tương tự RDS/Aurora.
</details>

---

### Question 39
Timestream lưu trữ dữ liệu theo tier?

A. Không có tier  
B. Memory store (hot) và magnetic store (cold) tự động lifecycle  
C. Chỉ magnetic  
D. Chỉ memory

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Dữ liệu mới lưu ở memory để query nhanh, sau đó chuyển sang magnetic tiết kiệm chi phí.
</details>

---

### Question 40
RDS Storage Auto Scaling giúp?

A. Tự tăng IOPS  
B. Tự tăng dung lượng lưu trữ khi gần đầy  
C. Tự thêm replica  
D. Tự bật Multi-AZ

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Storage Auto Scaling giúp tránh hết dung lượng, tăng dần theo ngưỡng cấu hình.
</details>

---

### Question 41
Khi nào nên dùng ElastiCache trước RDS?

A. Khi workload đọc lặp lại nhiều, cần giảm latency và offload DB  
B. Khi cần ghi nhiều  
C. Khi cần transaction  
D. Khi cần backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Cache giúp giảm tải DB, cải thiện latency cho nội dung đọc nhiều lần.
</details>

---

### Question 42
Redshift snapshot là?

A. Backup incremental lưu S3-managed  
B. Chỉ full copy  
C. Không hỗ trợ  
D. Lưu EBS local

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Redshift snapshot incremental lưu trên S3 do AWS quản lý.
</details>

---

### Question 43
Aurora Parallel Query là gì?

A. Tính năng caching  
B. Đẩy xử lý query xuống storage layer để parallel hóa, tăng tốc SELECT lớn  
C. Multi-master  
D. Dừng ghi

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Parallel Query giúp tăng tốc workload analytic trên Aurora MySQL compatible.
</details>

---

### Question 44
Khi dùng DynamoDB On-Demand, bạn được lợi gì?

A. Chi phí cố định  
B. Không cần dự báo capacity, auto scale theo request, trả theo dùng  
C. Không thể burst  
D. Chậm hơn provisioned

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** On-Demand phù hợp traffic khó dự báo, scale tự động.
</details>

---

### Question 45
ElastiCache Redis AOF/RDB là?

A. Cơ chế persistence của Redis (Append Only File / Snapshot)  
B. Công cụ migration  
C. Cơ chế cache invalidation  
D. Cơ chế encryption

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Redis có persistence AOF và RDB để khôi phục dữ liệu sau sự cố.
</details>

---

### Question 46
Redshift sort keys dùng cho?

A. Quy định thứ tự lưu cột để tối ưu query predicate  
B. Mã hóa  
C. Tăng HA  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Sort keys giúp tối ưu scan cho các cột thường filter/join.
</details>

---

### Question 47
Aurora MySQL vs RDS MySQL ưu điểm chính?

A. Aurora rẻ hơn luôn  
B. Aurora hiệu năng cao hơn, HA tốt hơn, storage tách rời, replication nhanh  
C. Không có khác biệt  
D. Aurora không có read replica

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Aurora tối ưu kiến trúc, throughput cao hơn RDS MySQL, thời gian failover nhanh.
</details>

---

### Question 48
DocumentDB scale read bằng?

A. Sharding  
B. Thêm read replicas  
C. Multi-master  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** DocumentDB thêm read replicas để scale đọc và HA.
</details>

---

### Question 49
DynamoDB hot partition xảy ra khi?

A. Partition key được phân bố tốt  
B. Quá nhiều truy cập dồn vào ít partition key, gây throttling  
C. Dùng on-demand  
D. Dùng TTL

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Phân phối key kém gây hotspot, cần thiết kế key phân tán.
</details>

---

### Question 50
Aurora Global Database dùng để DR như thế nào?

A. Không liên quan DR  
B. Cho phép promote region phụ thành primary khi thảm họa, RTO nhanh  
C. Chỉ đọc  
D. Chỉ 1 AZ

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Aurora Global Database cho phép failover region nhanh, giảm downtime lớn.
</details>

---

## Phần B - Câu hỏi khó (30 câu)

### Question 51
Bạn có ứng dụng serverless (Lambda) kết nối RDS PostgreSQL, bị lỗi connection exhaustion khi traffic spike. Giải pháp?

A. Tăng size DB instance  
B. Dùng RDS Proxy để pool connection và IAM auth  
C. Dùng NAT Gateway  
D. Dùng DAX

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** RDS Proxy quản lý connection pooling cho Lambda, cải thiện scalability và bảo mật.
</details>

---

### Question 52
Bạn muốn chuyển RDS MySQL sang Aurora MySQL với downtime tối thiểu. Cách?

A. Export/Import bằng mysqldump  
B. Dùng DMS với CDC, hoặc Aurora fast cloning snapshot nếu tương thích  
C. Stop ứng dụng và restore snapshot  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** DMS hỗ trợ replication liên tục (CDC) để switch với downtime thấp.
</details>

---

### Question 53
DynamoDB design: bạn cần query top-N theo thời gian cho từng user. Thiết kế khóa?

A. Partition key = userId, sort key = timestamp (DESC bằng invert/negative/ISO desc)  
B. Partition key = timestamp, sort key = userId  
C. Partition key = random  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** PK= userId nhóm bản ghi theo user; SK theo time để query range nhanh và top-N.
</details>

---

### Question 54
Redshift cần truy vấn join lớn giữa 2 bảng. Tối ưu?

A. Chọn distribution style KEY trên cột join chung để co-locate dữ liệu  
B. Dùng ALL cho mọi bảng  
C. Không có cách  
D. Dùng NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** KEY distribution đặt row có cùng key trên cùng node slice, giảm shuffle.
</details>

---

### Question 55
Aurora Serverless v2 thấy chi phí tăng đột biến do burst. Giải pháp?

A. Giới hạn ACU tối đa, bật autoscaling policy hợp lý, connection pooling từ ứng dụng  
B. Tắt serverless  
C. Dùng DAX  
D. Dùng NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Giới hạn ACU max/min, tuning pool kết nối, tránh bùng nổ connection gây scale không cần thiết.
</details>

---

### Question 56
DynamoDB Global Table gặp xung đột ghi đa vùng. Giải quyết?

A. Không thể giải quyết  
B. Dùng chiến lược conflict resolution (last-writer-wins dựa trên timestamp) ở ứng dụng hoặc attribute version  
C. Chỉ cho phép 1 vùng ghi  
D. Dùng DAX

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Global Tables cần chiến lược xử lý xung đột ở tầng ứng dụng khi multi-active.
</details>

---

### Question 57
RDS Multi-AZ vs Read Replica khác nhau?

A. Multi-AZ để scale đọc, Read Replica để HA  
B. Multi-AZ cho HA/DR đồng bộ; Read Replica cho scale đọc không đồng bộ  
C. Giống nhau  
D. Không dùng cho production

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Multi-AZ cung cấp failover; Read Replica dùng đọc và có thể promote thủ công.
</details>

---

### Question 58
Bạn cần audit mọi thay đổi schema trong RDS PostgreSQL. Công cụ?

A. CloudWatch Logs  
B. Database logs + pgAudit extension (nếu hỗ trợ) và/hoặc DMS CDC stream sang S3/Lake  
C. DAX  
D. CloudFront

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** pgAudit hoặc logical decoding + DMS để lưu thay đổi, tùy nhu cầu audit và compliance.
</details>

---

### Question 59
Redshift cần tách workload ETL và BI để không ảnh hưởng nhau. Giải pháp?

A. WLM (Workload Management) queue, hoặc 2 namespace (serverless)  
B. Tăng node  
C. Dùng NAT  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** WLM phân tách queue theo user/group/query group; serverless có namespace isolate.
</details>

---

### Question 60
ElastiCache Redis cần read scaling lớn và HA. Kiến trúc?

A. 1 primary, nhiều replicas, Multi-AZ, read endpoint, cluster mode enabled nếu dữ liệu lớn  
B. Single node  
C. Memcached  
D. Không replica

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Replica để scale đọc, Multi-AZ failover, cluster mode để sharding dữ liệu.
</details>

---

### Question 61
Aurora Global Database muốn giảm RPO gần 0. Lưu ý?

A. Không thể  
B. Dùng Replica Lag thấp do replication ở storage layer (<1s), nhưng RPO=0 không đảm bảo; cần chiến lược ứng dụng  
C. Dùng DAX  
D. Dùng Timestream

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Replication nhanh nhưng không đảm bảo RPO=0 cho thảm họa lớn; cân nhắc 2 vùng ghi (Aurora Multi-Master—giới hạn) hoặc thiết kế ứng dụng.
</details>

---

### Question 62
DynamoDB Streams + Lambda -> Kinesis Firehose -> S3 dùng để?

A. ETL real-time change data capture vào data lake  
B. Sao lưu  
C. Tăng TTL  
D. Caching

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CDC pipeline phổ biến để phân tích dữ liệu thay đổi theo thời gian.
</details>

---

### Question 63
Bạn cần khóa ứng dụng đọc nhiều, ghi ít với latency micro-giây. Chọn?

A. DynamoDB + DAX  
B. RDS MySQL  
C. Redshift  
D. Neptune

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** DAX cung cấp cache micro-giây cho read-heavy pattern.
</details>

---

### Question 64
Redshift muốn giảm chi phí khi query thưa. Chọn?

A. Redshift Serverless, pause/resume cluster truyền thống, hoặc concurrency scaling credits  
B. Tăng node  
C. Dùng DAX  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Serverless trả theo dùng; cluster có thể pause để tiết kiệm khi idle.
</details>

---

### Question 65
RDS Oracle/SQL Server có license. Cách tối ưu chi phí?

A. BYOL trên Dedicated Host khi yêu cầu compliance, hoặc dùng License Included nếu phù hợp  
B. Dùng Redshift  
C. Dùng Neptune  
D. Không có cách

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tùy license, có thể BYOL trên Dedicated Host hoặc sử dụng License Included.
</details>

---

### Question 66
DocumentDB cần multi-region read và DR. Giải pháp?

A. Global Clusters (DocumentDB Global) để replicate cross-region, promote khi DR  
B. Không hỗ trợ  
C. DynamoDB Global Table  
D. Redshift

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** DocumentDB Global Clusters cho phép replicate dữ liệu giữa regions để DR/low-latency read.
</details>

---

### Question 67
DynamoDB design: chống hot key cho top seller productId?

A. Sử dụng random suffix/prefix (write sharding) và GSI để aggregate  
B. Không cần  
C. Dùng TTL  
D. Dùng DAX

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Write sharding phân tán ghi, GSI phục vụ query tổng hợp.
</details>

---

### Question 68
Aurora muốn tách workload transactional và analytic. Làm sao?

A. Dùng Aurora read replicas chuyên cho analytic, hoặc Aurora zero-ETL integration với Redshift  
B. Không thể  
C. Dùng DAX  
D. Dùng NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Replica/zero-ETL giảm ảnh hưởng OLTP, đẩy analytic sang engine phù hợp.
</details>

---

### Question 69
Redshift muốn query trực tiếp Iceberg/Hudi/Delta trên S3. Cách?

A. Redshift Spectrum với Lake Formation và hỗ trợ table format mở  
B. Không thể  
C. Dùng DynamoDB  
D. Dùng RDS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Redshift Spectrum hỗ trợ data lake table formats thông qua Glue/Lake Formation catalog.
</details>

---

### Question 70
ElastiCache Redis cần bảo mật mạnh. Gợi ý?

A. Transit encryption (in-transit), at-rest encryption, AUTH, VPC only, SG/NACL chặt chẽ  
B. Public access  
C. Không cần encryption  
D. S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Redis hỗ trợ TLS, encryption at-rest, AUTH token, giới hạn mạng trong VPC.
</details>

---

### Question 71
DMS migration từ Oracle sang Aurora PostgreSQL. Thách thức?

A. Heterogeneous migration cần chuyển đổi schema (AWS SCT) trước khi DMS replicate  
B. Không thể  
C. Dùng DAX  
D. Dùng NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** AWS Schema Conversion Tool chuyển đổi schema/PLSQL -> PG trước khi dùng DMS CDC.
</details>

---

### Question 72
DynamoDB muốn audit mỗi thay đổi item chi tiết. Cách?

A. Bật Streams (NEW_AND_OLD_IMAGES) và đẩy sang S3/Firehose để lưu lâu dài  
B. Không thể  
C. TTL  
D. Cache

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Streams có thể bao gồm ảnh trước/sau để audit chi tiết.
</details>

---

### Question 73
Aurora muốn giảm cold start connection từ Lambda. Gợi ý?

A. Sử dụng RDS Proxy, giữ pool luôn ấm, cấu hình min connections  
B. Tắt Multi-AZ  
C. Dùng NAT  
D. Dùng DAX

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Proxy giữ kết nối sẵn, giảm overhead tạo kết nối mới.
</details>

---

### Question 74
Redshift cross-region snapshot copy dùng cho?

A. DR và compliance multi-region  
B. Tăng performance  
C. DAX  
D. TTL

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Snapshot copy cross-region hỗ trợ phục hồi khi region sự cố.
</details>

---

### Question 75
Neptune cần đảm bảo độ tin cậy cao và throughput đọc. Cách?

A. Thêm Neptune replicas, Multi-AZ, bật AutoFailover  
B. Single node  
C. DAX  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Replicas tăng read throughput và HA; failover tự động.
</details>

---

### Question 76
Timestream ingest cao, query chủ yếu thời gian gần. Tối ưu?

A. Tăng retention ở memory store cho khoảng thời gian quan trọng, optimize measures/dimensions  
B. Đưa hết sang magnetic  
C. Dùng DynamoDB  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Memory store phù hợp query gần; magnetic cho dữ liệu cũ, tối ưu hóa schema hợp lý.
</details>

---

### Question 77
Aurora muốn cô lập workload report nặng. Làm sao?

A. Tạo dedicated read replica và trỏ báo cáo vào replica đó  
B. Chạy trên primary  
C. Dùng DAX  
D. Dùng NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Replica cô lập ảnh hưởng report khỏi OLTP.
</details>

---

### Question 78
DynamoDB cần query linh hoạt field không nằm trong PK/SK. Cách?

A. Tạo GSI phù hợp cho pattern query  
B. Không thể  
C. Dùng TTL  
D. DAX

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** GSI cho phép query theo partition/sort key khác.
</details>

---

### Question 79
Redshift cần bảo vệ truy cập theo cột/hàng. Công cụ?

A. Role-based access control, column-level security, row-level security, Lake Formation với Spectrum  
B. IAM only  
C. Không hỗ trợ  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Redshift hỗ trợ column/row-level security; Lake Formation quản trị quyền trên S3 tables.
</details>

---

### Question 80
Bạn cần kiến trúc data platform: ingest -> lake -> DW -> BI, chi phí tối ưu. Phối hợp?

A. Kinesis/MSK -> S3 (data lake, Lake Formation) -> Redshift (serverless) -> QuickSight; metadata Glue  
B. DynamoDB -> DAX -> NAT -> CloudFront  
C. EC2 -> EBS -> S3  
D. Aurora -> S3 website

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Đây là kiến trúc chuẩn data platform trên AWS với dịch vụ managed và tối ưu chi phí/scale.
</details>

---

