# 🧠 HomeLab-Project-X

## 🚀 Overview

This repository documents my hands-on cybersecurity homelab project built to simulate a real-world enterprise environment.

The goal is to develop practical skills in:

* Network security
* Active Directory
* Threat detection
* Security monitoring

Rather than only learning theory, this project helps me understand how systems are built, attacked, monitored, and defended.

---

## 🏗️ Lab Environment

Current environment includes:

* Windows Server (Domain Controller)
* Windows Client Machines
* Linux Systems
* Kali Linux Attacker Machine
* Security Monitoring Server
* Virtual Network Environment

---

## 🎯 Skills Being Developed

* Windows Administration
* Active Directory Management
* Networking Fundamentals
* Offensive Security Concepts
* SIEM / Log Monitoring
* Detection Engineering
* Troubleshooting

---

## 📊 Progress

* [x] GitHub Project Created
* [x] Virtual Machines Setup
* [x] Network Connectivity
* [x] Domain Controller Deployment
* [x] Wazuh Integration
* [x] Detection Rules
* [ ] Final Documentation

---

## 📁 Project Structure

```bash
docs/
screenshots/
scripts/
notes/
diagrams/
```

---
## NAT Network

### NAT Network Setup
![NAT Configuration](screenshots/01-Network/01-nat-network-config.png)

![Network Adapter in Domain Controller](screenshots/01-Network/02-vm-network-adapter.png)


## Domain Controller

### Active Directory Configuration

![Admin Domain Joined](screenshots/02-domain-controller/01-admin-domains-joined.png)

![Active Directory Users](screenshots/02-domain-controller/02-active-directory-users.png)

![Server Manager](screenshots/02-domain-controller/03-server-manager-dashboard.png)

![Olivia Domain Joined](screenshots/02-domain-controller/04-olivia-domain-joined.png)

![Bothma Domain Joined](screenshots/02-domain-controller/05-bothma-domain-joined.png)

![Guest Domain Joined](screenshots/02-domain-controller/06-guest-domain-joined.png)

## Wazuh

### Wazuh Dashboard

![Linux Agent Connected](screenshots/03-Wazuh/01-linux-agent-connected.png)

![Wazuh Agents Overview](screenshots/03-Wazuh/02-wazuh-agents-overview.png)

![Domain Controller Monitoring](screenshots/03-Wazuh/03-domain-controller-monitoring.png)

![Wazuh Dashboard](screenshots/03-Wazuh/04-wazuh-dashboard.png)

![Domain Controller Agent Setup](screenshots/03-Wazuh/05-domain-controller-agent-setup.png)

![Windows Client Agent Setup](screenshots/03-Wazuh/06-windows-client-agent-setup.png)


## Client Systems

### Linux Client

![Linux Client IP Config](screenshots/04-Clients/01-linux-client-ip-config.png)

![Linux Hostname and IP](screenshots/04-Clients/02-linux-hostname-ip.png)

### Windows Client

![Windows Client IP Config](screenshots/04-Clients/03-windows-client-ip-config.png)


---

## 📌 Purpose

This project represents my transition from theory into practical cybersecurity experience by building and documenting a full lab environment.

---

## 🔄 Continuous Improvement

This repository will grow as I expand the lab, add detections, simulate attacks, and improve defenses.
