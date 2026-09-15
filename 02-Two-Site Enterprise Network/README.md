🌐 Two-Site Enterprise Network
Manual Configuration:
🎯 Objective
Design and implement a two-site enterprise network using Cisco devices in GNS3. Demonstrates VLAN segmentation, inter-VLAN routing, DHCP, WAN connectivity, and dynamic routing using OSPF.
🧩 Network Overview
HQ
- VLAN 10 – IT (192.168.10.0/24)
- VLAN 20 – HR (192.168.20.0/24)
- VLAN 30 – Guests (192.168.30.0/24)
- VLAN 99 – Management (192.168.100.0/24)
Branch
- VLAN 10 – IT (192.168.110.0/24)
- VLAN 20 – HR (192.168.120.0/24)
- VLAN 30 – Guests (192.168.130.0/24)
- VLAN 99 – Management (192.168.200.0/24)
WAN
- RW → 10.10.10.1/30
- RW-B → 10.10.10.2/30
- Inter-VLAN routing using Router-on-a-Stick
- DHCP provided by the routers
- OSPF Area 0 between the two routers
🖥️ Tools
- GNS3
- Cisco CSR1000v
- Cisco IOS L2 Switches
- VPCS
📊 Topology
