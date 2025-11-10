# Well-Architected - Exam Questions V2

> 🧠 Mục tiêu: Thấu hiểu AWS Well-Architected Framework (6 trụ cột): Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, Sustainability.  
> 📦 Nội dung: 50 câu nền tảng + 30 câu khó (tổng 80 câu) dạng multiple-choice/multiple-response

---

## Phần A - Câu hỏi nền tảng (50 câu)

### Question 1
Well-Architected Framework gồm bao nhiêu trụ cột hiện tại?

A. 4  
B. 5  
C. 6  
D. 7

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** C  
**Giải thích:** 6 pillars: Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, Sustainability.
</details>

---

### Question 2
Operational Excellence tập trung vào?

A. Vận hành, quan sát, tự động hóa, cải tiến liên tục  
B. Bảo mật  
C. Hiệu năng  
D. Chi phí

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Pillar về vận hành hiệu quả, feedback loop.
</details>

---

### Question 3
Security pillar nhấn mạnh?

A. Bảo mật, nhận dạng, detection, bảo vệ hạ tầng/dữ liệu, response  
B. Chi phí  
C. Hiệu năng  
D. Vận hành

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Bao gồm IAM, detection, protection, data security, incident response.
</details>

---

### Question 4
Reliability pillar bao gồm?

A. Thiết kế fault tolerance, testing failure, recovery, scaling  
B. Chỉ bảo mật  
C. Chi phí  
D. CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Reliability đảm bảo hệ thống chịu lỗi và phục hồi.
</details>

---

### Question 5
Performance Efficiency pillar?

A. Chọn kiến trúc/tài nguyên tối ưu hiệu năng, test/giám sát liên tục  
B. Chi phí  
C. Bảo mật  
D. Vận hành

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Bao gồm lựa chọn dịch vụ phù hợp, scale elastic, serverless, caching.
</details>

---

### Question 6
Cost Optimization pillar?

A. Tránh chi tiêu không cần thiết, đo lường, lựa chọn mô hình giá phù hợp  
B. Bảo mật  
C. Hiệu năng  
D. Vận hành

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Đo lường, quyền sở hữu chi phí, tối ưu liên tục.
</details>

---

### Question 7
Sustainability pillar tập trung?

A. Giảm tác động môi trường, tối ưu sử dụng tài nguyên, hiệu quả năng lượng  
B. Bảo mật  
C. Chi phí  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu năng lượng, chọn region sạch, kiến trúc bền vững.
</details>

---

### Question 8
Well-Architected Review (WAR) là?

A. Đánh giá hệ thống theo câu hỏi chuẩn mỗi pillar, ghi lại rủi ro (HRI)  
B. Pen-test  
C. Kiểm thử hiệu năng  
D. Kiểm toán tài chính

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** WAR xác định High-Risk Issues và đề xuất cải tiến.
</details>

---

### Question 9
Design Principles của Operational Excellence gồm?

A. Perform operations as code, make frequent small changes, anticipate failure, learn from all operations  
B. Encrypt everything  
C. Use edge  
D. Use Spot

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Nguyên tắc nhấn mạnh tự động hóa và học hỏi.
</details>

---

### Question 10
Security design principles?

A. Implement a strong identity foundation, enable traceability, apply security at all layers, automate  
B. Use biggest instances  
C. Disable logging  
D. Public by default

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** IAM, monitoring, defense-in-depth, automation.
</details>

---

### Question 11
Reliability design principles?

A. Test recovery procedures, scale horizontally, stop guessing capacity, automate changes  
B. Encrypt at rest  
C. Use containers  
D. Use NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tập trung thiết kế chịu lỗi và phục hồi.
</details>

---

### Question 12
Performance design principles?

A. Democratize advanced technologies, go global in minutes, use serverless architectures, experiment often  
B. Encrypt at rest  
C. Use NAT  
D. Disable cache

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tận dụng dịch vụ managed/serverless, global, thử nghiệm.
</details>

---

### Question 13
Cost design principles?

