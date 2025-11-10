# Monitoring & Management - Exam Questions V2

> 🧠 Mục tiêu: Nắm vững giám sát, vận hành, và quản trị trên AWS: CloudWatch, CloudTrail, Config, Systems Manager, X-Ray, EventBridge, Trusted Advisor, Health, Organizations/Control Tower, Service Catalog.  
> 📦 Nội dung: 50 câu nền tảng + 30 câu khó (tổng 80 câu) dạng multiple-choice/multiple-response

---

## Phần A - Câu hỏi nền tảng (50 câu)

### Question 1
Dịch vụ nào thu thập metrics, logs, alarms cho tài nguyên AWS?

A. AWS CloudTrail  
B. Amazon CloudWatch  
C. AWS Config  
D. AWS X-Ray

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** CloudWatch thu thập metrics, logs, events, và tạo alarms, dashboards.
</details>

---

### Question 2
CloudTrail dùng để?

A. Lưu API calls và hoạt động quản trị tài khoản  
B. Thu metrics CPU  
C. Bắt trace ứng dụng  
D. Quản lý cấu hình

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CloudTrail ghi nhận API events (management/data events) để audit, bảo mật, điều tra.
</details>

---

### Question 3
AWS Config cung cấp?

A. Log API  
B. Inventory cấu hình, compliance, và lịch sử thay đổi cấu hình tài nguyên  
C. CDN  
D. Caching

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Config theo dõi cấu hình, đánh giá compliance thông qua rules (managed/custom).
</details>

---

### Question 4
EventBridge (CloudWatch Events) dùng để?

A. Orchestrate workflow phức tạp  
B. Bus sự kiện để kết nối nguồn sự kiện và target (Lambda, Step Functions, etc.)  
C. Lưu logs  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** EventBridge cho phép build event-driven apps, filter theo pattern, schedule.
</details>

---

### Question 5
AWS X-Ray hỗ trợ?

A. Tracing phân tán cho ứng dụng để phân tích latency, lỗi  
B. DNS  
C. Backup  
D. Billing

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** X-Ray giúp phân tích request end-to-end, service map, root cause.
</details>

---

### Question 6
Trusted Advisor cung cấp gì?

A. Recommendations về cost, performance, security, fault tolerance, service limits  
B. CDN  
C. Secrets  
D. VPN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Trusted Advisor scan best practices và đề xuất tối ưu.
</details>

---

### Question 7
AWS Health (Personal Health Dashboard) cung cấp?

A. Trạng thái dịch vụ công khai  
B. Thông tin tác động cá nhân hóa tới tài nguyên của bạn khi có sự cố dịch vụ  
C. Pricing  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Health PHd cá nhân hóa theo tài nguyên tài khoản; Service Health Dashboard là công khai.
</details>

---

### Question 8
Systems Manager (SSM) cung cấp tính năng nào?

A. Patch Manager, Session Manager, Parameter Store, Automation  
B. CDN  
C. DNS  
D. Data warehouse

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** SSM là bộ công cụ vận hành cho EC2/on-prem/VMC.
</details>

---

### Question 9
Parameter Store vs Secrets Manager?

A. Cả hai đều không mã hóa  
B. Secrets Manager hỗ trợ rotation và tích hợp mạnh cho secrets; Parameter Store phù hợp config/kết hợp KMS  
C. Parameter Store chỉ plaintext  
D. Secrets Manager miễn phí

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Secrets Manager có rotation, charge theo secret; Parameter Store có free/standard tier, dùng KMS mã hóa.
</details>

---

### Question 10
CloudWatch Alarm có thể làm gì khi vi phạm ngưỡng?

A. Gửi SNS, gọi Auto Scaling, gọi EC2 action, gọi SSM OpsItem, EventBridge  
B. Backup tự động  
C. Đổi IAM  
D. Đổi DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Alarm kích hoạt action như SNS, scaling, EC2 recovery, EventBridge rule.
</details>

---

### Question 11
CloudWatch Logs retention mặc định?

