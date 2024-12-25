Hotel Network Design Project

Overview

This project involves designing and implementing a modern hotel network infrastructure for a multi-floor building with eight departments distributed across three floors. The network was created to meet operational, connectivity, and security requirements using VLANs, dynamic IP allocation, routing protocols, and secure remote access.

Network Requirements
Building Structure:

1st Floor: Reception, Store, Logistics.
2nd Floor: Finance, HR, Sales/Marketing.
3rd Floor: IT, Admin.
Hardware Configuration:

Routers: Three routers placed in the IT department server room, connected using serial DCE cables.
Switches: One switch per floor, connected to their respective routers.
Devices: Each department equipped with laptops, phones, printers, and Wi-Fi access.
VLAN Configuration: Each department operates within its own VLAN for logical segmentation and efficient communication:

1st Floor:
VLAN 80: Reception (192.168.8.0/24)
VLAN 70: Store (192.168.7.0/24)
VLAN 60: Logistics (192.168.6.0/24)
2nd Floor:
VLAN 50: Finance (192.168.5.0/24)
VLAN 40: HR (192.168.4.0/24)
VLAN 30: Sales/Marketing (192.168.3.0/24)
3rd Floor:
VLAN 20: Admin (192.168.2.0/24)
VLAN 10: IT (192.168.1.0/24)
Routing:

Implemented OSPF to advertise routes and ensure seamless communication between VLANs.
Inter-router communication configured with networks:
10.10.10.0/30
10.10.10.4/30
10.10.10.8/30
Dynamic IP Allocation:

Configured DHCP servers on routers to dynamically allocate IP addresses to devices in their respective VLANs.
Security and Management:

Configured SSH on all routers for secure remote access.
Implemented port security on the IT department switch:
Restricted access on port fa0/1 to a Test-PC using the sticky MAC address method.
Set violation mode to shutdown for unauthorized access.
Key Features
Logical segmentation using VLANs for efficient network traffic management.
Dynamic IP addressing to reduce administrative overhead.
Secure communication with OSPF routing and SSH configuration.
Robust access control with port security mechanisms.
Scalable design to accommodate the hotel's operational needs.
Skills Demonstrated
Network design and implementation using VLANs and subnets.
Configuring DHCP, OSPF, and secure remote access with SSH.
Applying security measures like sticky MAC addressing and port security.
Utilizing Cisco Packet Tracer for simulation and testing.
Project Outcomes
This project highlights the integration of routing, switching, dynamic IP configuration, and security features to create a robust and efficient network. It demonstrates a strong understanding of network protocols, design principles, and practical implementation.

Feel free to clone the repository or explore the detailed configuration files for more insights. Contributions and suggestions are always welcome!
