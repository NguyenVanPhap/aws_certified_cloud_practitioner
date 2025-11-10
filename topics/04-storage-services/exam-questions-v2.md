# Storage Services - Exam Questions V2

> 🧠 Mục tiêu: Ôn tập tổng lực Storage services cho kỳ thi AWS Certified Cloud Practitioner  
> 📦 Nội dung: 50 câu nền tảng + 30 câu khó (tổng 80 câu) dạng multiple-choice/multiple-response

---

## Phần A - Câu hỏi nền tảng (50 câu)

### Question 1
Dịch vụ nào là object storage bền vững cao trên AWS?

A. Amazon EBS  
B. Amazon S3  
C. Amazon EFS  
D. AWS Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Amazon S3 là dịch vụ object storage với độ bền 11 số 9, lưu trữ dữ liệu dưới dạng object trong bucket.
</details>

---

### Question 2
S3 Standard-Infrequent Access (Standard-IA) phù hợp nhất cho?

A. Dữ liệu truy cập thường xuyên  
B. Dữ liệu ít truy cập nhưng cần truy xuất nhanh  
C. Dữ liệu lưu trữ dài hạn, truy xuất chậm  
D. Dữ liệu cần phân tích thời gian thực

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Standard-IA dành cho dữ liệu ít truy cập nhưng khi cần phải truy cập nhanh, chi phí lưu trữ thấp hơn Standard, phí truy xuất.
</details>

---

### Question 3
Dịch vụ nào cung cấp block storage cho EC2?

A. Amazon S3  
B. Amazon EBS  
C. Amazon Glacier  
D. AWS Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Amazon EBS (Elastic Block Store) cung cấp block storage bền vững gắn với EC2 instances.
</details>

---

### Question 4
Amazon EFS phù hợp cho loại workload nào?

A. Ứng dụng cần object storage  
B. Ứng dụng cần file system chia sẻ giữa nhiều instance  
C. Dữ liệu archive dài hạn  
D. Dữ liệu NoSQL

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Amazon EFS là file system elastic, có thể mount trên nhiều EC2/EKS, phù hợp chia sẻ dữ liệu.
</details>

---

### Question 5
Dịch vụ nào hỗ trợ chuyển dữ liệu lớn bằng thiết bị vật lý?

A. AWS DataSync  
B. AWS Storage Gateway  
C. AWS Snowball  
D. Amazon S3 Transfer Acceleration

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** AWS Snowball/Snowball Edge là thiết bị chuyển dữ liệu vật lý dùng cho bulk transfer hoặc edge computing.
</details>

---

### Question 6
Amazon S3 Glacier Instant Retrieval có thời gian truy xuất khoảng?

A. Milliseconds  
B. Vài phút đến giờ  
C. Vài giờ đến ngày  
D. Không thể truy xuất

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Glacier Instant Retrieval cung cấp độ trễ mili giây với chi phí lưu trữ thấp, phù hợp dữ liệu truy cập theo chu kỳ.
</details>

---

### Question 7
AWS Storage Gateway dạng File Gateway cung cấp?

A. Giao diện block iSCSI  
B. SMB/NFS share kết hợp lưu trữ trên S3  
C. Máy chủ backup tape ảo  
D. Kênh truyền dữ liệu thời gian thực

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** File Gateway cung cấp SMB/NFS share on-prem lưu trữ ở S3 với cache cục bộ.
</details>

---

### Question 8
AWS DataSync được dùng để?

A. Sao lưu cơ sở dữ liệu RDS  
B. Di chuyển dữ liệu nhanh giữa on-prem và AWS hoặc giữa dịch vụ AWS  
C. Quản lý object versions  
D. Mã hóa dữ liệu S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** DataSync tự động hóa và tăng tốc chuyển dữ liệu giữa NFS, SMB, S3, EFS, FSx... với tích hợp bảo mật.
</details>

---

### Question 9
S3 Versioning giúp?

A. Tăng tốc download  
B. Lưu trữ nhiều phiên bản object để khôi phục khi cần  
C. Mã hóa dữ liệu  
D. Giảm chi phí lưu trữ

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Versioning giữ lịch sử object, hỗ trợ khôi phục khi bị xóa/ghi đè.
</details>