A. Không giới hạn (infinite) trừ khi cấu hình retention  
B. 1 ngày  
C. 7 ngày  
D. 30 ngày

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Mặc định giữ vô hạn, có thể đặt retention theo nhu cầu.
</details>

---

### Question 12
CloudWatch Logs Insights dùng để?

A. Query logs với ngôn ngữ truy vấn riêng, trực quan hóa nhanh  
B. Tạo dashboard billing  
C. Tạo S3 bucket  
D. Chạy Spark

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Logs Insights cho phép phân tích logs hiệu quả.
</details>

---

### Question 13
CloudWatch Metric filter dùng để?

A. Chuyển đổi log thành custom metric dựa trên pattern  
B. Đổi permission  
C. Backup  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Metric filter tạo metric từ logs để đặt alarm dễ dàng.
</details>

---

### Question 14
AWS Organizations cung cấp?

A. Quản trị đa tài khoản, consolidated billing, SCP  
B. CDN  
C. Security Group  
D. EBS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Organizations cho multi-account governance, guardrails (SCP).
</details>

---

### Question 15
Control Tower là?

A. Dịch vụ thiết lập landing zone multi-account với guardrails best practices  
B. CDN  
C. Backup  
D. Database

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Control Tower tự động hóa tạo OU, account, guardrails, SSO tích hợp.
</details>

---

### Question 16
Service Catalog dùng để?

A. Danh mục sản phẩm CNTT chuẩn hóa (CFN template), tự phục vụ  
B. CDN  
C. DNS  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Cho phép tổ chức publish danh mục tài nguyên chuẩn cho dev tự triển khai.
</details>

---

### Question 17
CloudWatch Agent dùng để?

A. Thu thập OS-level metrics/logs từ EC2/on-prem  
B. DNS  
C. Backup  
D. ETL

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Agent gửi metrics như memory, disk, logs lên CloudWatch.
</details>

---

### Question 18
EC2 status check alarms dùng để?

A. Restart instance khi hardware lỗi (EC2 recovery)  
B. Backup  
C. đổi VPC  
D. Đổi SG

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** EC2 action có thể auto-recover khi status check fail (system).
</details>

---

### Question 19
SSM Session Manager ưu điểm?

A. Truy cập shell/PowerShell không cần mở inbound SSH/RDP, audit đầy đủ  
B. Nhanh hơn SSH  
C. Rẻ hơn NAT  
D. Không cần IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Session Manager bảo mật, audit, không mở cổng inbound.
</details>

---

### Question 20
SSM Parameter Store loại tham số?

A. String, StringList, SecureString (KMS)  
B. JSON  
C. Binary bắt buộc  
D. Chỉ plaintext

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** SecureString dùng KMS mã hóa.
</details>

---

### Question 21
CloudWatch anomaly detection làm gì?

A. Học mô hình cho metric và phát hiện bất thường tự động  
B. Tạo logs  
C. DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Dùng ML để phát hiện anomaly trên metrics.
</details>

---

### Question 22
CloudWatch Synthetics Canary dùng để?

A. Giả lập người dùng, kiểm tra endpoint theo lịch, cảnh báo khi lỗi  
B. Backup  
C. DNS  
D. Build container

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Canaries kiểm tra synthetic monitoring đa điểm.
</details>

---

### Question 23
CloudWatch Dashboard dùng để?

A. Visualization metrics cross-account/region (nếu bật)  
B. Backup  
C. DNS  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Dashboard tùy biến để theo dõi metrics trọng yếu.
</details>

---

### Question 24
CloudTrail data events áp dụng cho?

A. S3 object-level, Lambda invoke-level  
B. EC2 API  
C. IAM  
D. Route 53

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Data events chi tiết hơn, tốn phí riêng.
</details>

---

### Question 25
AWS Health vs Service Health Dashboard?

A. Giống nhau  
B. Health cá nhân hóa theo tài nguyên của bạn; Service Health công khai theo region/service  
C. Health công khai  
D. Không khác biệt

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Health cung cấp tác động cụ thể tới bạn.
</details>

