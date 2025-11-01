# Database Services - Exam Style Questions

---

## Question 1
What is Amazon RDS?

A. A compute service  
B. A managed relational database service  
C. A storage service  
D. A networking service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** RDS = Relational Database Service = managed relational databases. Support MySQL, PostgreSQL, MariaDB, Oracle, SQL Server. AWS quản lý patching, backups.

**Exam Tip:** RDS = Managed SQL databases.
</details>

---

## Question 2
What is Amazon DynamoDB?

A. A relational database  
B. A NoSQL database service  
C. A data warehouse  
D. A cache service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** DynamoDB = fully managed NoSQL database. Serverless, auto-scaling, single-digit millisecond latency. Key-value và document database.

**Exam Tip:** DynamoDB = Managed NoSQL, serverless.
</details>

---

## Question 3
What is Amazon Redshift?

A. A relational database  
B. A NoSQL database  
C. A data warehouse service  
D. A cache service

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Redshift = fully managed data warehouse. Dùng cho analytics, business intelligence. Petabyte-scale, columnar storage.

**Exam Tip:** Redshift = Data warehouse, analytics.
</details>

---

## Question 4
Which database service is serverless and automatically scales?

A. RDS  
B. DynamoDB  
C. Redshift  
D. ElastiCache

<details>
<summary><strong>Answer: B - DynamoDB</strong></summary>

**Explanation:** DynamoDB = serverless, automatically scales. No servers to manage, pay for throughput. RDS và Redshift require instance management.

**Exam Tip:** DynamoDB = Serverless, auto-scaling. RDS/Redshift = Managed instances.
</details>

---

## Question 5
What is ElastiCache used for?

A. Long-term storage  
B. In-memory caching to improve application performance  
C. Database backups  
D. Data archiving

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** ElastiCache = in-memory caching (Redis hoặc Memcached). Improve application performance bằng cách cache frequently accessed data. Giảm database load.

**Exam Tip:** ElastiCache = In-memory caching, improve performance.
</details>

---

## Question 6
Which RDS feature automatically creates backups?

A. Manual backups  
B. Automated backups  
C. Snapshot backups  
D. Archive backups

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** RDS Automated Backups = automatically create daily backups và transaction logs. Retention 1-35 days. Point-in-time recovery.

**Exam Tip:** RDS = Automated daily backups, point-in-time recovery.
</details>

---

## Question 7
What is the difference between RDS and DynamoDB?

A. They are the same  
B. RDS is relational, DynamoDB is NoSQL  
C. DynamoDB is relational, RDS is NoSQL  
D. RDS is for analytics, DynamoDB is for transactions

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** RDS = relational databases (SQL, structured data). DynamoDB = NoSQL (key-value, document, flexible schema). Chọn dựa trên data structure.

**Exam Tip:** RDS = SQL | DynamoDB = NoSQL.
</details>

---

## Question 8
Which database service is best for analytics and data warehousing?

A. RDS  
B. DynamoDB  
C. Redshift  
D. ElastiCache

<details>
<summary><strong>Answer: C - Redshift</strong></summary>

**Explanation:** Redshift = designed cho analytics và data warehousing. Columnar storage, optimized cho queries trên large datasets.

**Exam Tip:** Analytics = Redshift. Transactions = RDS/DynamoDB.
</details>

---

## Question 9
Which of the following are RDS features? (Select TWO)

A. Automated backups  
B. Multi-AZ deployment for high availability  
C. Serverless architecture  
D. Automatic scaling without configuration  
E. In-memory caching

<details>
<summary><strong>Answer: A, B</strong></summary>

**Explanation:** RDS features: Automated backups, Multi-AZ (high availability). C, D mô tả DynamoDB (serverless, auto-scaling). E mô tả ElastiCache.

**Exam Tip:** RDS = Automated backups, Multi-AZ. DynamoDB = Serverless, auto-scaling.
</details>

---

## Question 10
What is Amazon Aurora?

A. A NoSQL database  
B. An AWS-optimized MySQL/PostgreSQL-compatible database  
C. A data warehouse  
D. A cache service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Aurora = AWS-optimized relational database, compatible với MySQL và PostgreSQL. Higher performance, automated backups, Multi-AZ.

**Exam Tip:** Aurora = AWS-optimized MySQL/PostgreSQL, high performance.
</details>

---

## 📊 Exam Simulation

Làm 10 câu trong **15 phút**:
- **9-10 đúng**: ✅ Excellent!
- **7-8 đúng**: ✅ Good!
- **Dưới 7 đúng**: 📚 Review

---

## 💡 Exam Tips

1. **RDS** = Managed SQL databases, automated backups, Multi-AZ
2. **DynamoDB** = Managed NoSQL, serverless, auto-scaling
3. **Redshift** = Data warehouse, analytics, columnar storage
4. **ElastiCache** = In-memory caching (Redis/Memcached)
5. **Aurora** = AWS-optimized MySQL/PostgreSQL

---

## 🔄 Review Schedule

- Lần 1: Sau notes
- Lần 2: Sau 2 ngày
- Lần 3: Sau 5 ngày
- Lần 4: 1 tuần trước thi

Mục tiêu: 100%!

