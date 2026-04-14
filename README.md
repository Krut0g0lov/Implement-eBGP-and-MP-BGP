
🌐 Cisco Lab: BGP & MP-BGP Implementation (ENCOR)
🚀 Combined lab based on Cisco NetAcad — eBGP + MP-BGP (IPv4 & IPv6)
This project demonstrates the implementation of eBGP and Multiprotocol BGP (MP-BGP) in a multi-AS environment, simulating a real-world service provider and customer topology.

📖 Description
In this lab, I combined two Cisco ENCOR labs into a single scenario to build a scalable, dual-stack BGP network.
The topology includes:
multiple Autonomous Systems (AS)
redundant links between routers
IPv4 and IPv6 routing
route summarization and policy control

💡 The goal was not just configuration, but understanding how BGP behaves in real networks.
🧠 Technologies Used
eBGP (External BGP) — inter-AS routing
MP-BGP — multiprotocol support (IPv4 + IPv6)
Route Aggregation — aggregate-address
BGP Attributes — Weight, Local Preference, AS-PATH
Dual-Stack Networking — IPv4 & IPv6
Loopback Interfaces — route advertisement
Null0 Routing — loop prevention

🌍 Topology
The lab simulates a realistic provider environment:
🟢 Customer AS 1000 (R1)
🔵 ISP AS 500 (R2)
🟠 ISP AS 300 (R3)
Key design elements:
Redundant links between R1 and R3
eBGP peering between all AS
Loopbacks used for network advertisement
IPv6 enabled via MP-BGP

⚙️ Key Features
🔹 eBGP Peering
Established between all routers
Exchange of IPv4 routes across AS boundaries

🔹 MP-BGP (Multiprotocol BGP)
router bgp XXXX
 address-family ipv4 unicast
 address-family ipv6 unicast
✔ Enables:
multiple routing tables over a single BGP process
simultaneous IPv4 and IPv6 route exchange

🔹 Route Summarization
aggregate-address 192.168.X.0 255.255.255.0 summary-only
reduces routing table size
suppresses specific prefixes
improves scalability
