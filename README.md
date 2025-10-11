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
| 5 | **Extended Star** | Multiple star topologies connected to a core router. |
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
| Dr Masiya PC | Fa0/1 | 192.168.10.4 | 255.255.255.0 | 2001:DB8:1::5/64 | 1 | Host |
| Dr Ngwenya PC | Fa0/1 | 192.168.10.2 | 255.255.255.0 | 2001:DB8:1::3/64 | 1 | Host |
| Offices DHCP Server | Fa0/1 | 192.168.10.11 | 255.255.255.0 | 2001:DB8:1::2/64 | 1 | Host |
| Router1 G0/1 | gig0/1 | 192.168.11.1 | 255.255.255.0 | 2001:DB8:2::1/64 | 1 | Gateway |
| Dr Segopa's PC | Fa0/2 | 192.168.11.4 | 255.255.255.0 | 2001:DB8:2::2/64 | 1 | Host |
| Dr Segopa Laptop | Fa0/3 | 192.168.11.2 | 255.255.255.0 | 2001:DB8:2::3/64 | 1 | Host |
| Dr Segopa Office Printer | Fa0/4 | 192.168.11.3 | 255.255.255.0 | 2001:DB8:2::4/64 | 1 | Host |
| Router1 G0/2 | gig0/2 | 192.168.12.1 | 255.255.255.0 | 2001:DB8:3::1/64 | 1 | Gateway |
| Router2 G0/0 | gig0/0 | 192.168.12.2 | 255.255.255.0 | 2001:DB8:3::2/64 | 1 | Gateway |
| Router2 G0/1 | gig0/1 | 192.168.14.1 | 255.255.255.0 | 2001:DB8:5::1/64 | 1 | Gateway |
| Ward Monitor 1 | Fa0/3 | 192.168.14.10 | 255.255.255.0 | 2001:DB8:5::2/64 | 1 | Host | 
| Ward Monitor 2 | Fa0/4 | 192.168.14.8 | 255.255.255.0 | 2001:DB8:5::3/64 | 1 | Host |
| Ward Monitor 3 | Fa0/3 | 192.168.14.3 | 255.255.255.0 | 2001:DB8:5::4/64 | 1 | Host |
| Ward Monitor 4 | Fa0/3 | 192.168.14.9 | 255.255.255.0 | 2001:DB8:5::5/64 | 1 | Host |
| Ward Monitor 5 | Fa0/4 | 192.168.14.4 | 255.255.255.0 | 2001:DB8:5::6/64 | 1 | Host |
| Ward Monitor 6 | Fa0/2 | 192.168.14.7 | 255.255.255.0 | 2001:DB8:5::7/64 | 1 | Host |
| Ward Monitor 7 | Fa0/3 | 192.168.14.6 | 255.255.255.0 | 2001:DB8:5::8/64 | 1 | Host |
| Router 2 G0/2 | gig0/2 | 192.168.13.1 | 255.255.255.0 | 2001:DB8:4::1/64 | 1 | Gateway |
| Waiting Area Monitor 1 | Fa0/3 | 192.168.13.8 | 255.255.255.0 | 2001:DB8:4::5/64 | 1 | Host |
| Waiting Area Monitor 2 | Fa 0/3 | 192.168.13.6 | 255.255.255.0 | 2001:DB8:4::3/64 | 1 | Host |
| Admin Department PC | Fa0/6 | 192.168.13.9 | 255.255.255.0 | 2001:DB8:4::4/64 | 20 | Host |
| Admin Department Printer | Fa0/5 | 192.168.13.7 | 255.255.255.0 | 2001:DB8:4::8/64 |20 | Host |
| Finance Laptop | Fa0/4 | 192.168.13.3 | 255.255.255.0 | 2001:DB8:4::6/64 | 10 | Host |
| Finance PC | Fa0/3 | 192.168.13.9 | 255.255.255.0 | 2001:DB8:4::4/64 | 10 | Host |
| Router3 G0/0 | gig0/0 | 192.168.13.254 | 255.255.255.0 | 2001:DB8:4::2/64 | 1 | Gateway |
| Router3 G0/1 | gig0/1 | 192.168.15.1 | 255.255.255.0 | 2001:DB8:6::1/64 | 1 | Gateway |
| IT Helpdesk | Fa0/5 | 192.168.15.2 | 255.255.255.0 | 2001:DB8:6::2/64 | 1 | Host | 
| DNS Server | Fa0/2 | 192.168.15.8 | 255.255.255.0 | 2001:DB8:6::3/64 | 1 | DNS |
| DHCP Server | Fa0/11 | 192.168.15.4 | 255.255.255.0 | 2001:DB8:6::5/64 | 1 | DHCP |
| Web Server | Fa0/12 | 192.168.15.3 | 255.255.255.0 | 2001:DB8:6::4/64 | 1 | HTTP |
| **Testing** | Verified with successful IPv4/IPv6 ping and HTTP access |

