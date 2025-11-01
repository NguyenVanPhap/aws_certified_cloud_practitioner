# Database Services - Tóm tắt kiến thức

## 1. Amazon RDS (Relational Database Service)

### Khái niệm
RDS = Managed relational database service. AWS quản lý patching, backups, monitoring, scaling.

### Supported Engines:
- MySQL
- PostgreSQL
- MariaDB
- Oracle
- SQL Server
- Aurora (AWS-optimized MySQL/PostgreSQL)

### Features:
- **Automated backups**: Daily backups, point-in-time recovery
- **Multi-AZ**: High availability across AZs
- **Read replicas**: Scale read performance
- **Encryption**: At rest và in transit

---

## 2. Amazon DynamoDB

### Khái niệm
DynamoDB = Fully managed NoSQL database service.

### Đặc điểm:
- **Serverless**: No servers to manage
- **Auto-scaling**: Automatically scale throughput
- **Low latency**: Single-digit millisecond
- **Key-value và document database**
- **Pay for throughput**: Provisioned hoặc On-demand

---

## 3. Amazon Redshift

### Khái niệm
Redshift = Fully managed data warehouse service.

### Đặc điểm:
- **Data warehouse**: Analytics và BI
- **Columnar storage**: Optimized cho analytics queries
- **Petabyte-scale**: Large datasets
- **SQL-based**: Familiar SQL interface

---

## 4. Amazon ElastiCache

### Khái niệm
ElastiCache = In-memory caching service.

### Engines:
- **Redis**: Advanced data structures
- **Memcached**: Simple caching

### Use cases:
- Improve application performance
- Reduce database load
- Session stores
- Real-time analytics

---

## 📚 Key Concepts

- **RDS** = Managed SQL databases
- **DynamoDB** = Managed NoSQL, serverless
- **Redshift** = Data warehouse, analytics
- **ElastiCache** = In-memory caching

---

## ✅ Checklist

- [ ] Hiểu RDS và managed services
- [ ] Biết DynamoDB và NoSQL
- [ ] Hiểu Redshift và analytics
- [ ] Biết ElastiCache và caching

