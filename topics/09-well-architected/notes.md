# Well-Architected Framework - Tóm tắt kiến thức

## 1. Well-Architected Framework

### Khái niệm
Well-Architected Framework = best practices và guidelines để build secure, reliable, efficient applications trên AWS.

---

## 2. Five Pillars

### 1. Operational Excellence
- **Focus**: Operations và processes
- **Best practices**: 
  - Automate changes
  - Learn from failures
  - Frequently refine procedures

### 2. Security
- **Focus**: Protect information và systems
- **Best practices**:
  - Implement strong identity foundation (IAM)
  - Apply security at all layers
  - Enable traceability (CloudTrail, CloudWatch)
  - Encrypt data at rest và in transit

### 3. Reliability
- **Focus**: Recover from failures, meet demand
- **Best practices**:
  - Test recovery procedures
  - Automatically recover from failures
  - Scale horizontally
  - Stop guessing capacity

### 4. Performance Efficiency
- **Focus**: Use resources efficiently
- **Best practices**:
  - Democratize advanced technologies
  - Go global in minutes
  - Use serverless architectures
  - Experiment more often

### 5. Cost Optimization
- **Focus**: Minimize costs
- **Best practices**:
  - Implement Cloud Financial Management
  - Adopt consumption model
  - Measure overall efficiency
  - Eliminate unneeded costs

---

## 3. Key Concepts

### High Availability:
- System remains operational với minimal downtime
- Achieved through redundancy, multiple AZs

### Fault Tolerance:
- Continue operating khi có component failures
- Zero downtime failures
- Redundancy at every level

### Scalability:
- Handle increasing load
- Horizontal scaling (add more instances)
- Vertical scaling (increase instance size)

### Elasticity:
- Automatically scale based on demand
- Auto Scaling, Lambda

---

## 📚 Design Principles

1. **Stop guessing capacity** - Auto Scaling
2. **Test systems at production scale**
3. **Automate to make architectural experimentation easier**
4. **Allow for evolutionary architectures**
5. **Drive architectures using data**
6. **Improve through game days** (chaos engineering)

---

## ✅ Checklist

- [ ] Hiểu 5 pillars
- [ ] Biết best practices cho từng pillar
- [ ] Hiểu High availability vs Fault tolerance
- [ ] Biết design principles

