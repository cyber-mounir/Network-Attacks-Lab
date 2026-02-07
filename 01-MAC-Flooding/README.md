# MAC Flooding Attack

## 📌 Objective
The goal of this project is to study the MAC Flooding attack and understand
its impact on switched networks in a controlled lab environment.

## 🧪 Lab Environment
- GNS3
- Kali Linux (Attacker)
- Ubuntu Linux (Victim)
- Layer 2 Switch
- Router (Gateway)

## 🧠 Attack Overview
MAC Flooding is a Layer 2 attack where an attacker sends a large number of
fake MAC addresses to a switch. This causes the switch CAM table to overflow.

When the CAM table is full, the switch starts broadcasting frames to all ports,
behaving like a hub instead of a switch.

## ⚠️ Impact
- Loss of switch efficiency
- Traffic flooding
- Enables packet sniffing
- Prepares the network for MITM attacks

## 🛡️ Defense
- Port Security
- Limiting MAC addresses per port
- Network monitoring

## 🔗 Relation to Next Attacks
MAC Flooding is often used as a preparation step for:
- Sniffing
- ARP Spoofing
- Man-in-the-Middle (MITM)

## ⚖️ Legal Notice
This project was conducted in a closed lab environment for educational purposes only.