---

### Question 10
S3 Transfer Acceleration tối ưu cho tình huống nào?

A. Upload từ client toàn cầu cần độ trễ thấp đến S3  
B. Chuyển dữ liệu giữa VPC  
C. Backup cơ sở dữ liệu  
D. Truy cập on-prem

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Transfer Acceleration tận dụng edge của CloudFront để tăng tốc upload/download khoảng cách xa đến S3.
</details>

---

### Question 11
Lifecycle policy của S3 dùng để?

A. Tự động chuyển đổi storage class theo thời gian  
B. Mã hóa object  
C. Xóa bucket  
D. Tạo IAM policy

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Lifecycle policy định nghĩa quy tắc chuyển object giữa storage class hoặc xóa sau thời gian nhất định.
</details>

---

### Question 12
Loại EBS volume nào phù hợp cho workload transactional (database)?

A. Throughput Optimized HDD (st1)  
B. Cold HDD (sc1)  
C. General Purpose SSD (gp3/gp2)  
D. Magnetic

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** General Purpose SSD cho IOps cân bằng giá/hiệu năng, phù hợp database transactional cỡ vừa. Với yêu cầu IO cao hơn dùng io1/io2.
</details>

---

### Question 13
EBS snapshot lưu ở đâu?

A. Trên local disk instance  
B. Trong Amazon S3 (managed)  
C. Trong Amazon EFS  
D. Trên Glacier

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** EBS snapshot lưu trong backend S3-managed, incremental, không cần quản lý bucket.
</details>

---

### Question 14
S3 SSE-S3 là gì?

A. Mã hóa phía client  
B. Mã hóa phía server do S3 quản lý khóa  
C. Mã hóa bằng khóa KMS do khách hàng quản lý  
D. Không phải mã hóa

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** SSE-S3 (Server-Side Encryption with S3 Managed Keys) sử dụng khóa do S3 quản lý tự động.
</details>

---

### Question 15
S3 Intelligent-Tiering phù hợp khi?

A. Biết rõ pattern truy cập  
B. Không biết pattern truy cập, cần tự động chuyển cấp lưu trữ  
C. Cần hiệu năng cao nhất  
D. Cần lưu trữ ở on-prem

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Intelligent-Tiering tự động phân loại object theo pattern truy cập, tối ưu chi phí với phí giám sát nhỏ.
</details>

---

### Question 16
Dịch vụ nào cung cấp NAS hoàn toàn managed dựa trên Windows?

A. Amazon FSx for Windows File Server  
B. Amazon EFS  
C. Amazon S3  
D. AWS Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** FSx for Windows File Server cung cấp file system Windows native, SMB, Active Directory integration.
</details>

---

### Question 17
Amazon FSx for Lustre phù hợp cho?

A. Ứng dụng HPC đòi hỏi throughput cao  
B. Ứng dụng IoT  
C. Email server  
D. Dịch vụ web serverless

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** FSx for Lustre cung cấp high-performance file system, tối ưu HPC, ML, video rendering.
</details>

---

### Question 18
Glacier Flexible Retrieval (trước kia Standard) có thời gian truy xuất?

A. Milliseconds  
B. Minutes  
C. Hours  
D. Days

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Glacier Flexible Retrieval cho phép truy xuất trong vài phút (từ 1-5 phút) hoặc chậm hơn tùy cấp.
</details>

---

### Question 19
S3 Object Lock giúp?

A. Xóa object nhanh hơn  
B. Bảo vệ object khỏi bị xóa/ghi đè theo thời gian WORM  
C. Tăng throughput  
D. Mã hóa

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Object Lock cung cấp Write-Once-Read-Many, phù hợp tuân thủ khi cần giữ dữ liệu không thể chỉnh sửa trong thời gian.
</details>

---

### Question 20
Cross-Region Replication (CRR) của S3 yêu cầu?

