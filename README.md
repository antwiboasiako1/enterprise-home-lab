# 🏢 Active Directory Domain Controller Lab

This lab simulates a real-world enterprise setup by configuring a **Windows Server 2019 Domain Controller (DC)** and joining a **Windows 10 client** to the `corp.local` Active Directory domain. It’s part of the larger [enterprise-home-lab](https://github.com/antwiboasiako1/enterprise-home-lab) series that includes pfSense, Snort IDS, Splunk SIEM, Cortex XSOAR, and more.

---

## 🧩 Lab Overview

| Component       | Configuration                          |
|----------------|-----------------------------------------|
| Domain Name     | `corp.local`                            |
| DC IP Address   | `192.168.56.10`                         |
| Win10 Client IP | `192.168.56.11`                         |
| Network Mode    | Host-only Adapter (vboxnet)             |

---

## 🛠️ Tools & Technologies

- 🖥️ **Windows Server 2019**
- 💻 **Windows 10 Pro**
- 📡 **Active Directory Domain Services (AD DS)**
- 🌐 **DNS Role Configuration**
- 🛜 **Static IP Setup**
- ⚙️ **PowerShell / nslookup / ping**

---

## 🧪 Step-by-Step Setup

| Step | Description |
|------|-------------|
| ✅ 1 | Installed **Active Directory Domain Services (AD DS)** role on Windows Server |
| ✅ 2 | Installed **DNS Server** role |
| ✅ 3 | Promoted server to Domain Controller (`corp.local`) |
| ✅ 4 | Verified DNS zone and service records using PowerShell |
| ✅ 5 | Set **static IP** on both Server and Win10 client |
| ✅ 6 | Tested DNS with `nslookup` and `ping` |
| ✅ 7 | Joined Windows 10 client to the domain successfully |
| ✅ 8 | Logged in with domain credentials and confirmed domain trust |

---

## 🖼️ Screenshots

These are included in the repo for visual reference:

1. `1_install_ad_ds_role.png`  
2. `2_install_dns_role.png`  
3. `3_install_addsforest.png`  
4. `4_reboot_after_promotion.png`  
5. `5_powershell_dns_zone_check.png`  
6. `6_static_ip_win10_client.png`  
7. `7_firewall_fix_command.png`  
8. `8_static_ip_config.png`  
9. `9_ipconfig_dns_settings.png`  
10. `10_nslookup_ping_success.png`  
11. `11_domain_join_dialog.png`  
12. `12_domain_join_success.png`  
13. `13_after_login_win10_domain.png`  

---

## ✅ Outcome

- Windows 10 client successfully joined `corp.local` domain
- Name resolution via DNS confirmed using `nslookup`
- Active Directory & DNS roles working on internal enterprise subnet

---

## 📁 Part of Larger Project

This is **Project 3** in the `enterprise-home-lab` series:
- 🔐 [Project 1: pfSense + Snort IDS](https://github.com/antwiboasiako1/enterprise-home-lab)
- 📨 [Project 2: Automated Phishing Response (Splunk + Cortex XSOAR)](https://github.com/antwiboasiako1/enterprise-home-lab)
- 🧑‍💼 **Project 3: Active Directory Domain Controller**

---

## 💬 Author

**David Antwi**  
[GitHub](https://github.com/antwiboasiako1) • [LinkedIn](https://www.linkedin.com/in/david-antwi-408907149)

---

