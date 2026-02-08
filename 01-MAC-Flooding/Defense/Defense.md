# Defense Against MAC Flooding Attack

## 1️⃣ Security Objective
The primary objective of defending against MAC Flooding is to protect the
switch CAM table from overflow and ensure that the switch continues to forward
frames securely and efficiently.

Effective defense mechanisms prevent the switch from behaving like a hub and
preserve traffic confidentiality.

---

## 2️⃣ Port Security (Primary Defense)

### Description
Port Security is a Layer 2 security feature available on managed switches.
It allows administrators to control which MAC addresses are permitted on a
specific switch port.

### How It Mitigates MAC Flooding
- Limits the number of MAC addresses learned per port
- Prevents excessive MAC address learning
- Blocks spoofed or unauthorized MAC addresses
- Protects the CAM table from overflow

### Violation Modes
- **Protect**: Drops frames from unknown MAC addresses
- **Restrict**: Drops frames and generates alerts/logs
- **Shutdown**: Disables the port when a violation occurs

Port Security is the most effective and widely used defense against MAC Flooding.

---

## 3️⃣ Static MAC Address Binding

### Description
Static MAC binding manually associates a known MAC address with a specific
switch port.

### Security Benefit
- Only trusted devices are allowed to communicate
- Eliminates MAC address learning abuse

### Limitation
This method is suitable for small or high-security environments due to
administrative overhead.

---

## 4️⃣ Disable Unused Switch Ports

### Description
Unused switch ports should be administratively disabled.

### Security Benefit
- Prevents attackers from connecting rogue devices
- Reduces the overall attack surface of the network

This is considered a basic but essential security best practice.

---

## 5️⃣ Network Monitoring and Logging

### Description
Continuous monitoring helps detect abnormal switch behavior caused by MAC
Flooding attacks.

### Indicators of Attack
- Rapid increase in learned MAC addresses
- Excessive broadcast traffic
- Switch performance degradation

### Tools
- Syslog
- SNMP
- Network monitoring systems

---

## 6️⃣ VLAN Segmentation (Supporting Defense)

### Description
VLANs divide the network into smaller broadcast domains.

### Security Benefit
- Limits the scope of MAC Flooding attacks
- Reduces the impact on the entire network
- Improves overall network isolation

---

## 7️⃣ Expert Insight
MAC Flooding is rarely used as a standalone attack.
Its primary role is to weaken Layer 2 defenses and enable traffic interception
and more advanced attacks such as ARP Spoofing and MITM.

Implementing Port Security at access layer switches effectively stops the attack
at an early stage.

---

## 8️⃣ Summary
Defending against MAC Flooding requires a combination of:
- Port Security
- Proper switch configuration
- Continuous monitoring
- Network segmentation

Layer 2 security is the foundation of secure network infrastructure, and
protecting the CAM table is a critical first step.

---
