# 🌐 Cisco Lab: BGP & MP-BGP Implementation (ENCOR)

> 🚀 Combined Cisco NetAcad Lab — eBGP + MP-BGP (IPv4 & IPv6)

This project demonstrates the implementation of **eBGP and Multiprotocol BGP (MP-BGP)** in a multi-AS environment, simulating a real-world **service provider ↔ customer topology**.

---

## 📖 Description

In this lab, I combined two Cisco ENCOR labs into a single scenario to build a **scalable dual-stack BGP network**.

The topology includes:
- Multiple Autonomous Systems (AS)
- Redundant inter-router links
- IPv4 & IPv6 routing (MP-BGP)
- Route summarization and policy control

💡 The goal was not just configuration, but understanding how **BGP behaves in real-world networks**.

---

## 🧠 Technologies Used

- **eBGP (External BGP)** — inter-AS routing  
- **MP-BGP** — multiprotocol support (IPv4 + IPv6)  
- **Route Aggregation** — `aggregate-address`  
- **BGP Attributes** — Weight, Local Preference, AS-PATH  
- **Dual-Stack Networking** — IPv4 & IPv6  
- **Loopback Interfaces** — route advertisement  
- **Null0 Routing** — loop prevention  

---

## 🌍 Topology

📌 The lab simulates a realistic provider environment:

- 🟢 **Customer — AS 1000 (R1)**  
- 🔵 **ISP — AS 500 (R2)**  
- 🟠 **ISP — AS 300 (R3)**  

### Key Design Elements:
- Redundant links between R1 and R3  
- eBGP peering between all AS  
- Loopbacks used for route advertisement  
- IPv6 enabled via MP-BGP  

---

## ⚙️ Key Features

### 🔹 eBGP Peering
- Established between all routers  
- Exchange of IPv4 routes across AS boundaries  

---

### 🔹 MP-BGP (Multiprotocol BGP)
