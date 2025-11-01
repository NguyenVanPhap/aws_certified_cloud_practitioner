# Well-Architected Framework - Exam Style Questions

---

## Question 1
What is the AWS Well-Architected Framework?

A. A compute service  
B. A set of best practices and guidelines for building secure, high-performing applications  
C. A storage service  
D. A database service

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Well-Architected Framework = best practices và guidelines để build secure, reliable, efficient applications trên AWS. 5 pillars.

**Exam Tip:** Well-Architected = Best practices, 5 pillars.
</details>

---

## Question 2
What are the five pillars of the Well-Architected Framework?

A. Compute, Storage, Database, Networking, Security  
B. Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization  
C. Availability, Scalability, Durability, Consistency, Partition Tolerance  
D. Development, Testing, Staging, Production, Disaster Recovery

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** 5 pillars: Operational Excellence (operations), Security (protection), Reliability (fault tolerance), Performance Efficiency (resource efficiency), Cost Optimization (minimize costs).

**Exam Tip:** 5 Pillars = OSRPC (Operational, Security, Reliability, Performance, Cost).
</details>

---

## Question 3
Which pillar focuses on protecting information and systems?

A. Operational Excellence  
B. Security  
C. Reliability  
D. Performance Efficiency

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Security pillar = protect information, systems, assets. IAM, encryption, monitoring, incident response.

**Exam Tip:** Security = Protection.
</details>

---

## Question 4
Which pillar focuses on the ability to recover from failures?

A. Operational Excellence  
B. Security  
C. Reliability  
D. Cost Optimization

<details>
<summary><strong>Answer: C</strong></summary>

**Explanation:** Reliability = ability to recover từ failures, meet demand, mitigate disruptions. High availability, fault tolerance, disaster recovery.

**Exam Tip:** Reliability = Recover from failures.
</details>

---

## Question 5
What does "high availability" mean?

A. High speed  
B. System remains operational with minimal downtime during failures  
C. High cost  
D. High storage capacity

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** High availability = system remains operational với minimal downtime khi có failures. Achieved through redundancy, multiple AZs, health checks.

**Exam Tip:** High availability = Minimal downtime during failures.
</details>

---

## Question 6
What is fault tolerance?

A. The ability to prevent failures  
B. The ability to continue operating when components fail  
C. The ability to reduce costs  
D. The ability to scale automatically

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** Fault tolerance = ability to continue operating khi có component failures. Zero downtime failures, achieved through redundancy.

**Exam Tip:** Fault tolerance = Continue operating despite failures (zero downtime).
</details>

---

## Question 7
Which pillar focuses on minimizing costs while maintaining system performance?

A. Operational Excellence  
B. Security  
C. Reliability  
D. Cost Optimization

<details>
<summary><strong>Answer: D</strong></summary>

**Explanation:** Cost Optimization = minimize costs while maintaining performance. Right-sizing resources, eliminate waste, use appropriate pricing models.

**Exam Tip:** Cost Optimization = Minimize costs.
</details>

---

## Question 8
Which pillar focuses on operations and processes?

A. Operational Excellence  
B. Security  
C. Reliability  
D. Performance Efficiency

<details>
<summary><strong>Answer: A</strong></summary>

**Explanation:** Operational Excellence = operations và processes. Automate changes, learn from failures, frequently refine procedures.

**Exam Tip:** Operational Excellence = Operations và processes.
</details>

---

## Question 9
What is the difference between high availability and fault tolerance?

A. They are the same  
B. High availability means minimal downtime, fault tolerance means zero downtime  
C. High availability is for databases, fault tolerance is for applications  
D. High availability costs more

<details>
<summary><strong>Answer: B</strong></summary>

**Explanation:** High availability = minimal downtime (99.9%, 99.99% uptime). Fault tolerance = zero downtime (system continues operating during failures). Both achieved through redundancy.

**Exam Tip:** High availability = Minimal downtime | Fault tolerance = Zero downtime.
</details>

---

## Question 10
Which of the following are design principles of the Well-Architected Framework? (Select THREE)

A. Stop guessing capacity  
B. Test systems at production scale  
C. Use dedicated hardware  
D. Automate to make architectural experimentation easier  
E. Always use on-premises solutions

<details>
<summary><strong>Answer: A, B, D</strong></summary>

**Explanation:** Design principles: Stop guessing capacity (use Auto Scaling), Test at production scale, Automate experimentation. C, E không phải best practices.

**Exam Tip:** Design principles: Auto Scaling, Test at scale, Automate, Evolutionary architectures.
</details>

---

## 📊 Exam Simulation

Làm 10 câu trong **15 phút**:
- **9-10 đúng**: ✅ Excellent!
- **7-8 đúng**: ✅ Good!
- **Dưới 7 đúng**: 📚 Review

---

## 💡 Exam Tips

1. **5 Pillars**: Operational Excellence, Security, Reliability, Performance, Cost
2. **High availability** = Minimal downtime
3. **Fault tolerance** = Zero downtime
4. **Design principles**: Auto Scaling, test at scale, automate
5. **Best practices** cho từng pillar

---

## 🔄 Review Schedule

- Lần 1: Sau notes
- Lần 2: Sau 2 ngày
- Lần 3: Sau 5 ngày
- Lần 4: 1 tuần trước thi

Mục tiêu: 100%!