A. Bật versioning cho cả hai bucket  
B. Không cần IAM  
C. Chỉ cần bucket cùng region  
D. Không hỗ trợ SSE-KMS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CRR yêu cầu bật versioning ở bucket nguồn và đích, IAM role replication để sao chép object.
</details>

---

### Question 21
S3 Access Points giúp?

A. Tăng dung lượng bucket  
B. Định nghĩa endpoint riêng với policy cho từng ứng dụng truy cập bucket  
C. Mã hóa dữ liệu  
D. Sao lưu

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Access Points tạo endpoint riêng, gắn policy riêng, giúp quản lý truy cập theo ứng dụng/dataset.
</details>

---

### Question 22
Dịch vụ nào hỗ trợ backup đa dịch vụ (EBS, RDS, DynamoDB, EFS...)?

A. AWS Backup  
B. AWS DataSync  
C. Storage Gateway  
D. Snowball

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** AWS Backup cung cấp quản lý backup tập trung, policy-driven cho nhiều dịch vụ AWS.
</details>

---

### Question 23
EBS Multi-Attach cho phép?

A. Gắn cùng volume vào nhiều AZ  
B. Gắn io1/io2 volume vào nhiều instance trong cùng AZ  
C. Gắn gp3 vào nhiều instance toàn vùng  
D. Tự động backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Multi-Attach hỗ trợ io1/io2 gắn tới 16 instances trong cùng AZ, dùng cho ứng dụng cluster-aware.
</details>

---

### Question 24
EBS gp3 so với gp2 mang lại lợi ích?

A. Throughput cố định thấp hơn  
B. Chọn IOPS/Tput độc lập với dung lượng  
C. Tự động replicate giữa region  
D. Rẻ hơn sc1

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** gp3 cho phép cấu hình IOPS và throughput tách biệt dung lượng, chi phí tốt hơn gp2.
</details>

---

### Question 25
S3 object mặc định có trạng thái chia sẻ công khai?

A. Có  
B. Không, mặc định private  
C. Tùy bucket policy  
D. Depends on IAM user

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** S3 object mặc định private, cần explicit permission để public.
</details>

---

### Question 26
EFS có hai mode throughput chính?

A. Standard và One Zone  
B. General Purpose và Max I/O  
C. Bursting và Provisioned  
D. Cold và Warm

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** EFS throughput modes: Bursting (default) và Provisioned. Ngoài ra performance mode General Purpose vs Max I/O.
</details>

---

### Question 27
S3 Select giúp?

A. Truy vấn một phần dữ liệu object (CSV, JSON, parquet)  
B. Mã hóa  
C. Chuyển region  
D. Replication

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** S3 Select cho phép truy vấn 1 phần object sử dụng SQL-like, giảm dữ liệu truyền tải.
</details>

---

### Question 28
Storage Lens cung cấp?

A. Dashboard phân tích usage và activity của S3  
B. Mã hóa tự động  
C. Dịch vụ backup  
D. Chuyển dữ liệu

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** S3 Storage Lens cung cấp phân tích, khuyến nghị tối ưu hóa chi phí, độ bền, security cho S3.
</details>

---

### Question 29
AWS Backup Vault Lock tương tự S3 Object Lock ở chỗ?

A. Không cần IAM  
B. Cung cấp bảo vệ WORM cho backup  
C. Giảm chi phí  
D. Chỉ dùng cho tape

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Backup Vault Lock ngăn xóa/sửa backup (WORM) đáp ứng compliance tương tự Object Lock.
</details>

---

### Question 30
S3 Bucket policy hỗ trợ điều gì?

A. Đặt rule truy cập ở cấp bucket  
B. Mã hóa  
C. Tạo version  
D. Quản lý billing

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Bucket policy định nghĩa IAM policy attach trực tiếp vào bucket để cho phép/deny truy cập.
</details>

---

### Question 31
Cổng VPC Gateway Endpoint hỗ trợ dịch vụ nào?

A. S3 và DynamoDB  
B. EFS và FSx  
C. Glacier và Backup  
D. Snowball

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Gateway Endpoint cho phép truy cập riêng tư đến S3/DynamoDB mà không qua internet.
</details>

