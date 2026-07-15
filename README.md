# Company / Business System Network Design

**Course:** Network Routing and Switching  
**Student:** Sumaira Safeer (FA22-BCE-019)  
**Campus:** COMSATS University Islamabad, Attock Campus

---

## Overview
This project presents a complete **hierarchical, redundant network design** for a 600-user trading floor support center relocating to a new three-floor building. The design was implemented and fully tested in **Cisco Packet Tracer**.

Key features include:
- Dual edge routers with dual-homed ISP connectivity (full redundancy)
- Two multilayer switches performing core switching + inter-VLAN routing
- Per-department VLANs, subnets, and dedicated wireless networks
- OSPF dynamic routing with automatic failover
- DHCP server with relay, static addressing in server room
- Security: SSH, port-security (Finance & Accounts), PAT + ACL

---

## Network Topology
![Full Network Topology](screenshots/topology-full.png)
**Hierarchical Design (Core-Distribution-Access)** with redundancy at every layer.

---

## Key Technologies & Configurations
- **Routing:** OSPF (Area 0), default routes with floating statics for ISP failover
- **Switching:** 802.1Q trunks, VLANs 10, 20, 30, 40, 50, 60
- **IP Addressing:** 172.16.1.0/16 private scheme with VLSM
- **Services:** DHCP relay, DNS, Email server (static)
- **Security:** Port security (sticky MAC), PAT overload, SSHv2
- **Wireless:** WPA2-PSK per department

---

## Project Files
- `Company Business System Network Design (Sumaira).pkt` → Complete Packet Tracer simulation
- `Network_Design_Report_Sumaira_Safeer.pdf` → Full project report
- `documentation/` → Original Word document
- `screenshots/` → Verification evidence

---

## Results
All objectives successfully achieved and verified:
- End-to-end connectivity & inter-VLAN routing
- DHCP allocation across all departments
- Redundancy testing (link, device, ISP failure)
- Security features validation

---

## Future Enhancements
- First-Hop Redundancy (HSRP/VRRP)
- IPv6 dual-stack implementation
- Centralized monitoring (SNMP/Syslog)
- QoS for trading traffic

---

## References
- Cisco Networking Academy – Routing and Switching Essentials
- Cisco Packet Tracer Documentation

---

**Author:** Sumaira Safeer  

