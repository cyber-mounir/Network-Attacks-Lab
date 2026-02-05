# MAC Flooding Attack

## Objective
Explain how MAC Flooding works and its impact on switched networks.

## Environment

The lab environment was built using the following components:

- **GNS3** – Network simulation platform  
- **Kali Linux** – Attacker machine used for traffic analysis  
- **Ubuntu Linux** – Victim machine generating network traffic  
- **Cisco Switch** – Layer 2 device used for packet forwarding

## Attack Description
MAC Flooding fills the switch CAM table with fake MAC addresses...

## Impact
- Switch behaves like a hub
- Traffic sniffing becomes possible

## Defense
- Port Security
- MAC address limiting