---

### Question 32
S3 Multipart Upload dùng để?

A. Mã hóa  
B. Upload object lớn (>5 GB) hiệu quả, song song  
C. Phân quyền  
D. Xóa object

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Multipart upload chia object thành phần, upload song song, dùng cho file lớn.
</details>

---

### Question 33
FSx for Lustre có thể import dữ liệu trực tiếp từ?

A. S3 bucket  
B. DynamoDB  
C. RDS  
D. Glacier

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** FSx for Lustre có thể link S3 bucket làm data repository, sync dữ liệu qua lại.
</details>

---

### Question 34
AWS Backup hỗ trợ backup on-prem thông qua?

A. AWS Direct Connect  
B. AWS Backup Gateway (trước là Storage Gateway integration)  
C. AWS Global Accelerator  
D. Route 53

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** AWS Backup sử dụng Backup Gateway để quản lý backup on-prem VMware/Hyper-V lên AWS.
</details>

---

### Question 35
S3 Block Public Access giúp?

A. Tự động phát hiện malware  
B. Chặn thiết lập public cho bucket/object ở cấp account hoặc bucket  
C. Tối ưu chi phí  
D. Tăng throughput

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Block Public Access ngăn tạo ACL/policy cho phép public, tăng bảo mật S3.
</details>

---

### Question 36
EBS Snapshots có thể copy cross-region nhằm?

A. Multiregion backup và DR  
B. Tăng throughput  
C. Giảm chi phí  
D. Hỗ trợ encryption

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Copy snapshot sang region khác cho mục đích DR hoặc triển khai EC2 ở region mới.
</details>

---

### Question 37
S3 Event Notifications có thể trigger dịch vụ nào?

A. AWS Lambda  
B. Amazon RDS  
C. Amazon CloudFront  
D. AWS Glue DataBrew

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Event notifications gửi sự kiện đến Lambda, SNS, SQS, EventBridge khi object thay đổi.
</details>

---

### Question 38
EFS One Zone phù hợp khi?

A. Cần HA nhiều AZ  
B. Muốn tiết kiệm chi phí cho workload không critical trong 1 AZ  
C. Cần on-prem caching  
D. Cần throughput tối đa

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** EFS One Zone lưu dữ liệu trong một AZ, chi phí thấp hơn, phù hợp workload không đòi hỏi multi-AZ.
</details>

---

### Question 39
Amazon S3 Object Storage phân biệt với EBS ở điểm?

A. Object storage truy cập qua API, không mount trực tiếp như block storage  
B. Dung lượng tối đa nhỏ hơn  
C. Không hỗ trợ versioning  
D. Không thể public

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** S3 là object storage, truy cập qua HTTP API; EBS là block storage gắn vào hệ điều hành.
</details>

---

### Question 40
S3 Presigned URL dùng để?

A. Cấp quyền truy cập tạm thời cho object  
B. Mã hóa dữ liệu  
C. Backup snapshot  
D. Chạy analytics

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Presigned URL cho phép user không có credentials truy cập object trong thời gian giới hạn.
</details>

---

### Question 41
FSx for NetApp ONTAP nổi bật với?

A. Hỗ trợ giao thức NFS, SMB và tính năng ONTAP như Snapshots, cloning  
B. Chỉ NFS  
C. Chỉ SMB  
D. Không hỗ trợ replication

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** FSx for ONTAP cung cấp đầy đủ tính năng NetApp: NFS/SMB/iSCSI, Snapshot, cloning, data dedup.
</details>

---

### Question 42
S3 Access Analyzer giúp?

A. Phân tích bucket policy và cảnh báo quyền public/unintended access  
B. Mã hóa  
C. Backup  
D. Nén object

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** S3 Access Analyzer (IAM Access Analyzer) kiểm tra policy, phát hiện truy cập từ outside account.
</details>

---

### Question 43
Glacier Deep Archive phù hợp cho?

