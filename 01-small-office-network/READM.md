# 🧠 Small Office Network

## 🎯 Objective

Design and implement a small enterprise network using Cisco devices in GNS3.

This project demonstrates VLAN segmentation, trunking, inter-VLAN routing, DHCP, management VLAN configuration, basic Layer 2 security, and SSH management.

---

## 🧩 Network Overview

- VLAN 10 – IT (`192.168.10.0/24`)
- VLAN 20 – HR (`192.168.20.0/24`)
- VLAN 30 – Guests (`192.168.30.0/24`)
- VLAN 99 – Management (`192.168.100.0/24`)

### Routing

- Router-on-a-Stick
- Inter-VLAN routing provided by the Core-Router
- DHCP provided by the Core-Router

---

## 🖥️ Tools

- GNS3
- Cisco CSR1000v
- Cisco IOS L2 Switch
- 3 VPCS
- 1 SSH-Client
---

## 📊 Topology

![Topology](topology/topology.png)

---

## ⚙️ Configuration Summary

### Router — Core-Router

- Router-on-a-Stick
- VLAN subinterfaces
- Inter-VLAN routing
- DHCP for the VLAN networks
- Management connectivity

### Switch — SW

- VLAN 10 – IT
- VLAN 20 – HR
- VLAN 30 – Guests
- VLAN 99 – Management
- 802.1Q trunk toward the router
- Access ports assigned to the appropriate VLANs
- Basic Layer 2 security
- Management SVI

---

## 🧪 Verification

| Test | Screenshot |
|------|------------|
| VLAN | [View](screenshots/Vlans.png) |
| Trunk | [View](screenshots/Trunk.png) |
| Routing | [View](screenshots/Routing.png) |
| DHCP | [View](screenshots/dhcp.png) |
| Security | [View](screenshots/PortSecurity.png) |
| SSH to Router | [View](screenshots/sshToRouter.png) |
| SSH to Switch | [View](screenshots/sshToSw.png) |