A. Implement cloud financial management, adopt consumption model, measure, stop spending on undifferentiated heavy lifting  
B. Always on  
C. Hardcode  
D. Ignore cost

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Nguyên tắc FinOps trong WA.
</details>

---

### Question 14
Sustainability design principles?

A. Region selection, user behavior patterns, software/application design efficiency, data management, hardware utilization  
B. Always biggest  
C. Ignore energy  
D. Disable monitoring

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu hóa nhiều lớp để giảm tác động môi trường.
</details>

---

### Question 15
High-Risk Issue (HRI) là?

A. Phát hiện quan trọng từ WAR có thể gây rủi ro cao cho workload  
B. Bug nhẹ  
C. Chi phí nhỏ  
D. Không quan trọng

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** HRI cần ưu tiên khắc phục.
</details>

---

### Question 16
Operational Excellence metrics ví dụ?

A. MTTR/MTTD, change failure rate, deployment frequency  
B. CPU  
C. TTL  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Các chỉ số DevOps/SRE điển hình.
</details>

---

### Question 17
Security patterns?

A. Least privilege, separation of duties, rotation, encryption, logging  
B. Public  
C. Hardcode secrets  
D. No logging

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Mẫu bảo mật cốt lõi.
</details>

---

### Question 18
Reliability patterns?

A. Multi-AZ/Region, health checks, retries/backoff, circuit breaker  
B. Single-AZ  
C. No retries  
D. No health checks

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Mẫu chuẩn đảm bảo sẵn sàng cao.
</details>

---

### Question 19
Performance patterns?

A. Caching, async, event-driven, autoscaling, edge, right-sizing  
B. Single thread  
C. No cache  
D. No scaling

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Công thức phổ biến cho hiệu năng tốt.
</details>

---

### Question 20
Cost patterns?

A. Serverless, schedule off-hours, RI/SP/Spot, storage tiering, monitor & optimize  
B. Always on  
C. No monitoring  
D. No tags

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Thực hành tối ưu chi phí liên tục.
</details>

---

### Question 21
Sustainability patterns?

A. Use managed services, efficient code, scale-to-zero, data lifecycle, region carbon intensity  
B. Always biggest  
C. No telemetry  
D. Ignore user behavior

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu đa lớp giúp bền vững.
</details>

---

### Question 22
Shared Responsibility Model liên quan WAR?

A. Biết ranh giới: AWS vs khách hàng, WAR đánh giá phần của khách hàng  
B. AWS chịu hết  
C. Khách hàng chịu hết  
D. Không liên quan

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** AWS bảo mật đám mây; khách hàng bảo mật trong đám mây.
</details>

---

### Question 23
Well-Architected Tool (WAT) dùng để?

A. Thực hiện review, lưu trữ câu trả lời, phát hiện HRI, theo dõi cải tiến  
B. Billing  
C. CDN  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** WAT tích hợp trong console để review chuẩn.
</details>

---

### Question 24
Design trade-offs?

A. Cân bằng giữa pillars theo ngữ cảnh (vd. thêm cache tăng cost nhưng cải thiện hiệu năng)  
B. Không cần cân bằng  
C. Chỉ bảo mật  
D. Chỉ chi phí

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Quyết định kiến trúc là lựa chọn trade-off rõ ràng.
</details>

---

### Question 25
Threat modeling (Security) là?

A. Xác định mối đe dọa và kiểm soát giảm thiểu trong thiết kế  
B. Test hiệu năng  
C. Tối ưu chi phí  
D. Backup

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Nên thực hiện sớm và liên tục.
</details>

---

### Question 26
Game Day (Operational Excellence)?

A. Diễn tập sự cố để kiểm thử quy trình và khả năng phục hồi  
B. Bảo mật  
C. Chi phí  
D. CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Giúp cải tiến vận hành qua trải nghiệm thực tế.
</details>

---

### Question 27
Chaos engineering (Reliability)?

A. Cố ý tạo lỗi có kiểm soát để đo lường/ cải thiện độ tin cậy  
B. Bảo mật  
C. Chi phí  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tư duy “failure is normal”.
</details>