---

### Question 26
AWS Compute Optimizer liên quan monitoring?

A. Đưa khuyến nghị tối ưu kích cỡ EC2, Lambda, EBS dựa trên metrics sử dụng  
B. Backup  
C. CDN  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Dùng metrics CloudWatch để recommend resources phù hợp.
</details>

---

### Question 27
AWS Application Insights dùng để?

A. Phát hiện bất thường ứng dụng .NET/SQL/… và tạo dashboard/alarms tự động  
B. CDN  
C. Backup  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Service giúp quan sát ứng dụng enterprise nhanh chóng.
</details>

---

### Question 28
Systems Manager Automation runbook dùng để?

A. Quy trình tự động remediation/sao lưu/patching được chuẩn hóa  
B. DNS  
C. Build  
D. CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Runbook định nghĩa step-by-step automation với approval/rollback.
</details>

---

### Question 29
OpsCenter (Systems Manager) cung cấp?

A. Tạo, theo dõi, và khắc phục sự cố (OpsItems) liên kết metrics/logs/alarms  
B. CDN  
C. DNS  
D. Billing

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** OpsCenter tập trung hóa incidents/operations issues.
</details>

---

### Question 30
Inventory (SSM) làm gì?

A. Thu thập inventory phần mềm/phần cứng EC2/on-prem theo lịch  
B. CDN  
C. DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Inventory cho CMDB cơ bản về tài sản CNTT.
</details>

---

### Question 31
Patch Manager dùng để?

A. Tự động vá hệ điều hành/ứng dụng theo baseline và lịch  
B. CDN  
C. DNS  
D. Billing

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Patch Manager tự động hóa patch compliance.
</details>

---

### Question 32
State Manager dùng để?

A. Duy trì trạng thái cấu hình mong muốn của các instance  
B. CDN  
C. DNS  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tự động áp cấu hình (document) theo lịch.
</details>

---

### Question 33
AWS Organizations SCP dùng để?

A. Giới hạn tối đa hành động IAM có thể làm trong account/OU  
B. Tạo user  
C. Billing  
D. CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** SCP là guardrail cấp tổ chức, không cấp quyền mà chỉ giới hạn.
</details>

---

### Question 34
CloudWatch cross-account observability?

A. Không có  
B. Cho phép chia sẻ metrics/logs/traces giữa accounts để quan sát tập trung  
C. Chỉ logs  
D. Chỉ metrics

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** B  
**Giải thích:** Hỗ trợ hub/spoke để tập trung quan sát multi-account.
</details>

---

### Question 35
CloudWatch Contributor Insights dùng để?

A. Phân tích top-n contributors trong logs/metrics  
B. DNS  
C. Backup  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Cho biết tác nhân lớn nhất gây load/lỗi.
</details>

---

### Question 36
CloudTrail Lake giúp?

A. Lưu trữ và truy vấn logs CloudTrail bằng SQL lâu dài  
B. CDN  
C. DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** CloudTrail Lake hỗ trợ phân tích nâng cao sự kiện.
</details>

---

### Question 37
AWS Chatbot dùng để?

A. Nhận thông báo SNS/CloudWatch/Code* vào Slack/Chime, tương tác lệnh  
B. DNS  
C. Backup  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** ChatOps để vận hành qua kênh chat.
</details>

---

### Question 38
CloudWatch Composite Alarms?

A. Kết hợp nhiều alarms bằng logic AND/OR để giảm nhiễu cảnh báo  
B. Chỉ một alarm  
C. Không hỗ trợ  
D. Chỉ cho EC2

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Composite alarms hữu ích cho SRE/operations.
</details>

---

### Question 39
Service Quotas tích hợp?

A. Theo dõi và yêu cầu tăng hạn mức dịch vụ AWS  
B. DNS  
C. Backup  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Quản lý hạn mức theo dịch vụ và region.
</details>

---

### Question 40
AWS Health Aware (AHA) là?

