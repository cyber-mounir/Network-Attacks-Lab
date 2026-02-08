# MAC Flooding Attack

## 📌 Overview
This project studies the **MAC Flooding attack**, a Layer 2 network attack that
targets the CAM (MAC address) table of a switch.  
The goal is to understand how this attack works, its impact on switched networks,
and how it can be mitigated using proper security mechanisms.

---

## 🎯 Objectives
- Understand how a switch learns MAC addresses
- Explain how CAM table overflow occurs
- Analyze the security impact of MAC Flooding
- Demonstrate why this attack enables further attacks such as sniffing and MITM
- Study effective defense techniques

---

## 🧪 Lab Environment
This project was implemented in a controlled lab environment using:

- GNS3
- Kali Linux (Attacker)
- Ubuntu Linux (Victim)
- Layer 2 Switch
- Router (Gateway)

⚠️ No real or public networks were involved.

---

## 🧠 Attack Description
A switch uses a CAM table to map MAC addresses to physical ports.
In a MAC Flooding attack, the attacker sends a large number of Ethernet frames
with **fake source MAC addresses**.

As a result:
- The CAM table becomes full
- The switch cannot learn new MAC addresses
- The switch starts broadcasting frames to all ports

This behavior makes the switch act like a **hub**, which breaks network isolation.

---

## ⚠️ Impact
- Loss of switch efficiency
- Increased broadcast traffic
- Traffic exposure to unauthorized hosts
- Enables packet sniffing
- Prepares the network for MITM attacks

---

## 🛡️ Defense & Mitigation
Common defenses against MAC Flooding include:

- Port Security (limit MAC addresses per port)
- Static MAC address binding
- Disabling unused switch ports
- Network monitoring and logging
- VLAN segmentation

When Port Security is properly configured, this attack is effectively blocked.

---

## 🔗 Relation to Other Attacks
MAC Flooding is rarely used alone.  
It is commonly used as a **preparation step** for:
- Sniffing
- ARP Spoofing
- Man-in-the-Middle (MITM) attacks

This makes Layer 2 security a critical foundation for overall network security.

---

## ⚖️ Legal Disclaimer
This project is intended **for educational purposes only**.
All experiments were conducted in an isolated laboratory environment.
Unauthorized use of these techniques on real networks is illegal.

---

## 📚 Educational Context
This project is part of a **Network Security Attacks Lab**, designed for students
studying Networks and Systems (Réseaux et Systèmes) and cybersecurity fundamentals.

---

