# 📦 pcap-arsenal

> *Every packet tells a story. A growing arsenal of PCAP files from hands-on Web App, API & Network penetration testing.*

![Wireshark](https://img.shields.io/badge/Tool-Wireshark-1679A7?style=flat&logo=wireshark&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=flat)
![Focus](https://img.shields.io/badge/Focus-Network%20Security-red?style=flat)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat)

---

## 📖 About This Repository

**pcap-arsenal** is a curated collection of Wireshark packet captures (.pcap / .pcapng) organized by network protocol and security topic. These captures are sourced from real-world lab environments, ethical hacking engagements, and controlled network simulations.

This repository is intended for:
- 🔐 Penetration Testers & Ethical Hackers
- 🧑‍💻 Network Security Analysts
- 🎓 Security Learners & Researchers
- 🛡️ SOC Analysts sharpening detection skills

> ⚠️ **Disclaimer:** All packet captures in this repository are collected from authorized lab environments and ethical hacking engagements only. This repository is strictly for educational and research purposes. Unauthorized network interception is illegal.

---

## 🗂️ Repository Structure

```
pcap-arsenal/
│
├── 802.1q/                  # VLAN Tagging — trunk traffic, tagged frames
├── 802.1x/                  # Port-based Network Access Control (NAC)
├── ARP/                     # Address Resolution Protocol — ARP spoofing, poisoning
├── BGP/                     # Border Gateway Protocol — session setup, route updates
├── GRE/                     # Generic Routing Encapsulation — tunneling traffic
├── HSRP/                    # Hot Standby Router Protocol — gateway redundancy
├── IGMPv2/                  # Internet Group Management Protocol — multicast joins
├── IPv6/                    # IPv6 traffic — NDP, ICMPv6, dual-stack behavior
├── ISE/                     # Cisco ISE — RADIUS auth, policy enforcement flows
├── IS-IS/                   # Intermediate System to Intermediate System routing
├── MTU-MSS-FRAG/            # MTU discovery, MSS negotiation, fragmentation
├── native-vs-normal/        # Native VLAN vs normal VLAN traffic comparison
├── OSPF/                    # Open Shortest Path First — LSA, neighbor adjacency
├── PIMv2/                   # Protocol Independent Multicast v2
├── Ping/                    # ICMP Echo — latency, TTL analysis, ICMP tunneling
├── QoS/                     # Quality of Service — DSCP marking, traffic shaping
├── Spanning-Tree/           # STP — BPDU frames, topology changes, root election
├── SSL/                     # SSL/TLS handshakes — cipher suites, cert analysis
├── TCP/                     # TCP fundamentals — handshake, retransmission, flags
├── Traceroute/              # Path discovery — UDP/ICMP traceroute behavior
└── vxlan-flood-learn/       # VXLAN overlay — BUM traffic, MAC learning, flood behavior
```

---

## 🔍 Topic Highlights

| Folder | Protocol / Topic | Security Relevance |
|---|---|---|
| `802.1q` | VLAN Tagging | VLAN hopping attacks |
| `802.1x` | NAC / EAP | Auth bypass, rogue device detection |
| `ARP` | Layer 2 Resolution | ARP spoofing, MITM |
| `BGP` | Routing Protocol | BGP hijacking, route leaks |
| `GRE` | Tunneling | Covert channels, tunnel abuse |
| `HSRP` | Gateway Redundancy | HSRP hijacking |
| `IGMPv2` | Multicast | Multicast flooding |
| `IPv6` | Next-gen IP | NDP spoofing, rogue RA |
| `ISE` | Cisco NAC | RADIUS traffic, policy bypass |
| `IS-IS` | Routing Protocol | Routing table manipulation |
| `MTU-MSS-FRAG` | Fragmentation | Fragmentation-based evasion |
| `native-vs-normal` | VLAN Behavior | Double tagging attack |
| `OSPF` | Routing Protocol | OSPF injection, neighbor spoofing |
| `PIMv2` | Multicast Routing | Multicast abuse |
| `Ping` | ICMP | ICMP tunneling, recon |
| `QoS` | Traffic Marking | QoS abuse, priority manipulation |
| `Spanning-Tree` | L2 Loop Prevention | STP root bridge attack |
| `SSL` | Encrypted Traffic | TLS downgrade, weak ciphers |
| `TCP` | Transport Layer | SYN floods, session hijacking |
| `Traceroute` | Path Discovery | Network mapping, TTL abuse |
| `vxlan-flood-learn` | Overlay Networking | BUM flooding, VXLAN misconfig |

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| **Wireshark** | Primary packet capture & analysis |
| **tshark** | CLI-based packet filtering & export |
| **tcpdump** | Lightweight capture on Linux |
| **GNS3 / EVE-NG** | Network lab simulation |
| **Scapy** | Custom packet crafting |

---

## 📌 How to Use

1. **Clone the repo**
   ```bash
   git clone https://github.com/YOUR_USERNAME/pcap-arsenal.git
   cd pcap-arsenal
   ```

2. **Open any .pcap file in Wireshark**
   ```bash
   wireshark 802.1q/capture.pcap
   ```

3. **Filter traffic using tshark**
   ```bash
   tshark -r SSL/tls-handshake.pcap -Y "tls.handshake"
   ```

---

## 👤 Author

**Dheeraj** — Certified Ethical Hacker | Web App & API Penetration Tester | Full Stack Developer

Domain Expertise: Income Tax · Retail · E-Commerce · Education · Freight Logistics · Banking

[![GitHub](https://img.shields.io/badge/GitHub-Profile-black?style=flat&logo=github)](https://github.com/YOUR_USERNAME)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://linkedin.com/in/YOUR_PROFILE)

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

> 💡 *Star ⭐ this repo if you find it useful. Contributions and pull requests for additional captures are welcome!*
