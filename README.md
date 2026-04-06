Enterprise Multi-Branch Network Design

A comprehensive network simulation of a 3-branch enterprise infrastructure (Bangkok HQ, Phuket, and Chiang Mai) using Cisco Packet Tracer.

Project Overview
This project demonstrates the implementation of a scalable and secure enterprise network. It features multi-departmental segmentation using VLANs, inter-branch connectivity via OSPF, and secure internet access through NAT/PAT.

Key Technical Features

- Routing: Configured OSPF (Area 0) for dynamic routing between branches and Static Default Routing for internet egress.

- VLAN & Inter-VLAN Routing: Implemented 802.1Q Router-on-a-Stick to segment the network into Admin (VLAN 10) and Sale (VLAN 20) departments.- 

- Network Services: * DHCP Server: Localized pools for automatic IP assignment per VLAN.

- Security: * Device hardening with Enable Secret and Line Console/VTY passwords
   - Enabled Service Password-Encryption for configuration security.
   - Custom Banner MOTD for unauthorized access warnings.

  <img width="1659" height="714" alt="image" src="https://github.com/user-attachments/assets/73fedb45-df0a-4ccf-a31f-4836dc005ddf" />
