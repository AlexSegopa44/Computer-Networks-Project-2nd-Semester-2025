# Computer-Networks-Project-2nd-Semester-2025
Name: Ndivhuwo Alex Segopa
Module: Computer Networks Practical Project
Institution: North-West University
Feature Implemented: Port Security

Computer Networks project on cisco packet tracer which contains a variety of topologies, configuration of devices with IPv4 &amp; IPv6,VLAN segmentation including servers and implementation of port security on switches to control access to end devices.

## Part I – Network Topologies Design & Simulation

### Overview  
This project demonstrates the design, configuration, and simulation of **five classic network topologies** — Bus, Star, Ring, Mesh, and Extended Star — and an integrated **Hybrid Topology** combining elements of all.  

The hybrid topology features:  
- Dual Stack addressing (**IPv4 & IPv6**)  
- **VLAN segmentation** for departments (Admin and Finance)  
- Three dedicated servers (**DNS, DHCP, and Web**)  
- Basic Layer 2 security using **Port Security**

All designs were created and simulated using **Cisco Packet Tracer**.

---

### Topologies Implemented

| No. | Topology | Description |
|-----|-----------|-------------|
| 1 | **Bus** | Simple linear topology with a single communication backbone. |
| 2 | **Star** | Centralized connection through a main switch. |
| 3 | **Ring** | Devices connected in a closed loop for redundancy. |
| 4 | **Mesh** | High fault tolerance via multiple interconnections. |
| 5 | **Extended Star** | Multiple star topologies connected to a core switch. |
| 6 | **Hybrid** | Integration of the above topologies with dual-stack IP, VLANs, and servers. |

---

### Hybrid Network Overview

| Feature | Description |
|----------|-------------|
| **Addressing** | IPv4 and IPv6 (dual stack) |
| **VLANs** | VLAN 10 – Admin, VLAN 20 – Finance |
| **Servers** | DNS, DHCP, and Web servers configured and active |
| **Security** | Port Security on all access ports |


---


### IP Addressing Table

| Device | Interface | IPv4 Address | Subnet Mask | IPv6 Address | VLAN | Role |
|---------|------------|--------------|--------------|---------------|------|------|
| Router1 G0/0 | gig0/0 | 192.168.10.1 | 255.255.255.0 | 2001:DB8:1::1/64 | 1 | Gateway |
| Dr Shabangu PC | Fa0/1 | 192.162.10.5 | 255.255.255.0 | 2001:DB8:1::6/64 | 1 | Host |
| Router1 G0/1 | gig0/1 | 192.168.11.1 | 255.255.255.0 | 2001:DB8:20::1/64 | 1 | Gateway |
| Router1 G0/2 | gig0/2 | 192.168.12.1 | 255.255.255.0 | 2001:DB8:3::1/64 |1| Gateway |
| DNS Server | Fa0/10 | 192.168.10.8 | 255.255.255.0 | 2001:DB8:6::3/64 | 1 | DNS |
| DHCP Server | Fa0/11 | 192.168.15.4 | 255.255.255.0 | 2001:DB8:6::5/64 | 1 | DHCP |
| Web Server | Fa0/12 | 192.168.15.3 | 255.255.255.0 | 2001:DB8:6::4/64 | 1 | HTTP |
| Admin-PC1 | Fa0/1 | 192.168.10.2 | 255.255.255.0 | 2001:DB8:10::2/64 | 10 | Host |
| Finance-PC1 | Fa0/2 | 192.168.20.2 | 255.255.255.0 | 2001:DB8:20::2/64 | 20 | Host |
| **Testing** | Verified with successful IPv4/IPv6 ping and HTTP access |

