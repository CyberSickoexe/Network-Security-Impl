# Enterprise Network Security Architecture
<img width="562" height="378" alt="image" src="https://github.com/user-attachments/assets/2cc15772-ffac-4c8b-8954-65a8114b6286" />


# Enterprise Network Security Architecture

I have designed, configured, and documented a complete enterprise network security architecture, including **edge routing, firewalling, VLAN segmentation, server connectivity, and NAT configuration**. The network topology, IP addressing, device configurations, and security measures have all been implemented and tested to ensure proper connectivity and access control.

## Key Highlights

- **Network Topology:**  
  Logical layout includes:
  - Edge Router (1841)  
  - Firewall-Router (2811)  
  - Core Switch  
  - IoT Switch  
  - PCs (HR, Finance, IT Admin)  
  - IoT Server and SOC Server  

- **IP Addressing Scheme:**  
  Structured addressing with clear segmentation:
  - WAN: `203.0.133.x`  
  - LAN: `192.168.1.x / 192.168.2.x`  
  - Management VLANs included

- **Routing & NAT:**  
  Firewall-Router implements **PAT** for internal LAN hosts to access WAN. Default gateways configured for proper host routing.

- **VLAN & Segmentation:**  
  Core Switch and IoT Switch ports assigned to VLAN 1; management IPs configured for monitoring.

- **Security Controls:**  
  ACL 100 on Firewall-Router restricts LAN traffic; console/VTY passwords set for device access.

- **Testing & Validation:**  
  Connectivity verified between hosts, gateways, and WAN. NAT translation tested to confirm external access.

## Devices & Configurations

- **Edge-Router (1841):**  
  WAN and LAN interfaces configured with default route to ISP.

- **Firewall-Router (2811):**  
  NAT, ACLs, and interfaces configured to secure LAN-WAN traffic.

- **Core Switch & IoT Switch:**  
  VLAN 1 assigned for management and device segmentation.

- **Hosts/Servers:**  
  IPs, subnet masks, and gateways properly configured for network access.

> A professional topology diagram has been created showing all routers, switches, VLANs, servers, and IP addressing to provide a complete visual representation of the architecture.
