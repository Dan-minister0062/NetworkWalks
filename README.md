# 🔐 Cybersecurity & Penetration Testing Lab Setup
## 📌 Project Overview
This project involves setting up a virtual cybersecurity laboratory using **Oracle VirtualBox and Kali Linux**. The lab provides a controlled environment for learning cybersecurity, network reconnaissance, vulnerability assessment, and authorized penetration testing.
## 🎯 Project Objectives
- Install and configure VirtualBox.
- Set up Kali Linux as the primary security machine.
- Create a private NAT Network for virtual machines.
- Configure IP addressing, gateway, and DNS.
- Test network connectivity.
- Create a VM snapshot for system recovery.
- Prepare the environment for future penetration-testing exercises.
## ⚙️ Lab Configuration
| Component | Configuration |
|---|---|
| Host OS | Windows 10 |
| Hypervisor | VirtualBox 7.2 |
| Security OS | Kali Linux 2026.2 |
| Allocated RAM | 2048 MB |
| Network Type | NAT Network |
| Network Name | NatNetwork |
| Network Range | 10.0.0.0/24 |
| Kali IP Address | 10.0.0.2 |
| Gateway | 10.0.0.1 |
| DNS | 10.0.0.1 |
## 🛠️ Tools Used
- Oracle VirtualBox
- Kali Linux
- 7-Zip
- NetworkManager
- Nmap
## 🔎 Network Verification
The following commands are used to verify the laboratory configuration:
```bash
ip a
ip route
ping -c 4 10.0.0.1
ping -c 4 8.8.8.8
nslookup google.com
nmap --version
```
## 🐞 Challenges & Solutions
**Network Configuration:** Adjusted the Kali Linux NetworkManager connection settings during network troubleshooting.
Command used:
```bash
sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
```
**Virtualization Error:** Enabled Intel VT-x hardware virtualization through BIOS/UEFI to allow VirtualBox to run virtual machines.
## 📚 What I Learned
- Virtualization and virtual machine management.
- NAT Network configuration.
- IPv4 addressing, gateways, and DNS.
- Linux network administration.
- Network troubleshooting.
- Virtual machine snapshots and recovery.
## 🚀 Future Improvements
- Add vulnerable target machines.
- Practice network scanning with Nmap.
- Perform web application security testing with Burp Suite.
- Practice vulnerability assessment.
- Explore Wireshark, Metasploit, and Wazuh.
## 🔐 Security Disclaimer
This laboratory is designed for educational purposes and authorized security testing only. All testing activities will be performed on systems owned by me or for which I have explicit permission.
## 👨‍💻 Author
Name:Ibrahim Idris Ibrahim 
Project: Cybersecurity & Penetration Testing Lab Setup  
Environment: VirtualBox & Kali Linux

**Project Status:** Initial Lab Setup Completed