---

### Question 28
Performance benchmark/Load test?

A. Kiểm thử hiệu năng để xác nhận thiết kế và auto scaling  
B. Không cần  
C. Chỉ production  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Cần test thực tế để tối ưu.
</details>

---

### Question 29
Cost KPI?

A. Unit cost (chi phí/đơn vị giá trị), cost per request, cost per user  
B. CPU  
C. TTL  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** KPI chi phí gắn với giá trị kinh doanh.
</details>

---

### Question 30
Sustainability KPI?

A. Energy per transaction, carbon per request, resource utilization  
B. TTL  
C. CPU  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** KPI phản ánh tác động môi trường.
</details>

---

### Question 31
Security: Data classification giúp?

A. Áp dụng kiểm soát phù hợp theo mức độ nhạy cảm  
B. Không cần  
C. Chỉ mã hóa  
D. Chỉ IAM

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Cơ sở để thiết kế bảo vệ đúng mức.
</details>

---

### Question 32
Reliability: Backoff with jitter?

A. Retry theo backoff ngẫu nhiên để tránh thác lũ  
B. Retry tối đa liên tục  
C. Không retry  
D. Retry tức thì

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Jitter giảm contention khi sự cố.
</details>

---

### Question 33
Performance: Edge computing (CloudFront/Lambda@Edge) giúp?

A. Giảm latency bằng xử lý gần người dùng  
B. Tăng latency  
C. Không ảnh hưởng  
D. Chỉ bảo mật

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Edge phù hợp nội dung tĩnh/tùy biến nhẹ.
</details>

---

### Question 34
Cost: “Stop spending on undifferentiated heavy lifting” nghĩa là?

A. Dùng dịch vụ managed để tập trung vào giá trị kinh doanh  
B. Tự quản lý mọi thứ  
C. Không tối ưu  
D. Dùng on-prem

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Điều này giảm chi phí vận hành và rủi ro.
</details>

---

### Question 35
Sustainability: Region selection?

A. Chọn region có cường độ carbon thấp, nguồn năng lượng tái tạo cao khi phù hợp  
B. Bất kỳ  
C. Chỉ theo giá  
D. Không liên quan

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Lựa chọn region ảnh hưởng trực tiếp footprint.
</details>

---

### Question 36
Operational Excellence: Runbook/Playbook?

A. Tài liệu/Automation chuẩn hóa xử lý sự cố và tác vụ định kỳ  
B. Không cần  
C. Chỉ miệng  
D. DNS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Chuẩn hóa giúp giảm MTTR.
</details>

---

### Question 37
Security: Defense in depth?

A. Nhiều lớp bảo vệ (network, instance, app, data)  
B. Một lớp  
C. Không cần  
D. Chỉ mã hóa

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Nhiều lớp giảm rủi ro bị xuyên thủng.
</details>

---

### Question 38
Reliability: DR strategies?

A. Backup & Restore, Pilot Light, Warm Standby, Multi-Site Active/Active  
B. Chỉ backup  
C. Không DR  
D. Single-AZ

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Lựa chọn theo RTO/RPO.
</details>

---

### Question 39
Performance: Load testing KPI?

A. Throughput, latency percentiles (p95/p99), error rate, saturation  
B. Chỉ CPU  
C. Chỉ memory  
D. TTL

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** KPI phản ánh trải nghiệm người dùng.
</details>

---

### Question 40
Cost: Unit economics?

A. Gắn chi phí với đơn vị giá trị (một request, một người dùng, một đơn hàng)  
B. Tổng chi phí  
C. Không cần  
D. Chỉ EC2

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Giúp tối ưu theo giá trị kinh doanh.
</details>

---

### Question 41
Sustainability: User behavior optimization?

A. Giảm tải không cần thiết (caching client, hạn chế polling), format hiệu quả  
B. Không cần  
C. Chỉ server  
D. Chỉ DB

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu client giúp giảm footprint tổng thể.
</details>

---

### Question 42
Security: Encryption best practice?