A. Dữ liệu cần truy xuất milli-second  
B. Lưu trữ dài hạn ít truy xuất nhất, chi phí thấp nhất  
C. Dữ liệu cần chia sẻ real-time  
D. Dữ liệu không thể mã hóa

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Glacier Deep Archive dành cho dữ liệu truy xuất hiếm, chi phí thấp nhất, thời gian truy xuất 12 giờ.
</details>

---

### Question 44
EBS encryption có thể bật bằng?

A. Chỉ AWS CLI  
B. Console, API/CLI, bằng KMS key  
C. Không thể  
D. Chỉ when creating snapshot

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** EBS hỗ trợ encryption at-rest bằng KMS key khi tạo volume/snapshot, qua console/CLI/API.
</details>

---

### Question 45
S3 Inventory dùng để?

A. Thống kê object hàng ngày/tuần, metadata, phục vụ audit  
B. Mã hóa  
C. Backup  
D. Replicate

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** S3 Inventory tạo report (CSV/ORC/Parquet) liệt kê object, metadata, hỗ trợ audit và compliance.
</details>

---

### Question 46
AWS Transfer Family cung cấp?

A. Giao thức quản lý đối tượng  
B. SFTP/FTPS/FTP managed service kết nối S3/EFS  
C. Giao thức HTTP  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Transfer Family cho phép client dùng SFTP/FTPS/FTP upload/download dữ liệu vào S3/EFS.
</details>

---

### Question 47
Amazon Macie liên quan S3 thế nào?

A. Công cụ phát hiện dữ liệu nhạy cảm (PII) trong S3 bằng machine learning  
B. Sao lưu S3  
C. Quản lý lifecycle  
D. Mã hóa

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Macie dùng machine learning phát hiện dữ liệu nhạy cảm trong S3, cảnh báo rủi ro bảo mật.
</details>

---

### Question 48
Hybrid cloud caching cần lưu trữ file gần on-prem, nên dùng?

A. Storage Gateway Cached Volume  
B. S3 Standard  
C. EBS  
D. Lambda

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Storage Gateway Cached Volume lưu dữ liệu chính ở S3, cache on-prem giảm latency.
</details>

---

### Question 49
S3 Replication Time Control (RTC) đảm bảo?

A. Times to replicate object cross-region < 15 phút  
B. Mã hóa  
C. Tăng throughput  
D. Sao lưu

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** RTC đảm bảo SLA replication dưới 15 phút cross-region, phục vụ compliance.
</details>

---

### Question 50
S3 EventBridge integration giúp?

A. Nhận sự kiện object tạo/xóa gần real-time qua EventBridge bus  
B. Mã hóa  
C. Backup  
D. Copy object

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** EventBridge nhận sự kiện tăng cường từ S3, tích hợp với nhiều target hơn S3 notifications truyền thống.
</details>

---

## Phần B - Câu hỏi khó (30 câu)

### Question 51
Bạn có hàng tỷ object nhỏ trong S3, truy cập theo event unpredictable. Giải pháp tối ưu chi phí nhưng vẫn cần millisecond access?

A. Standard-IA  
B. Intelligent-Tiering với archive tiers bật Deep Archive Access  
C. Glacier Flexible  
D. Glacier Deep Archive

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Intelligent-Tiering tự động phân chia, có thể bật các tier archive access cho object ít truy cập, vẫn giữ millisecond ở Frequent/IA. Đáp ứng pattern khó đoán.
</details>

---

### Question 52
Workload Big Data trên EMR cần file system high throughput, gắn S3 làm nguồn chính, nên dùng?

A. EFS  
B. FSx for Lustre linked S3 (data repository)  
C. Storage Gateway  
D. EBS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** FSx for Lustre tích hợp S3, cung cấp throughput cao (100s GB/s), phù hợp analytics/ML.
</details>

---

### Question 53
Bạn cần enforce rằng mọi EBS snapshot đều được mã hóa với CMK tùy chỉnh. Triển khai?

A. AWS Config rule + Lambda automation + EBS default encryption với CMK  
B. IAM policy  
C. Chỉ rely vào user  
D. Không làm được

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Bật default encryption với CMK tùy chỉnh; dùng AWS Config rule kiểm tra snapshot không mã hóa và trigger Lambda remediation.
</details>