A. Giải pháp thông báo sự kiện Health tới kênh như Slack/Email, có sẵn sample solution  
B. DNS  
C. CDN  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** AHA là solution pattern sử dụng EventBridge/SES/SNS/Lambda.
</details>

---

### Question 41
Application/Infrastructure Monitoring khác nhau?

A. App monitoring: code-level, traces; Infra: metrics OS/resource  
B. Không khác  
C. Chỉ app  
D. Chỉ infra

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kết hợp cả hai để full observability.
</details>

---

### Question 42
Operational Excellence pillar trong Well-Architected tập trung?

A. Quy trình vận hành, quan sát, tự động hóa, phản hồi sự cố  
B. Bảo mật  
C. Hiệu năng  
D. Chi phí

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Pillar về vận hành hiệu quả, liên quan monitoring/management.
</details>

---

### Question 43
AWS Console Mobile App hỗ trợ?

A. Theo dõi tài nguyên, alarm cơ bản khi di động  
B. CDN  
C. Backup  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** App di động để xem trạng thái tài nguyên và alarm.
</details>

---

### Question 44
AWS Resource Groups dùng để?

A. Gom tài nguyên theo tag để xem/điều khiển theo nhóm  
B. CDN  
C. DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Quản lý theo tag giúp operations thuận tiện.
</details>

---

### Question 45
CloudWatch Kinesis Firehose integration dùng để?

A. Xuất logs sang S3/OpenSearch/Data Firehose để phân tích dài hạn  
B. DNS  
C. Backup  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Firehose chuyển dữ liệu log đến destinations analytics.
</details>

---

### Question 46
Centralized logging pattern?

A. Gửi logs đa tài khoản/region về một tài khoản phân tích qua Kinesis/Firehose/S3/OpenSearch  
B. Mỗi account tự phân tích  
C. Không cần  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Centralized giúp bảo mật và phân tích tập trung.
</details>

---

### Question 47
Run Command (SSM) dùng để?

A. Thực thi lệnh từ xa trên nhiều instance có IAM kiểm soát và audit  
B. DNS  
C. Backup  
D. CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Không cần SSH, kiểm soát bằng IAM/Logs.
</details>

---

### Question 48
Incident Manager (Systems Manager) là?

A. Công cụ quản lý sự cố: escalation, on-call, runbook, chat ops  
B. DNS  
C. Backup  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Điều phối response khi có sự cố.
</details>

---

### Question 49
Change Manager (SSM) giúp?

A. Quy trình phê duyệt và thực thi thay đổi cấu hình an toàn  
B. DNS  
C. Backup  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Chuẩn hóa change management có approval.
</details>

---

### Question 50
Phân biệt Alarm vs EventBridge rule?

A. Alarm dựa trên metric threshold; EventBridge rule dựa trên sự kiện/cron pattern  
B. Cả hai giống nhau  
C. Cả hai dựa trên logs  
D. Không có khác biệt

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Alarm -> metrics, EventBridge -> events/schedule.
</details>

---

## Phần B - Câu hỏi khó (30 câu)

### Question 51
Bạn muốn phát hiện cấu hình S3 public và tự động sửa. Kiến trúc?

A. AWS Config managed rule + EventBridge -> SSM Automation/Lambda để block public access  
B. CloudTrail  
C. NAT  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Compliance + remediation tự động là pattern phổ biến.
</details>

---

### Question 52
Bạn cần correlation trace giữa Lambda, ECS và RDS. Công cụ?

A. X-Ray với instrumentation SDK/Daemon, propagate trace headers  
B. CloudTrail  
C. NAT  
D. Trusted Advisor

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** X-Ray end-to-end tracing across services.
</details>

---

### Question 53
Giảm noisy alerts khi nhiều metrics biến động đồng thời?

A. Composite Alarms + Anomaly Detection + metric math  
B. Tăng ngưỡng  
C. Tắt alarm  
D. Chỉ gửi email

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kết hợp nhiều kỹ thuật để giảm nhiễu và false positives.
</details>

---

### Question 54
Giám sát log ứng dụng ở nhiều account/region, yêu cầu query tập trung real-time?

