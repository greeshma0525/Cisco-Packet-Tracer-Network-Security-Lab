# Cisco Packet Tracer Network Security Lab

## Project Overview

This project demonstrates a segmented network designed and configured using Cisco Packet Tracer. It focuses on VLAN segmentation, inter-VLAN routing, access control, secure device management, and switch port security.

## Network Topology

The lab consists of:

* 2 routers: R1 and R2
* 4 switches: SW1, SW2, SW3, and SW4
* 6 PCs organized into three departmental VLANs

### End Devices

| PC Name | Department | VLAN | IP Address    |
| ------- | ---------- | ---- | ------------- |
| S1      | SALES      | 10   | 192.168.10.10 |
| S2      | SALES      | 10   | 192.168.10.11 |
| H1      | HR         | 20   | 192.168.20.10 |
| H2      | HR         | 20   | 192.168.20.11 |
| I1      | IT         | 30   | 192.168.30.10 |
| I2      | IT         | 30   | 192.168.30.11 |

## VLAN Configuration

| VLAN ID | Name   | Purpose                             |
| ------- | ------ | ----------------------------------- |
| 10      | SALES  | Sales department                    |
| 20      | HR     | Human Resources department          |
| 30      | IT     | IT department and device management |
| 99      | NATIVE | Native VLAN for trunk links         |

## IP Addressing

| Network / Interface   | IP Address       |
| --------------------- | ---------------- |
| SALES VLAN gateway    | 192.168.10.1/24  |
| HR VLAN gateway       | 192.168.20.1/24  |
| IT VLAN gateway       | 192.168.30.1/24  |
| R1–R2 link — R1       | 192.168.100.1/30 |
| R1–R2 link — R2       | 192.168.100.2/30 |
| R2 additional network | 10.10.10.0/24    |
| SW4 management SVI    | 192.168.30.2/24  |
| SW3 management SVI    | 192.168.30.3/24  |
| SW2 management SVI    | 192.168.30.4/24  |
| SW1 management SVI    | 192.168.30.5/24  |

## Security and Networking Features

* VLAN segmentation and trunk links
* Inter-VLAN routing using router-on-a-stick
* Static routing between R1 and R2
* Standard and extended Access Control Lists (ACLs)
* SSH version 2 for secure remote device management
* Management access restricted to the IT subnet using an ACL
* Switch port security with sticky MAC addresses
* Unused switch ports administratively shut down

## Testing and Verification

* Verified VLAN and trunk configurations
* Verified routing tables and static routes
* Tested permitted and restricted communication between VLANs
* Verified SSH management access from the IT subnet
* Checked switch port security configuration

## Tools Used

* Cisco Packet Tracer
* Cisco IOS CLI

## Project Files

* `Network-Security-Lab.pkt` — Packet Tracer topology and configurations
* `screenshots/` — Network topology, configuration, and verification evidence

## Learning Outcomes

This project strengthened my practical understanding of network segmentation, routing, access control, secure remote administration, and Layer 2 switch security.

---

**Author:** Greeshma Madalreddy
