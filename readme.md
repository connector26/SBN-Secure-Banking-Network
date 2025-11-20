🏦 Secure Banking Network – Cisco Packet Tracer

A fully simulated secure banking infrastructure built in Cisco Packet Tracer, featuring VLAN segmentation, multilayer switching, routing security, ACLs, and controlled inter-department communication. This project demonstrates best practices for securing financial networks.

📌 Project Overview

This project models a real-world banking network with a focus on security, segmentation, and controlled access. The design isolates departments, protects internal data, and enforces strict communication rules using Cisco networking technologies.

🛡️ Key Features

VLAN Segmentation for departments (IT, HR, Finance, Managers, Security).

Layer 3 Inter-VLAN Routing with restricted access.

Access Control Lists (ACLs) to secure critical services and limit communication.

Secure Router Configuration (SSH, passwords, banners, disabled unnecessary services).

Firewall-like Filtering using extended ACLs.

DHCP / Static IP Assignments depending on department security levels.

Redundant Switch Links (optional) to enhance reliability.

End-to-end Testing including ping, traceroute, packet simulation.

🗂️ Network Components
Component	Description
Routers	Core routing + secured management access
Layer 2/3 Switches	VLANs, trunking, inter-VLAN routing
Servers	DHCP, DNS, Authentication (optional)
Bank Staff PCs	Segmented per department
Security Systems	Monitoring/Logging (optional in layout)
🧩 Network Topology

The topology includes:

Departmental VLANs

A central router or multilayer switch

Trunk links between switches

Separate subnets for each department

ACLs to limit access from one segment to another

A management network for IT administrators

(Add your Packet Tracer topology image here if available)

![Network Topology](topology.png)

🔐 Security Measures Implemented
1. VLAN-Based Isolation

Each department is placed in its own VLAN:

VLAN 10 – IT

VLAN 20 – HR

VLAN 30 – Finance

VLAN 40 – Managers

VLAN 50 – Security Team

2. ACL Policies

Examples:

Finance VLAN blocked from HR network

HR VLAN allowed to access shared services only

Only IT VLAN may SSH into routers/switches

Managers VLAN allowed full access

Public access fully restricted

3. Router Hardening

Encrypted passwords

SSH remote access only

Login banners for legal warning

Disabled CDP/unused ports

4. Switch Hardening

Port security

BPDU Guard (optional)

Shutdown unused ports

🧪 Testing & Verification

Use Packet Tracer’s Simulation Mode to validate:

Ping + inter-VLAN communication

ACL behavior

DHCP assignments

Failures and recovery

Device reachability

📁 Repository Contents
📦 Secure-Banking-Network
 ├── topology.pkt          # Cisco Packet Tracer file
 ├── configs/              # Router + Switch configurations
 ├── README.md             # Documentation
 └── notes/                # Optional design notes or screenshots

🚀 How to Use

Open Cisco Packet Tracer 8.x

Load topology.pkt

Explore device CLI configurations

Test communication between VLANs

Review the ACLs to understand security behavior

🤝 Contributions

Contributions, improvements, and suggestions are welcome!
Feel free to open a pull request or issue.

📜 License

This project is released under the MIT License.