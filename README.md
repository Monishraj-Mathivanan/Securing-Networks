# **Network Security Assignment – Secure Network Design & IDS**  

## 📌 **Overview**  
This project demonstrates the **design, implementation, and security analysis** of a **multi-campus network** using **GNS3**. The assignment includes **firewall rule enforcement, VPN & BGP configuration, and intrusion detection system (IDS) deployment** to secure network communications and detect potential threats.  

## 🛠 **Key Components**  
- **🔹 Network Design & Implementation:** Secure topology across multiple campuses  
- **🔹 Firewall Rules & Security Hardening:** Access control & attack prevention  
- **🔹 BGP & VPN Configuration:** Secure inter-campus routing & encrypted traffic  
- **🔹 Intrusion Detection System (IDS):** Snort-based threat detection  
- **🔹 Attack Simulations & Security Analysis:** Testing firewall effectiveness  

## 🔍 **Setup & Configuration**  
### **1️⃣ Network Topology (GNS3 Simulation)**  
The network consists of:  
✅ **Clayton (Primary Data Center)** – Hosting internal & external services  
✅ **Caulfield & Peninsula Campuses** – Connected via **BGP & VPN**  
✅ **External Attacker Node** – Simulated attack scenarios  
✅ **DMZ Web Server** – External access with security controls  

### **2️⃣ Firewall Rules (Perimeter Security)**  
🚀 Implemented strict **IP filtering, access control, and packet inspection** for:  
✔ **Allowing DNS & Web traffic**  
✔ **Restricting SSH & mail access**  
✔ **Preventing unauthorized connections**  

### **3️⃣ IDS Implementation (Snort Rules)**  
🛡️ **Custom Snort rules** were created to detect:  
✔ **TCP Port Scans**  
✔ **SYN Flood DoS Attacks**  

Example Rule:  
```snort
alert tcp any any -> any any (msg: "TCP Port Scan Detected"; flags: S; sid:1000001; rev:1;)
```

## 🔥 **Security Analysis & Findings**  
✔ **Firewalls successfully blocked unauthorized traffic**  
✔ **IDS detected port scanning & DoS attempts in real-time**  
✔ **VPN tunnels secured communication between campuses**  
✔ **Ethical Network Usage Policy** drafted for compliance  

## 🚀 **Lessons Learned**  
🔹 **Importance of firewall rule enforcement** in preventing cyber attacks  
🔹 **Real-time monitoring with IDS** enhances network security  
🔹 **VPN & BGP improve secure inter-campus communication**  

## 📜 **References**  
📄 Full **assignment report** is available in this repository for further details.  

---

### ⚠ **Disclaimer**  
This project was conducted for **academic purposes only** as part of Monash University's **Network Security Assignment**. Unauthorized security testing on live systems is illegal.  

