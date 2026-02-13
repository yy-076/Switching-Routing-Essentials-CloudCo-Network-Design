# CT133-3-2-SRE — Cloud Co Network (Cisco Packet Tracer)

This repository contains the design and implementation of a secure, scalable enterprise network for **Cloud Co**, simulated using **Cisco Packet Tracer**.

The topology covers 3 main sites (**Kuala Lumpur HQ, Penang, Johor**) and a **Server Farm**, including LAN segmentation, WAN routing, WLAN deployment, and basic security hardening.

---

## Project Scope (What is implemented)
### LAN (Switching)
- VLAN segmentation (department-based)
- Voice VLAN
- Access ports & trunk ports (802.1Q, native VLAN)
- EtherChannel (link aggregation + redundancy)

### Inter-VLAN & Gateway Redundancy
- Router-on-a-Stick (ROAS)
- HSRP (active/standby gateway per VLAN)

### WAN (Routing)
- OSPF (Area 0)
- Default static route + floating static route

### Wireless (Penang)
- WLC-based WLAN
- VLAN-WLAN mapping + WPA2-PSK
- LAP registration (CAPWAP)

### Server Farm Services
- DHCP, DNS, Web (HTTP), FTP
- Verification using end-device tests

### Security
- SSH device access
- Layer 2 attack mitigations (e.g., BPDU Guard/PortFast, port shutdown, blackhole VLAN)

---

## Repository Structure
- `packet-tracer/` : Final Packet Tracer topology (.pkt)
- `report/` : Final group report (PDF/DOCX)
- `configs/` : Saved running-config outputs (routers/switches by site)
- `addressing/` : IPv4 addressing table (VLSM)
- `evidence/` : Screenshots + ping/tracert outputs for verification

---

## How to Run
1. Install **Cisco Packet Tracer**
2. Open: `packet-tracer/CloudCo_Final.pkt`
3. Use the report to follow verification steps (HSRP/OSPF/WLAN/Server tests)

---

## Module Info
- Module: CT133-3-2-SRE (Switching and Routing Essentials)
- Simulation Tool: Cisco Packet Tracer

---

## Credits
Group: HELLO KITTY
(Refer to the report for full member list and TP numbers.)
