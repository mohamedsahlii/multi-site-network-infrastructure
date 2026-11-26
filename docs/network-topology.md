# Network Topology

The project is based on a multi-site network architecture connecting three locations:

- Tunis – R4
- Bizerte – R5
- Sfax – R6

Each site uses VLAN segmentation to separate administrative, technical, and server networks.

## Network Segments

| Site | VLAN 1 – ADMIN | VLAN 2 – TECH | VLAN 3 – SERVER |
|---|---|---|---|
| Tunis | Not specified | 10.0.2.0/24 | 10.0.3.0/24 |
| Bizerte | 10.1.1.0/24 | 10.1.2.0/24 | 10.1.3.0/24 |
| Sfax | 10.2.1.0/24 | Not configured | 10.2.3.0/24 |

## Security

ACL policies restrict communication between administrative and technical networks while permitting authorized access to server networks.
