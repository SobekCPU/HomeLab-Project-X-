# Project X Enterprise Security Homelab (HeavyWeight)

## Overview

Project X is a self-built enterprise cybersecurity homelab designed to simulate a realistic corporate network environment. The lab focuses on identity management, endpoint monitoring, network administration, and security operations through centralized logging and threat detection.

This environment is built using Oracle VM VirtualBox and operates on an isolated NAT Network, allowing controlled communication between virtual machines while maintaining separation from the host system.

This project reflects a hands-on approach to learning enterprise security concepts under real hardware constraints.

---

## Objectives

The goal of Project X is to build practical, job-ready skills in:

* Active Directory administration
* Windows and Linux system management
* SIEM deployment and monitoring
* Endpoint detection and response concepts
* Network design and segmentation
* Security event analysis
* Detection engineering fundamentals

---

## Network Architecture

### Virtual Network Configuration

| Setting      | Value          |
| ------------ | -------------- |
| Network Type | NAT Network    |
| Network Name | project-x-nat  |
| Subnet       | 10.0.0.0/24    |
| DHCP Range   | 10.0.0.100–200 |

### Design Approach

The lab follows a centralized architecture where core services such as authentication, DNS, DHCP, and security monitoring are hosted on dedicated servers.

Static IP addresses are assigned to critical infrastructure systems to ensure consistent communication and stability across the network.

---

## Lab Systems

### project-x-sec-box

**Role**
Security Monitoring Server

**Purpose**
Hosts the SIEM stack responsible for centralized logging, monitoring, and threat detection across the environment.

**Services**

* Wazuh Manager
* Wazuh Indexer
* Wazuh Dashboard

**IP Address**
`10.0.0.10`

**Responsibilities**

* Collect logs from all endpoints
* Detect suspicious activity using rules and decoders
* Generate security alerts
* Monitor file integrity
* Provide centralized visibility

---

### project-x-dc

**Role**
Domain Controller

**Purpose**
Provides centralized identity and network services.

**Services**

* Active Directory Domain Services
* DNS Server
* DHCP Server

**IP Address**
`10.0.0.5`

**Responsibilities**

* Manage users and computers
* Handle authentication across the domain
* Provide DNS resolution
* Assign IP addresses via DHCP

---

### project-x-admin

**Role**
Corporate Server

**Purpose**
Represents internal business systems and administrative infrastructure.

**IP Address**
`10.0.0.8`

**Responsibilities**

* Host internal services
* Support administrative operations
* Act as a monitored asset within the network

---

### project-x-win-client

**Role**
Windows Workstation

**Purpose**
Simulates a standard enterprise user endpoint.

**Responsibilities**

* Join the Active Directory domain
* Generate user activity and system logs
* Run a Wazuh agent for monitoring

---

### project-x-linux-client

**Role**
Linux Workstation

**Purpose**
Provides cross-platform visibility and testing within the environment.

**Responsibilities**

* Generate Linux system logs
* Forward logs to the SIEM
* Validate monitoring across operating systems

---

### project-x-sec-work

**Role**
Security Workstation

**Purpose**
Dedicated system for testing, monitoring, and security analysis.

**Responsibilities**

* Simulate attack scenarios
* Test detection rules
* Validate security controls

---

### attacker

**Role**
Adversary Simulation System

**Purpose**
Used to perform controlled attacks to test detection and monitoring capabilities.

**Responsibilities**

* Execute simulated attacks
* Generate security events
* Validate alerting and detection accuracy

---

## Wazuh Monitoring

### Agent Configuration

All monitored systems are configured to send logs to:

* Server: `10.0.0.10`
* Port: `1514`

### Monitoring Capabilities

* Centralized log collection
* File integrity monitoring
* Authentication tracking
* Threat detection and alerting

---

## Security Use Cases

This lab supports multiple real-world detection scenarios:

* Failed login attempts
* Privilege escalation activity
* Unauthorized access attempts
* Malware simulation detection
* File integrity changes
* Correlation of security events

---

## Hardware Constraints and Optimization

This project is built on limited hardware and reflects realistic resource management.

### Host Specifications

* 8 GB RAM
* 2 CPU cores

### Optimization Strategy

* Run a maximum of two virtual machines at a time
* Reduce memory usage for the SIEM stack
* Use headless mode to reduce overhead
* Build and test the lab in phases rather than all at once

---

## Skills Demonstrated

This project showcases hands-on experience in:

* Virtualization and lab design
* Active Directory deployment and management
* Windows Server administration
* Linux system administration
* SIEM implementation
* Endpoint monitoring and logging
* Network configuration
* Security operations workflows

---

## Future Improvements

Planned enhancements for Project X include:

* Network segmentation and firewall deployment
* DMZ implementation
* Automated setup scripts
* Advanced detection rules
* Expanded attack simulations

---

## Repository Structure

```text
/docs
  overview.md

/screenshots
  .gitkeep

/notes
  daily-log.md

/scripts
  .gitkeep

/diagrams
  .gitkeep
```

---

## Notes

This homelab is designed and maintained as a continuous learning project. It is built incrementally, tested under constraints, and documented to reflect real-world problem solving and system design decisions.