---

### Question 54
Bạn muốn replication giữa hai bucket thuộc hai account, sử dụng SSE-KMS. Yêu cầu?

A. Không thể với SSE-KMS  
B. Chia sẻ CMK giữa account, thiết lập policy cho phép replicate và role replication  
C. Không cần gì thêm  
D. Chỉ SSE-S3 hỗ trợ

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Cần CMK cho phép account nguồn/replication role sử dụng; thiết lập policy đúng cho bucket và KMS.
</details>

---

### Question 55
Ứng dụng analytics cần query trực tiếp dữ liệu trong S3 bằng SQL, không di chuyển dữ liệu. Hai dịch vụ phù hợp?

A. Athena và Redshift Spectrum  
B. Glue và DynamoDB  
C. CloudWatch Logs  
D. EBS và Lambda

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Athena (serverless) và Redshift Spectrum cho phép query dữ liệu S3 trực tiếp bằng SQL.
</details>

---

### Question 56
Bạn có workload on-prem cần truy cập low latency tới dữ liệu lưu trên S3. Dịch vụ tối ưu?

A. S3 Transfer Acceleration  
B. File Gateway hoặc Cached Volume để cache cục bộ  
C. DataSync  
D. Snowball

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Storage Gateway cung cấp cache tại chỗ, truy cập qua NFS/SMB, dữ liệu chính ở S3.
</details>

---

### Question 57
Bạn cần tuân thủ quy định giữ log không thể chỉnh sửa 7 năm. Giải pháp?

A. Lưu S3 với Object Lock Compliance mode + lifecycle chuyển Deep Archive sau 1 năm  
B. S3 Standard-IA  
C. Glacier Flexible  
D. EBS snapshot

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Object Lock compliance mode đảm bảo WORM, lifecycle giúp tối ưu chi phí chuyển sang Deep Archive.
</details>

---

### Question 58
Bạn muốn replicate chỉ một tập hợp object (prefix cụ thể) và bỏ qua metadata tùy chỉnh. Cấu hình?

A. S3 replication filtering theo prefix + lựa chọn không sao chép metadata  
B. S3 replication mặc định  
C. Bucket policy  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Replication rules hỗ trợ filter theo prefix/tag. Có thể bỏ sao chép storage class, ACL, metadata tùy chọn.
</details>

---

### Question 59
Khối lượng dữ liệu 5PB cần di chuyển vào AWS trong 3 tuần, băng thông mạng hạn chế. Giải pháp khả thi?

A. DataSync  
B. Snowball Edge hoặc Snowmobile tùy khối lượng  
C. Transfer Family  
D. VPN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Khối lượng rất lớn, Snowball Edge (tối đa ~80TB mỗi thiết bị) hoặc Snowmobile (tới 100PB) phù hợp.
</details>

---

### Question 60
Muốn audit quyền truy cập cross-account đến S3 bucket, nên dùng?

A. S3 Access Analyzer + CloudTrail data events  
B. CloudWatch  
C. Route 53  
D. Inspector

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Access Analyzer phát hiện policy cấp quyền công khai/cross-account; CloudTrail ghi log truy cập chi tiết.
</details>

---

### Question 61
Ứng dụng web đa AZ cần chia sẻ cấu hình và tài sản tĩnh giữa nhiều instance. Nên dùng?

A. Amazon EFS với performance mode General Purpose  
B. Amazon S3 Standard  
C. Amazon FSx for Lustre  
D. Amazon Glacier

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** EFS là file system multi-AZ, cho phép nhiều EC2 truy cập đồng thời với độ trễ thấp, phù hợp web/app server cần chia sẻ file.
</details>

---

### Question 62
Bạn muốn đảm bảo mọi object upload vào S3 được gắn tag `data-classification=confidential`. Giải pháp tự động?

A. AWS CloudTrail  
B. S3 Object Lambda  
C. S3 Event kết hợp Lambda sửa tag trên PUT  
D. IAM policy deny nếu không có tag + yêu cầu header x-amz-tagging

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** D  
**Giải thích:** IAM policy có thể deny PUT nếu thiếu header tag mong muốn, buộc client gửi tag khi upload.
</details>

