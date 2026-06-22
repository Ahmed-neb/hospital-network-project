# hospital-network-project
# 🏥 Hospital Network Infrastructure Project

## 📌 Overview

This project presents a complete enterprise-level Hospital Network Infrastructure designed and implemented using Cisco networking technologies. The network architecture provides secure, scalable, and highly available communication between different hospital departments while maintaining strict security policies and efficient traffic management.

The design simulates a real-world hospital environment where multiple departments require isolated network segments, centralized services, secure remote management, monitoring systems, and controlled access to sensitive medical resources.

---

## 🎯 Project Objectives

* Build a secure and scalable hospital network.
* Segment departments using VLAN technology.
* Implement dynamic routing using OSPF.
* Provide automatic IP addressing through DHCP.
* Secure communication using SSH.
* Apply firewall policies and network access control.
* Enable network monitoring and management.
* Ensure redundancy and fault tolerance.
* Protect critical healthcare data from unauthorized access.

---

## 🏗 Network Architecture

The network consists of:

### Core Layer

* Core Switches
* High-speed backbone connectivity
* EtherChannel implementation
* Rapid PVST configuration

### Distribution Layer

* Routers connecting different network segments
* OSPF routing domain
* Traffic forwarding and policy enforcement

### Access Layer

* Departmental access switches
* End-user connectivity
* Port security implementation

### Security Layer

* Cisco ASA Firewall
* Data Center Firewall
* ACL-based traffic filtering
* NAT configuration

---

## 🏥 Hospital Departments (VLAN Segmentation)

| VLAN    | Department              |
| ------- | ----------------------- |
| VLAN 10 | Hospital Administration |
| VLAN 20 | Patient Records         |
| VLAN 30 | Clinical Laboratories   |
| VLAN 40 | Radiology Department    |
| VLAN 50 | Pharmacy                |
| VLAN 60 | Ward Station A          |
| VLAN 70 | Ward Station B          |
| VLAN 80 | Emergency Room          |
| VLAN 99 | Management Network      |

Each department is isolated in its own VLAN to improve security, reduce broadcast traffic, and simplify management.

---

## 🌐 Routing Configuration

### OSPF Dynamic Routing

The network uses OSPF Area 0 as the primary routing protocol.

Features:

* Automatic route advertisement
* Fast convergence
* Scalable routing architecture
* Inter-router communication

### Static Routing

Static routes are configured where required for:

* Internet access
* Firewall connectivity
* External network reachability

---

## 📡 DHCP Services

DHCP pools are configured for all VLANs to provide:

* Automatic IP assignment
* Default gateway configuration
* DNS server allocation
* Centralized address management

---

## 🔥 Firewall Implementation

### Cisco ASA Firewall

Provides:

* Perimeter security
* Access control
* Network Address Translation (NAT)
* Secure remote management

### Data Center Firewall

Protects:

* Hospital Information System (HIS)
* Zabbix Monitoring Server
* Internal Data Center Services
* DMZ Resources

---

## 🔒 Security Features

### Access Control Lists (ACLs)

Implemented to:

* Restrict unauthorized access
* Control inter-VLAN communication
* Protect sensitive departments
* Filter incoming and outgoing traffic

### SSH Secure Management

All networking devices support:

* SSH Version 2
* Encrypted remote administration
* Local user authentication

### Port Security

Implemented on access switches to:

* Limit connected devices
* Prevent unauthorized access
* Learn MAC addresses dynamically
* Reduce Layer 2 attacks

### DHCP Snooping

Protects against:

* Rogue DHCP Servers
* DHCP Spoofing Attacks

### Dynamic ARP Inspection (DAI)

Protects against:

* ARP Spoofing
* Man-in-the-Middle Attacks

---

## 🔄 Redundancy & High Availability

The network includes:

* Multiple routers
* EtherChannel links
* Redundant paths
* Backup switch connectivity
* OSPF failover capabilities

These mechanisms ensure uninterrupted communication during failures.

---

## 📊 Network Monitoring

### Zabbix Monitoring

Used for:

* Device monitoring
* Availability tracking
* Performance analysis
* Network health monitoring

### SNMP

Configured across network devices for:

* Statistics collection
* Monitoring integration
* Fault detection

### SPAN Monitoring

Traffic mirroring is configured for:

* Packet analysis
* Security investigations
* Troubleshooting

---

## 🧪 Testing Performed

The following tests were successfully conducted:

### Connectivity Testing

* Ping Tests
* End-to-End Communication Validation

### Remote Access Testing

* SSH Connectivity

### Security Testing

* MAC Flooding Protection
* DHCP Spoofing Protection
* ARP Spoofing Protection

### Monitoring Validation

* SNMP Monitoring
* Zabbix Integration

---

## 🛠 Technologies Used

* Cisco Routers
* Cisco Switches
* Cisco ASA Firewall
* OSPF Routing Protocol
* VLANs
* Inter-VLAN Routing
* DHCP
* NAT
* ACLs
* SSH
* SNMP
* EtherChannel
* Rapid PVST
* DHCP Snooping
* Dynamic ARP Inspection
* Zabbix Monitoring

---

## 📈 Project Outcomes

This project demonstrates the implementation of a modern hospital network capable of supporting secure communication, efficient departmental isolation, centralized management, and advanced security controls. The design follows enterprise networking best practices and can be extended to support larger healthcare environments.

---

## 👨‍💻 Author

Ahmed
Computer Networks Student

Network Design | Routing & Switching | Network Security | Infrastructure Management
