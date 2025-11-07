# Small-Office-Network-Simulation-Cisco-Packet-Tracer-


## 📘 Overview
This project demonstrates how to design and configure a **small office network** using **Cisco Packet Tracer**.  
The network includes **two switches**, **one router**, and **four PCs**.  
Each switch represents a local network (LAN), and the router connects both LANs to allow communication between devices.

Through this project, I learned how routers, switches, and PCs communicate and how to configure IP addressing, default gateways, and router interfaces for network connectivity.

---

## 🧠 Key Concepts Learned
- **Switches** connect devices within a local area network (LAN).  
- **Routers** connect multiple LANs and direct traffic between different networks.  
- **Default Gateway** is the “exit door” for devices to reach other networks through the router.  
- Each interface on a router must be assigned an IP address to identify which network it belongs to.  
- **Subnet masks** define the range of IP addresses within a network.  
- Learned to test connectivity using the **ping command** in Packet Tracer’s Command Prompt.

---

🖥️ Network Topology Description

This network follows a star topology design, where two local area networks (LANs) are connected through a central router. Each LAN is managed by a switch that connects multiple PCs, allowing devices on the same network to communicate directly. The router acts as the gateway between both LANs, enabling inter-network communication and serving as the path for data to travel between different subnets. This setup mirrors how real-world small office or campus networks operate, separating traffic for efficiency and control while maintaining full connectivity across the organization.



**Devices Used:**
- Router: `Cisco 2901`
- Switches: `Cisco 2960-24TT`
- PCs: `PC0, PC1, PC2, PC3`

---

## ⚙️ Configuration Summary

### Router Configuration

enable
configure terminal

interface gigabitEthernet 0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
exit

interface gigabitEthernet 0/1
ip address 192.168.2.1 255.255.255.0
no shutdown
exit

end


### PC IP Configuration

| PC | IP Address | Subnet Mask | Default Gateway |
|----|-------------|--------------|------------------|
| PC0 | 192.168.1.2 | 255.255.255.0 | 192.168.1.1 |
| PC2 | 192.168.1.3 | 255.255.255.0 | 192.168.1.1 |
| PC1 | 192.168.2.2 | 255.255.255.0 | 192.168.2.1 |
| PC3 | 192.168.2.3 | 255.255.255.0 | 192.168.2.1 |

---
✅ Successful replies indicate both LANs can communicate through the router.

---

## 📊 What I Learned
- How to design a basic **two-network topology** using Cisco Packet Tracer.  
- How to **assign IP addresses and subnet masks** logically.  
- How to configure **router interfaces** and bring them online using the `no shutdown` command.  
- How to use **ping** to test network reachability.  
- The importance of the **default gateway** in inter-network communication.  
- Real-world understanding of how **routers and switches** connect multiple departments or office floors in a company.

---

## 🚀 Future Improvements
- Add a **DHCP server** to automate IP assignments.
- Add a **web server** to simulate Internet access.
- Connect the router to a **Cloud (Internet)** module for external communication.
- Implement VLANs and routing protocols like RIP or OSPF.

---

## 🧰 Tools Used
- **Cisco Packet Tracer v8.x**
- **Command Line Interface (CLI)**
- **Ping utility** for testing network connectivity

---

## 👩🏽‍💻 Author
**Amani Evans**  
Engineering Management & Cybersecurity Enthusiast  