---

### Question 63
Bạn cần storage cho SAP HANA on AWS với shared file system high throughput, tuân thủ SAP. Chọn?

A. Amazon EFS  
B. Amazon FSx for NetApp ONTAP  
C. Amazon FSx for OpenZFS  
D. Amazon S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** FSx for ONTAP được chứng nhận cho nhiều workload doanh nghiệp như SAP, hỗ trợ NFS/SMB, snapshot, throughput cao.
</details>

---

### Question 64
Team ML cần chia sẻ dataset 200 TB lưu trên S3, training cluster ở nhiều account khác nhau. Giải pháp tối ưu?

A. Copy dữ liệu sang từng account  
B. S3 Access Point + VPC Access Point + Bucket policy cross-account  
C. Dùng Glacier  
D. Chuyển sang EFS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** S3 Access Point chuyên dụng cho từng account/VPC, quản lý policy riêng, tránh phải copy dữ liệu.
</details>

---

### Question 65
Bạn cần khôi phục dữ liệu EFS về trạng thái 1 tuần trước do ransomware. Công cụ?

A. EFS-to-S3 sync  
B. EFS Backup bằng AWS Backup hoặc EFS native backup  
C. CloudFront  
D. EBS snapshot

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** AWS Backup hoặc EFS backup tích hợp cho phép point-in-time recovery, phù hợp kịch bản ransomware.
</details>

---

### Question 66
Bạn vận hành ứng dụng cần replicate EBS volume giữa hai AZ để failover tự động. Cách tiếp cận?

A. EBS volume tự động replicate multi-AZ  
B. Dùng Amazon Data Lifecycle Manager hoặc AWS Backup tạo snapshot rồi restore sang AZ khác  
C. Dùng S3  
D. Dùng EFS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** EBS không tự replicate multi-AZ. Sử dụng snapshot (DLM/Backup) để sao lưu và restore tại AZ khác khi cần.
</details>

---

### Question 67
Workload yêu cầu throughput tuyến tính theo kích thước file system, tối đa hóa IO. Với EFS nên dùng?

A. Throughput mode Bursting  
B. Throughput mode Provisioned + performance mode Max I/O  
C. One Zone  
D. Lifecycle policy

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Provisioned throughput đảm bảo tput cố định độc lập dung lượng, Max I/O cho phép concurrency cao.
</details>

---

### Question 68
Dữ liệu nhạy cảm cần được mã hóa client-side trước khi vào S3, AWS chỉ lưu bản mã. Công cụ?

A. SSE-S3  
B. SSE-KMS  
C. S3 Encryption Client (SDK) hoặc AWS Encryption SDK cho Client-Side Encryption  
D. S3 Access Analyzer

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** Client-side encryption bằng SDK giúp mã hóa trước khi gửi lên S3; SSE-KMS/SSE-S3 mã hóa phía server.
</details>

---

### Question 69
Bạn muốn di chuyển dữ liệu từ Google Cloud Storage sang S3 nhanh chóng. Dịch vụ?

A. DataSync với agent hỗ trợ GCS  
B. Snowball  
C. EFS  
D. Transfer Family

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** DataSync hỗ trợ GCS lẫn Azure Blob như nguồn, chuyển dữ liệu trực tiếp sang S3/EFS/FSx.
</details>

---

### Question 70
Workload phân tích log cần lưu vào S3 với partition theo ngày để query hiệu quả. Làm thế nào?

A. Dùng S3 Lifecycle  
B. Sử dụng Glue ETL hoặc Lambda để tổ chức prefix `year=YYYY/month=MM/day=DD`  
C. Dùng S3 Select  
D. Không cần

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Partition theo prefix giúp Athena/Redshift Spectrum query hiệu quả; Glue/Lambda tự động phân loại khi ingest.
</details>

---

### Question 71
Cần đảm bảo rằng nếu replication thất bại, bạn được cảnh báo ngay. Công nghệ?