A. Mã hóa at-rest và in-transit, quản trị key an toàn, rotate  
B. Không cần  
C. Chỉ at-rest  
D. Chỉ in-transit

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kết hợp cả hai và key management chặt chẽ.
</details>

---

### Question 43
Reliability: Health checks & graceful degradation?

A. Phát hiện sớm lỗi và degrade chức năng để hệ thống vẫn phục vụ cơ bản  
B. Tắt hệ thống  
C. Không degrade  
D. Không health

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tránh gián đoạn hoàn toàn khi lỗi một phần.
</details>

---

### Question 44
Performance: Choice of database?

A. Chọn DB theo workload (relational, key-value, graph, time-series, analytics)  
B. Một DB cho tất cả  
C. Luôn relational  
D. Luôn NoSQL

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Polyglot persistence nâng cao hiệu năng/đơn giản thiết kế.
</details>

---

### Question 45
Cost: Start/Stop non-production?

A. Tự động dừng môi trường dev/test off-hours để tiết kiệm  
B. Luôn bật  
C. Không cần  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Lịch tắt mở giúp tiết kiệm lớn.
</details>

---

### Question 46
Sustainability: Data lifecycle?

A. Chính sách retention, tiering, xóa dữ liệu không cần thiết  
B. Lưu vô hạn  
C. Không nén  
D. Không tiering

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Giảm footprint lưu trữ/chi phí.
</details>

---

### Question 47
Operational Excellence: Observability?

A. Logs, metrics, traces, synthetics, RUM  
B. Chỉ logs  
C. Chỉ metrics  
D. Chỉ traces

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Quan sát đầy đủ giúp phản ứng nhanh và tối ưu.
</details>

---

### Question 48
Security: Zero Trust?

A. Không tin cậy mặc định, xác thực/ủy quyền liên tục, least privilege, network segmentation  
B. Tin cậy tất cả  
C. Chỉ mật khẩu tĩnh  
D. Không log

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Zero Trust là xu hướng bảo mật hiện đại.
</details>

---

### Question 49
Reliability: SLO/SLI/SLA?

A. SLI đo, SLO mục tiêu nội bộ, SLA cam kết với khách hàng  
B. Ngược lại  
C. Giống nhau  
D. Không liên quan

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Định nghĩa chuẩn trong SRE/WA.
</details>

---

### Question 50
Performance: Caching layers?

A. Client cache, CDN, application cache, database cache  
B. Chỉ CDN  
C. Chỉ DB  
D. Không cache

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Multi-layer cache cải thiện hiệu năng và chi phí.
</details>

---

## Phần B - Câu hỏi khó (30 câu)

### Question 51
Bạn có ứng dụng đa region active-active. Yêu cầu latency thấp, conflict resolution. Lưu ý pillars nào?

A. Reliability, Performance, Cost, Security  
B. Chỉ Reliability  
C. Chỉ Performance  
D. Chỉ Cost

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Multi-region liên quan nhiều trụ cột, cần cân bằng trade-offs.
</details>

---

### Question 52
Thiết kế DR Pilot Light: chọn đáp án đúng.

A. Giữ dữ liệu và core services tối thiểu ở region DR, khi sự cố scale lên nhanh chóng  
B. Luôn active-active  
C. Không lưu gì  
D. Cold backup hoàn toàn

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Pilot Light cân bằng chi phí và RTO.
</details>

---

### Question 53
Bạn muốn giảm carbon footprint cho workload batch hàng đêm.

A. Chạy ở region carbon thấp, Spot, tối ưu thời lượng, scale-to-zero khi xong  
B. Luôn On-Demand  
C. Không đo  
D. Bật tối đa

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Sustainability thực tế qua region & tối ưu compute.
</details>

---

### Question 54
Hệ thống có spike traffic bất thường, gây overload. Giải pháp theo WA?

A. Autoscaling phản ứng nhanh, queue đệm (SQS), rate limiting, circuit breaker, caching  
B. Tăng cố định  
C. Bỏ qua  
D. Không cache

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kết hợp pattern cho ổn định.
</details>

