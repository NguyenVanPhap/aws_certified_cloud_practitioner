# Networking - Flashcards

---

## Q: VPC là gì?
**A:** Virtual Private Cloud - isolated network section trong AWS

---

## Q: Subnet là gì?
**A:** Network segment trong VPC, contained trong một AZ

---

## Q: Public vs Private subnet?
**A:** 
- **Public** = Route to Internet Gateway
- **Private** = No direct internet, dùng NAT Gateway cho outbound

---

## Q: Internet Gateway?
**A:** VPC ↔ Internet connectivity (two-way)

---

## Q: NAT Gateway?
**A:** Private subnet → Internet (outbound only)

---

## Q: CloudFront?
**A:** CDN - Content Delivery Network, distribute content globally với low latency

---

## Q: Edge Locations?
**A:** Locations gần users để cache content cho CloudFront

---

## Q: Route 53?
**A:** DNS service - translate domain names thành IP addresses

---

## Q: Security Groups vs NACLs?
**A:** 
- **Security Groups** = Instance-level, stateful
- **NACLs** = Subnet-level, stateless

---

## Q: API Gateway?
**A:** Service để create, publish, manage APIs

---

## Q: Direct Connect?
**A:** Dedicated network connection on-premises ↔ AWS

---

## Q: VPN?
**A:** Secure connection over public internet (Site-to-Site hoặc Client VPN)

---

## 🎯 Quick Reference

### VPC:
- **Subnets** = Public (IGW) / Private (NAT)
- **Security Groups** = Instance firewall
- **NACLs** = Subnet firewall

### CloudFront:
- **CDN** = Global distribution
- **Edge Locations** = Cache locations

### Route 53:
- **DNS** = Domain resolution
- **Routing policies** = Traffic routing