A. CloudWatch Logs subscription filter -> Kinesis Data Streams/Firehose -> OpenSearch central  
B. Mỗi account tự xem  
C. Export manual  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Centralized logging real-time với OpenSearch/Kibana.
</details>

---

### Question 55
Bạn cần “runbook as code” cho quy trình khắc phục sự cố tiêu chuẩn. Chọn?

A. Systems Manager Automation runbook lưu trong Git/CodeCommit, trigger từ EventBridge/Incident Manager  
B. Chạy tay  
C. IAM  
D. S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** IaC vận hành giúp kiểm soát thay đổi và audit.
</details>

---

### Question 56
Bạn muốn enforce thu thập logs CloudTrail cho mọi account mới. Giải pháp?

A. Organizations CT organization trail cho tất cả account/region, S3 centralized, KMS  
B. Tạo từng account riêng  
C. Không cần  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Org trail đảm bảo audit tập trung multi-account.
</details>

---

### Question 57
Phát hiện EC2 mở SSH ra Internet và tự động đóng. Thiết kế?

A. Config rule kiểm tra SG, EventBridge -> Lambda update SG và tạo OpsItem  
B. CloudFront  
C. NAT  
D. WAF

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Remediation tự động dựa compliance.
</details>

---

### Question 58
Bạn muốn alert khi chi phí tăng bất thường trong ngày. Công cụ?

A. CloudWatch Anomaly Detection cho Billing metrics (tài khoản consolidated) + Budgets alert  
B. WAF  
C. IAM  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kết hợp Budgets và anomaly detection trên metrics billing (nếu khả dụng).
</details>

---

### Question 59
SRE cần Postmortem tự động thu thập logs/metrics/traces liên quan sự cố. Gợi ý?

A. Incident Manager + Automation runbook tổng hợp artefacts (CW Logs/metrics, X-Ray) và đẩy S3  
B. Làm tay  
C. Không cần  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tự động hóa thu thập bằng runbook/SDK.
</details>

---

### Question 60
Kiến trúc event-driven cross-account, bạn muốn kiểm toán sự kiện. Làm gì?

A. EventBridge archive/replay + CloudTrail Lake cho audit  
B. Chỉ SNS  
C. Không thể  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Archive/replay và audit events là best practice.
</details>

---

### Question 61
Bạn muốn zero-trust shell vào EC2 private. Chọn?

A. SSM Session Manager với IAM/Logging/KMS  
B. Mở SSH 22  
C. Bastion public  
D. Client VPN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Session Manager không cần inbound port, kiểm soát IAM, lưu logs.
</details>

---

### Question 62
Giảm log chi phí cao ở CloudWatch Logs?

A. Đặt retention phù hợp, nén/stream sang S3 qua Firehose, dùng Logs Insights tiết kiệm truy vấn  
B. Giữ vô hạn  
C. Export thủ công  
D. Không log nữa

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Lưu dài hạn ở S3 rẻ hơn; chỉ giữ hot logs ở CW Logs.
</details>

---

### Question 63
Phát hiện drift cấu hình IaC (CloudFormation) so với thực tế?

A. CloudFormation drift detection + AWS Config rules  
B. WAF  
C. NAT  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kết hợp drift detection và Config để quản trị.
</details>

---

### Question 64
OpenTelemetry trên AWS?

A. Dùng ADOT (AWS Distro for OpenTelemetry) để thu thập metrics/traces/logs -> CloudWatch/X-Ray/OpenSearch  
B. Không hỗ trợ  
C. Chỉ X-Ray  
D. Chỉ logs

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** ADOT hỗ trợ chuẩn open telemetry.
</details>

---

### Question 65
SSM Fleet Manager?

A. Quản lý kết nối file, process, registry, console cho nhiều máy từ một nơi  
B. CDN  
C. DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Quản trị tập trung đội máy chủ.
</details>

---

### Question 66
OpsItem loại thông tin nào hữu ích?