---

### Question 55
Secrets rò rỉ trong repo. Theo Security pillar, xử lý?

A. Rotate ngay (Secrets Manager), kiểm tra logs, quét phạm vi ảnh hưởng, cải tiến quy trình  
B. Bỏ qua  
C. Đổi region  
D. Không cần

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Quy trình IR chuẩn cho secrets.
</details>

---

### Question 56
Microservices latency cao do chatty calls. Theo Performance, hướng cải thiện?

A. Batching, async, caching, co-location, GraphQL/gateway aggregation, service mesh policy  
B. Tăng CPU  
C. Thêm NAT  
D. Không thể

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Giảm số round-trips và overhead.
</details>

---

### Question 57
Chi phí tăng do logging quá chi tiết. Theo Cost, làm gì?

A. Điều chỉnh sampling/retention, chuyển lâu dài sang S3, Logs Insights chọn lọc  
B. Giữ nguyên  
C. Tăng thêm  
D. Xóa hết

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu logging cân bằng quan sát/chi phí.
</details>

---

### Question 58
Reliability: thử nghiệm failover định kỳ thế nào?

A. Game Day + automation, runbook, đo RTO/RPO thực tế  
B. Chỉ documentation  
C. Không test  
D. Log thôi

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Test thực chiến mới tin cậy.
</details>

---

### Question 59
Security: multi-account strategy giúp?

A. Cô lập blast radius, tách môi trường (prod/non-prod), áp guardrail theo OU  
B. Không cần  
C. Một account cho tất cả  
D. Chỉ billing

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Multi-account là best practice cho bảo mật/quản trị.
</details>

---

### Question 60
Performance: workload CPU-bound trên EC2. Tối ưu?

A. Chọn instance C-family, ENA/EFA khi cần, tối ưu code, autoscaling  
B. Chọn T-family  
C. Chọn R-family  
D. Không cần

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Chọn instance phù hợp workload.
</details>

---

### Question 61
Cost: kiến trúc analytics tiết kiệm?

A. Data lake S3 + Athena/Glue + Redshift Serverless, tách compute/storage  
B. Cluster always-on  
C. Không lake  
D. Chỉ RDS

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Lake-first tối ưu chi phí/linh hoạt.
</details>

---

### Question 62
Sustainability: dữ liệu hình ảnh/video lớn, ít truy cập.

A. Tiering S3 (IA/Glacier), transcode hiệu quả, CDN cache  
B. Lưu Standard suốt  
C. Không nén  
D. Không CDN

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Giảm footprint lưu trữ/bandwidth.
</details>

---

### Question 63
Operational Excellence: “Operations as code” ví dụ?

A. IaC (CloudFormation/Terraform), SSM Automation, GitOps  
B. Thao tác tay  
C. Shell rời rạc  
D. Không quản lý

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tự động hóa và kiểm soát phiên bản.
</details>

---

### Question 64
Security: Detect –> Respond?

A. CloudTrail/Config/GuardDuty/Macie -> EventBridge -> Lambda/SSM/IR automation  
B. Không cần  
C. Thủ công  
D. Chỉ logs

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Chuỗi phát hiện-ứng phó tự động.
</details>

---

### Question 65
Reliability: Throttling downstream service?

A. Queue buffer, retry with jitter, rate limit, circuit breaker  
B. Gửi tối đa  
C. Không buffer  
D. Không retry

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Pattern chống backpressure.
</details>

---

### Question 66
Performance: Database hot key?

A. Sharding, caching, write spreading, precompute  
B. Tăng một node  
C. Không thể  
D. NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Thiết kế phân tán key và dùng cache.
</details>

---

### Question 67
Cost: Không dùng đến tài nguyên ban đêm. Làm gì?

A. Schedule dừng bằng EventBridge/SSM/Lambda  
B. Để nguyên  
C. Tăng size  
D. Không tag

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Lịch hóa tiết kiệm chi phí đáng kể.
</details>

---

