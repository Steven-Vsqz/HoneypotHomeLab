# 🌍 Failed RDP to IP Geolocation Tracking

This project demonstrates how to **detect failed Remote Desktop Protocol (RDP) brute-force attacks**, extract log data via **PowerShell**, and **map attacker IP geolocation** using **Azure Sentinel** and a third-party API.

A custom honeypot virtual machine (VM) was configured in **Microsoft Azure**, monitored in real-time via **Sentinel (SIEM)**. Detected attacks were analyzed using a **custom PowerShell script** that gathered geolocation data from external APIs, visualized live on a world map.

---

## 📸 Demo Snapshots

<p align="center">
  <b>📌 Brute Force RDP Attempt (Recorded)</b><br>
  <img src="https://i.imgur.com/oArZdLj.png" width="80%" alt="RDP Attempt Screenshot" />
  <br><br>
  <b>📌 Real-time PowerShell Log Output</b><br>
  <img src="https://i.imgur.com/h9Qv34B.png" width="80%" alt="PowerShell Output Screenshot" />
  <br><br>
  <b>📌 Azure Sentinel World Map of Attack Sources</b><br>
  <img src="https://i.imgur.com/BJ3JpNh.png" width="80%" alt="Sentinel Map Screenshot" />
</p>

---

## 🛠️ Tools & Technologies Used

- 🧠 **Microsoft Azure** – Hosted Sentinel on a live VM honeypot  
- 💻 **PowerShell** – Parsed Windows Event Logs for failed RDP attempts  
- 🌐 [**ipgeolocation.io**](https://ipgeolocation.io/) – Converted attacker IPs to geolocation info

---

## 🧪 Environment

- 🖥️ Windows 10 (Honeypot VM)

---

## 🔍 What I Did

1. ✅ Created a **free-tier Azure account** and deployed a **Windows 10 VM**  
2. 🧲 Configured the VM as a **honeypot** to lure attackers via exposed RDP  
3. 🛡️ Connected the VM to **Azure Sentinel** for centralized log collection  
4. 📜 Wrote a **PowerShell script** to extract failed RDP login attempts from Event Viewer  
5. 🌍 Queried the **ipgeolocation.io API** to map attacker origin by IP  
6. 📈 Sent the geolocation data into **Sentinel** for **visual map-based analysis**  

---

## 🎯 Project Purpose

This project simulates a **real-world SOC workflow** involving:

- RDP brute-force detection  
- IP-to-location correlation  
- SIEM-based threat mapping  
- Custom script automation

It highlights how SIEMs and scripts can be combined for **threat intelligence**, **geospatial visualization**, and **alert triage** in cybersecurity operations.

---

## 📷 Original Visualization

<p align="center">
  <img src="https://i.imgur.com/VHxkSKa.png" width="80%" alt="Full Process Overview" />
</p>