A. Liên kết alarm, metric, log, runbook, timeline  
B. Chỉ text  
C. Chỉ số  
D. Không có

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** OpsItem tập trung tri thức sự cố.
</details>

---

### Question 67
Multi-account guardrails cho tagging?

A. AWS Organizations SCP + Tag Policies  
B. CloudTrail  
C. NAT  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tag Policies ép chuẩn tag keys/values.
</details>

---

### Question 68
Xây dựng SLO/SLI cho API?

A. Dùng CloudWatch metrics (latency, error rate), Alarms/Anomaly, Dashboard; X-Ray traces cho p95/p99  
B. Dùng IAM  
C. Dùng DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kết hợp metrics/traces cho SRE practices.
</details>

---

### Question 69
Tự động dọn dẹp tài nguyên idle?

A. Scheduled EventBridge + Lambda/SSM tìm tài nguyên idle -> tag/notify/stop/delete theo policy  
B. Không nên  
C. WAF  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Automation tiết kiệm chi phí vận hành.
</details>

---

### Question 70
OpenSearch dành cho observability?

A. Lưu/visualize logs, traces, metrics với OpenSearch dashboards  
B. DNS  
C. Backup  
D. IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Stack ELK/OS phổ biến cho observability.
</details>

---

### Question 71
Bạn cần chuẩn hóa baseline monitoring khi tạo môi trường mới. Giải pháp?

A. Service Catalog + CloudFormation StackSets + Control Tower lifecycle hook  
B. Làm tay  
C. Không cần  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tự động provision baseline theo chuẩn.
</details>

---

### Question 72
Alert fatigue do duplicate alerts multi-layer. Giải pháp?

A. Central alert routing (EventBridge/SNS), dedup, grouping, composite alarms  
B. Gửi hết email  
C. Tắt bớt  
D. Không cần

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Alert hygiene giúp vận hành bền vững.
</details>

---

### Question 73
Phòng chống xóa log audit?

A. S3 Object Lock (compliance mode) cho CloudTrail logs, bucket policy chặt chẽ, KMS key policy  
B. Cho phép write và delete  
C. Không cần  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** WORM cho audit logs là best practice.
</details>

---

### Question 74
Capture sự kiện thay đổi tham số cấu hình ứng dụng?

A. Parameter Store change trigger -> EventBridge -> Lambda notify  
B. WAF  
C. NAT  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Parameter Store phát sự kiện khi thay đổi (advanced params).
</details>

---

### Question 75
Theo dõi giới hạn dịch vụ gần đạt?

A. Service Quotas metrics + CloudWatch Alarms + Trusted Advisor checks  
B. Không cần  
C. NAT  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Chủ động nâng hạn mức trước khi bị chặn.
</details>

---

### Question 76
Tự động rollback khi deploy hỏng?

A. CloudWatch Alarm (error/latency) -> CodeDeploy Auto Rollback -> notify/Incident Manager  
B. Không rollback  
C. Làm tay  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kết nối alarm với pipeline để rollback tự động.
</details>

---

### Question 77
Quan sát Lambda cold start?

A. CloudWatch Duration p95/p99 + X-Ray init segment + Logs  
B. IAM  
C. DNS  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Theo dõi phân phối độ trễ và init time.
</details>

---

### Question 78
Giám sát độ trễ RDS query?

A. Performance Insights + Enhanced Monitoring + query logs  
B. IAM  
C. DNS  
D. S3

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kết hợp nhiều nguồn để tối ưu SQL.
</details>

---

### Question 79
Thiết lập maintenance window cho patching?

A. SSM Maintenance Windows + Patch Manager baseline  
B. CloudFront  
C. WAF  
D. Route 53

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Định thời gian bảo trì và áp patch an toàn.
</details>

---

### Question 80
Thiết kế vận hành chuẩn theo Well-Architected?

A. Thu thập logs/metrics/traces, định nghĩa SLO/SLI, tự động hóa remediation, runbook, game day  
B. Không cần  
C. Chỉ logs  
D. Chỉ metrics

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Đây là thực hành vận hành tốt theo WA.
</details>

---

