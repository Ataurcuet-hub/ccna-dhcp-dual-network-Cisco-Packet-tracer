# ccna-dhcp-dual-network-Cisco-Packet-tracer
A Cisco Packet Tracer project demonstrating DHCP-based dual networks with integrated wired and wireless hosts.
# Dual Network DHCP with Wireless & Wired Hosts – Packet Tracer Project

## Project Overview
This Packet Tracer project uses a single router to configure two separate networks: one with wireless hosts connected through an Access Point (AP) and the other with wired hosts connected via a switch. DHCP is used on both networks to provide dynamic IP addressing for all end devices.

---

## Network Design Summary

### Devices Used
- 1 × Router
- 2 × Switch
- 1 × Access Point (AP)
- 3 × Wireless Hosts
- 3 × Wired Hosts

---

## IP Addressing & Network Information

### Network–1 (Wireless Side)
- Network Address: 192.168.2.0 /24
- Default Gateway: 192.168.2.1
- Router Interface: FastEthernet0/0
- Access Point Gateway: 192.168.2.0 255.255.255.0
- IP Assignment: DHCP
- Hosts: 3 Wireless Clients

### Network–2 (Wired Side)
- Network Address: 192.168.3.0 /24
- Router Interface: FastEthernet0/1
- IP Assignment: DHCP
- Hosts: 3 Wired PCs
- All switches are connected to the same DHCP-enabled router

---

## Router Interface Configuration (Summary)

- FastEthernet0/0  
  Used for Wireless Network (192.168.2.0/24)

- FastEthernet0/1  
  Used for Wired Network (192.168.3.0/24)

Each interface is configured with IP addressing and enabled using `no shutdown`.

---

## DHCP Configuration

The router is configured with separate DHCP pools for both networks to ensure dynamic IP allocation for all end devices.

- Wireless hosts receive IPs from the 192.168.2.0/24 network
- Wired hosts receive IPs from the 192.168.3.0/24 network
- Default gateway is provided automatically through DHCP

---

## Connectivity & Verification

The following tests were successfully performed:

- All hosts received IP addresses dynamically using DHCP
- Wireless hosts can communicate with each other
- Wired hosts can communicate with each other
- Cross-network communication is successful via the router
- Ping tests between wireless and wired hosts were successful

---

## Learning Outcomes

- Configuration of multiple DHCP networks on a single router
- Understanding FastEthernet interface-based network separation
- Wireless and wired network integration
- Practical experience with dynamic IP addressing
- End-to-end connectivity verification using ping

---

## Project Files

- Packet Tracer File (.pkt)
- README.md
- Screenshots (Topology and successful ping results)

---

## Notes

This project was created for learning and practice purposes using Cisco Packet Tracer.  
It demonstrates real-world concepts of DHCP, routing between networks, and mixed wired/wireless environments.

---

## Author
Ataur Rahman  
Networking Learner