### Question 68
Sustainability: Serverless có lợi gì?

A. Scale theo nhu cầu, ít idle -> hiệu quả năng lượng tốt hơn  
B. Luôn chạy  
C. Không lợi  
D. Chỉ chi phí

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Serverless tối ưu utilization.
</details>

---

### Question 69
Operational Excellence: Post-incident review tốt?

A. Không đổ lỗi, tập trung cải tiến hệ thống/quy trình, action items rõ ràng  
B. Đổ lỗi cá nhân  
C. Bỏ qua  
D. Không ghi chép

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Văn hóa học hỏi cải thiện bền vững.
</details>

---

### Question 70
Security: Multi-factor authentication (MFA) cho tài khoản root?

A. Bắt buộc nên bật và tránh dùng root cho hoạt động hằng ngày  
B. Không cần  
C. Chỉ user thường  
D. Không liên quan

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Root cần bảo vệ cao nhất.
</details>

---

### Question 71
Reliability: Test capacity?

A. Load test, stress test, game day để thấy ngưỡng và hành vi khi quá tải  
B. Không test  
C. Chỉ đọc tài liệu  
D. Đợi sự cố

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Kiểm thử giúp lên kế hoạch scaling.
</details>

---

### Question 72
Performance: Optimize serialization?

A. Dùng format hiệu quả (ProtoBuf/Avro/Parquet), nén hợp lý  
B. JSON không nén luôn  
C. Không quan tâm  
D. Không cache

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Format ảnh hưởng latency/bandwidth mạnh.
</details>

---

### Question 73
Cost: Kiểm soát chi phí NAT Gateway enterprise?

A. Centralized egress VPC, PrivateLink, endpoints, audit lưu lượng, tối ưu route  
B. Tăng NAT  
C. Không cần  
D. Không log

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Mẫu egress chuẩn giảm chi phí đáng kể.
</details>

---

### Question 74
Sustainability: Ứng dụng streaming?

A. Batch processing khi phù hợp, windowing hợp lý, filter sớm, edge processing  
B. Push mọi dữ liệu  
C. Không filter  
D. Không window

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Giảm compute/bandwidth thừa.
</details>

---

### Question 75
Operational Excellence: Change management?

A. Canary/blue-green, rollback tự động, approval, IaC pipelines  
B. Deploy tay  
C. Big-bang  
D. Không rollback

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Quản trị thay đổi hiện đại giảm rủi ro.
</details>

---

### Question 76
Security: DLP cho S3?

A. Macie + S3 Object Lock + Access Analyzer + Bucket policy chặt  
B. Không cần  
C. Public default  
D. Không log

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Bộ công cụ bảo vệ dữ liệu nhạy cảm.
</details>

---

### Question 77
Reliability: Latency outlier ở 1 AZ?

A. Enable cross-zone LB, health checks, route away, investigate networking/placement  
B. Tắt LB  
C. Fix tay  
D. Bỏ qua

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** LB và health giúp cô lập AZ xấu.
</details>

---

### Question 78
Performance: Data locality?

A. Đặt compute gần dữ liệu, tránh chuyển dữ liệu không cần  
B. Di chuyển dữ liệu liên tục  
C. Không quan tâm  
D. Dùng NAT

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Locality giảm latency/chi phí.
</details>

---

### Question 79
Cost: KPI “cost per million requests” tăng.

A. Điều chỉnh caching, compression, compute sizing, xem xét pricing model (SP/RI)  
B. Bỏ qua  
C. Không đo  
D. Tăng tài nguyên

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Tối ưu theo đơn vị giá trị.
</details>

---

### Question 80
Sustainability: Culture of sustainability?

A. Mục tiêu rõ ràng, đo lường, báo cáo, tối ưu liên tục, đào tạo đội ngũ  
B. Không cần  
C. Chỉ 1 lần  
D. Không đo

<details>
<summary><strong>Hiển thị đáp án</strong></summary>

**Đáp án:** A  
**Giải thích:** Bền vững là hành trình văn hóa/kinh doanh.
</details>

---

