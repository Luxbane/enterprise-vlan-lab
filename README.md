# GNS3 Enterprise VLAN Network

## 📖 Overview

This project simulates a small enterprise network infrastructure using GNS3. The network was designed with VLAN segmentation for different departments, inter-VLAN communication, automatic IP addressing using DHCP, internet access through NAT/PAT, and basic security policies using ACLs.

The topology demonstrates core networking concepts commonly used in enterprise environments, including router-on-a-stick architecture, 802.1Q trunking, and network segmentation.

---

# 🏢 Departments & VLANs

| Department | VLAN    | Network         | Gateway      |
| ---------- | ------- | --------------- | ------------ |
| IT         | VLAN 10 | 192.168.10.0/24 | 192.168.10.1 |
| HR         | VLAN 20 | 192.168.20.0/24 | 192.168.20.1 |
| Finance    | VLAN 30 | 192.168.30.0/24 | 192.168.30.1 |

---

# ⚙️ Technologies Used

* GNS3
* Cisco IOSv
* Cisco IOSvL2
* VPCS
* VLAN
* 802.1Q Trunking
* Router-on-a-Stick
* DHCP
* NAT Overload (PAT)
* ACL (Access Control List)

---

# 🛠️ Tasks Performed

1. Designed an enterprise-style network topology
2. Configured VLAN segmentation for multiple departments
3. Implemented 802.1Q trunk links between switches and router
4. Configured inter-VLAN routing using router subinterfaces
5. Deployed DHCP services for automatic IP assignment
6. Implemented NAT overload (PAT) for internet access
7. Applied ACL-based traffic restrictions between departments
8. Tested end-to-end connectivity and internet access

---

# 🌐 Network Features

## VLAN Segmentation

Each department was isolated into its own VLAN and subnet to improve organization, scalability, and security.

## Inter-VLAN Routing

Router-on-a-stick configuration was implemented to allow communication between VLANs through router subinterfaces.

## DHCP Services

The router dynamically assigned IP addresses, gateways, and network settings to client devices in each VLAN.

## NAT Overload (PAT)

Private internal addresses were translated to a public address to enable internet connectivity for all VLANs.

## ACL Security Policies

Access control rules were configured to restrict specific communication between departments.

---

# 🧪 Validation & Testing

The following tests were successfully performed:

* PC-to-PC communication within the same VLAN
* Inter-VLAN connectivity testing
* Internet connectivity testing
* DNS/domain access testing
* ACL restriction validation
* DHCP automatic address assignment verification

---

# 📸 Topology

images/Small Office.png

---

# 📂 Repository Structure

```text
configs/
├── Router.txt
├── SW1Core.txt
├── SW2Access.txt
├── SW3Access.txt
└── SW4Access.txt

images/
└── topology.png

project-files/
└── topology.gns3
```

---

# 🎯 Skills Demonstrated

* Enterprise network design
* VLAN implementation
* Layer 2 switching
* Inter-VLAN routing
* DHCP deployment
* NAT/PAT configuration
* ACL configuration
* Network troubleshooting
* Cisco CLI configuration
* GNS3 simulation design
