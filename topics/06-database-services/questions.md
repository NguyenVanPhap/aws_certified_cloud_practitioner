# Database Services - Practice Questions

---

## Question 1
**What is Amazon RDS?**

A. A compute service  
B. A managed relational database service  
C. A storage service  
D. A networking service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** RDS (Relational Database Service) = managed relational database service. Support MySQL, PostgreSQL, MariaDB, Oracle, SQL Server. AWS quản lý patching, backups, monitoring.

**Key Concept:** RDS = Managed relational databases
</details>

---

## Question 2
**What is Amazon DynamoDB?**

A. A relational database  
B. A NoSQL database service  
C. A data warehouse  
D. A cache service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** DynamoDB = fully managed NoSQL database service. Serverless, auto-scaling, single-digit millisecond latency. Key-value và document database.

**Key Concept:** DynamoDB = Managed NoSQL database
</details>

---

## Question 3
**What is Amazon Redshift?**

A. A relational database  
B. A NoSQL database  
C. A data warehouse service  
D. A cache service

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Redshift = fully managed data warehouse service. Dùng cho analytics, business intelligence. Petabyte-scale data, columnar storage.

**Key Concept:** Redshift = Data warehouse for analytics
</details>

---

## Question 4
**Which database service is serverless and automatically scales?**

A. RDS  
B. DynamoDB  
C. Redshift  
D. ElastiCache

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** DynamoDB = serverless, automatically scales. No servers to manage, pay for throughput. RDS và Redshift require instance management.

**Key Concept:** DynamoDB = Serverless, auto-scaling
</details>

---

## Question 5
**What is ElastiCache used for?**

A. Long-term storage  
B. In-memory caching to improve application performance  
C. Database backups  
D. Data archiving

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** ElastiCache = in-memory caching service (Redis hoặc Memcached). Improve application performance bằng cách cache frequently accessed data. Giảm database load.

**Key Concept:** ElastiCache = In-memory caching
</details>

---

## Question 6
**Which RDS feature automatically creates backups?**

A. Manual backups  
B. Automated backups  
C. Snapshot backups  
D. Archive backups

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** RDS Automated Backups = automatically create daily backups và transaction logs. Retention period 1-35 days. Point-in-time recovery.

**Key Concept:** RDS = Automated daily backups
</details>

---

## Question 7
**What is the difference between RDS and DynamoDB?**

A. They are the same  
B. RDS is relational, DynamoDB is NoSQL  
C. DynamoDB is relational, RDS is NoSQL  
D. RDS is for analytics, DynamoDB is for transactions

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** RDS = relational databases (SQL, structured data). DynamoDB = NoSQL (key-value, document, flexible schema). Chọn dựa trên data structure và use case.

**Key Concept:** RDS = SQL | DynamoDB = NoSQL
</details>

---

## Question 8
**Which database service is best for analytics and data warehousing?**

A. RDS  
B. DynamoDB  
C. Redshift  
D. ElastiCache

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Redshift = designed cho analytics và data warehousing. Columnar storage, optimized cho queries trên large datasets. RDS và DynamoDB = transactional workloads.

**Key Concept:** Redshift = Analytics và data warehousing
</details>

---

## 📊 Tự đánh giá

- **6-8 câu đúng**: ✅ Excellent!
- **4-5 câu đúng**: ✅ Good!
- **Dưới 4 câu**: 📚 Review notes.md

---

## 💡 Tips

1. RDS = Managed relational (SQL)
2. DynamoDB = Managed NoSQL, serverless
3. Redshift = Data warehouse, analytics
4. ElastiCache = In-memory caching

