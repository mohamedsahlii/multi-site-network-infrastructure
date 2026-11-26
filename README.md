# Multi-Site Network Infrastructure – VLAN & Inter-Site Routing

## Project Overview

This project focuses on designing and implementing a multi-site enterprise network infrastructure based on network segmentation, inter-site routing, and access control.

The architecture includes three sites: Tunis, Bizerte, and Sfax.

The main objective is to improve network organization, communication between sites, and security through VLAN segmentation and Access Control Lists (ACLs).

## Network Architecture

The infrastructure consists of three interconnected sites:

- **Tunis:** Router R4
- **Bizerte:** Router R5
- **Sfax:** Router R6

## VLAN Segmentation

Three VLANs were defined:

| VLAN | Name | Purpose |
|---|---|---|
| VLAN 1 | ADMIN | Administration |
| VLAN 2 | TECH | Technical department |
| VLAN 3 | SERVER | Servers |

Each site uses the VLANs according to its network requirements.

## IP Addressing

### Tunis – R4

- VLAN 2: 10.0.2.1
- VLAN 3: 10.0.3.1

### Bizerte – R5

- VLAN 1: 10.1.1.0/24
- VLAN 2: 10.1.2.0/24
- VLAN 3: 10.1.3.0/24

### Sfax – R6

- VLAN 1: 10.2.1.1
- VLAN 3: 10.2.3.1

## Routing and Network Connectivity

Inter-site routing was configured to enable communication between the different network segments across the three sites.

Connectivity tests were performed to verify communication between authorized networks.

## Access Control Lists (ACLs)

ACLs were implemented to enforce network access policies.

| Source | Destination | Policy |
|---|---|---|
| VLAN 1 – ADMIN | VLAN 3 – SERVER | Allowed |
| VLAN 1 – ADMIN | VLAN 2 – TECH | Denied |
| VLAN 2 – TECH | VLAN 3 – SERVER | Allowed |
| VLAN 2 – TECH | VLAN 1 – ADMIN | Denied |

These rules help isolate administrative and technical traffic while allowing authorized access to server resources.

## Technologies Used

- Cisco Networking
- VLAN
- Inter-VLAN Routing
- Inter-Site Routing
- Cisco IOS
- Access Control Lists (ACL)
- Network Troubleshooting
- Cisco Packet Tracer

## Skills Demonstrated

- Enterprise Network Design
- Network Segmentation
- Routing Configuration
- Network Security
- ACL Implementation
- Connectivity Testing

## Author

**Mohamed Sahli**

Applied Bachelor's Student – Computer Networks and Information Systems (RSI)

ISET Bizerte, Tunisia

[LinkedIn](https://www.linkedin.com/in/sahlii-mohamed-3aa578451/) | [GitHub](https://github.com/mohamedsahlii)

---

*Academic networking project – Multi-site enterprise network design and implementation.*
