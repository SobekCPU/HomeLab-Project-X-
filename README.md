# HomeLab-Project-X

## 🚀 Overview

This repo documents my journey building a realistic cybersecurity homelab from the ground up.

Instead of just learning theory, I’m simulating a full enterprise environment including servers, workstations, attackers, and security tools to understand how real-world systems get attacked and defended.

This setup mirrors how actual business networks operate, allowing me to learn by doing, breaking and fixing.

## 🏗️ What I Built:

Inside this lab, I created a virtual corporate network with multiple systems interacting together:

🖥️ Domain Controller (authentication, DNS, DHCP)

🧑‍💻 Windows & Linux client machines

🔐 Dedicated security server

🧪 Security testing workstation

⚔️ Attacker machine

🌐 Internal network (10.0.0.0/24 NAT environment)

Everything runs inside virtualization (VirtualBox/VMware), simulating a real enterprise topology.

## 🎯 What This Lab Actually Does

This isn’t just a setup it’s a full attack + defense playground:

🔴 Offensive (Attacker Side)
Phishing simulation (credential harvesting)

Reverse shells (remote access)

Password attacks (brute force, wordlists)

Lateral movement & remote execution

🔵 Defensive (Blue Team)
Log monitoring & analysis

Intrusion detection

Vulnerability detection

Security event correlation

All of this is done using real tools used in industry.

## 🧰 Tools I’m Using

🛡️ Defensive Tools
Wazuh (SIEM + detection)

Security monitoring systems

Mail server simulation for phishing analysis

⚔️ Offensive Tools
Hydra (password cracking)

Evil-WinRM (remote command execution)

NetExec (lateral movement)

SecLists (payloads & wordlists)

RDP tools for system access

These tools reflect real-world cybersecurity workflows, not just labs.

## 🧪 Key Learning Areas

This homelab is helping me build skills in:

🧠 Networking fundamentals (IP ranges, NAT, DHCP)

🏢 Active Directory environments

🔍 Threat detection & logging

🕵️‍♂️ Ethical hacking techniques

🔐 Blue team vs red team mindset

🧱 Enterprise infrastructure design

📚 Why This Matters (For Me)
--
Most cybersecurity learning is:

fragmented

overly theoretical

or tool-focused without context

This project fixes that by giving me:

✅ Hands-on experience (not just watching videos)

✅ Real-world simulation of enterprise environments

✅ Understanding of attacker mindset AND defense strategy

✅ A portfolio project I can show recruiters

## 🔄 My Workflow

Build infrastructure

Configure systems

Introduce vulnerabilities

Simulate attacks

Detect & analyze activity

Improve defenses

This cycle helps me think like both an attacker and defender.

## Objective

To become sonmeone who doesn't just understand cybersecurity in theory, but can:
Design environments
Break systems
Detect threats
Respond like a professional