A. S3 Replication Metrics + CloudWatch Alarms  
B. CloudTrail  
C. Access Analyzer  
D. AWS Shield

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Replication metrics cung cấp số liệu thời gian, có thể đặt alarm khi danh sách pending object vượt ngưỡng.
</details>

---

### Question 72
Bạn có ứng dụng legacy sử dụng SMB và cần lưu trữ dữ liệu gần như real-time trên AWS với backup tự động. Chọn?

A. FSx for Windows File Server + AWS Backup  
B. EFS  
C. S3  
D. Glacier

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** FSx for Windows hỗ trợ SMB native, tích hợp Windows ACL; AWS Backup bảo vệ snapshots tự động.
</details>

---

### Question 73
Muốn giảm chi phí EFS khi file ít sử dụng. Tính năng?

A. EFS Infrequent Access (IA) lifecycle policy tự động chuyển file  
B. EBS snapshot  
C. S3 lifecycle  
D. Glacier

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** EFS lifecycle policy chuyển file không truy cập sang EFS IA (chi phí thấp hơn) sau khoảng thời gian cấu hình.
</details>

---

### Question 74
Bạn đang dùng Storage Gateway Tape Gateway. Dữ liệu lưu ở lớp nào?

A. EBS  
B. S3 Glacier Flexible Retrieval/Deep Archive tùy cấu hình  
C. DynamoDB  
D. Redshift

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Tape Gateway lưu dữ liệu băng ảo trên S3 Glacier Flex hoặc Deep Archive, mô phỏng tape offsite.
</details>

---

### Question 75
Bạn muốn theo dõi chính xác chi phí từng nhóm dự án dùng chung S3 bucket. Làm sao?

A. Cost Explorer mặc định  
B. Dùng S3 storage class  
C. Gắn Cost Allocation Tag trên object (qua tagging hoặc manifest) và bật trong Billing  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** Tag object hoặc bucket với cost allocation tag, bật trong billing để phân tích chi phí theo dự án.
</details>

---

### Question 76
Bạn cần expose dữ liệu S3 qua REST API tùy chỉnh kèm xác thực, không muốn client truy cập trực tiếp S3. Giải pháp?

A. API Gateway + Lambda proxy S3 + IAM/Authorizer  
B. Public bucket  
C. Transfer Family  
D. Snowball

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** API Gateway front-end, Lambda xử lý logic/ủy quyền, truy cập S3 bằng IAM role, tránh expose trực tiếp.
</details>

---

### Question 77
Amazon S3 cung cấp bao nhiêu request PUT/GET mặc định mỗi prefix?

A. Không giới hạn, scale horizontal bằng cách dùng nhiều prefix  
B. 100 requests/s  
C. 1000 requests/s  
D. 5500 GET và 3500 PUT per prefix (giới hạn cũ)

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** S3 hiện hỗ trợ automatic scaling, không giới hạn cứng per prefix như trước; khuyến nghị dùng key design tốt để song song.
</details>

---

### Question 78
Bạn cần mount file system POSIX trên container ECS Fargate. Lựa chọn?

A. S3 direct  
B. EFS integration với Fargate  
C. EBS  
D. Glacier

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Fargate hỗ trợ mount EFS để cung cấp shared POSIX storage cho container.
</details>

---

### Question 79
Giải pháp DR cho on-premises SQL Server: replicate log lên AWS và khôi phục nhanh. Công cụ?

A. Storage Gateway Volume Gateway (stored mode) + EC2  
B. Snowball  
C. S3  
D. DynamoDB

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Volume Gateway stored mode giữ dữ liệu chính on-prem, replicate snapshot lên S3, có thể khôi phục lên EC2 cho DR.
</details>

---

### Question 80
Bạn muốn tự động phát hiện dữ liệu PII tải lên S3 và cảnh báo security team. Kiến trúc?

A. S3 Event -> Amazon Macie -> Security Hub/SNS  
B. CloudWatch -> SQS  
C. EFS -> Lambda  
D. Glacier -> SNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Macie scan S3, phát hiện PII, gửi findings tới Security Hub/SNS để cảnh báo tự động.
</details>

---
