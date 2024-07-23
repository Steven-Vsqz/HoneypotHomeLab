<h1>Failed RDP to IP Geolocation Information</h1>

The PowerShell script in this repository is designed to extract information from Windows Event Logs regarding failed Remote Desktop Protocol (RDP) attacks. It then uses a third-party API to gather geographic details about the attacker's location.
<br />
<br />
In this demonstration, I configure <strong>Azure Sentinel (SIEM)</strong> and link it to a live virtual machine functioning as a honeypot. We will monitor real-time RDP brute force attacks originating from various global locations. By using a custom PowerShell script, we can retrieve the attackers' geolocation information and display it on an Azure Sentinel map.
<br />
<br />
<p align="center">
<img src="https://i.imgur.com/VHxkSKa.png" height="80%" width="80%" alt="Failed RDP Steps"/>
</p>

<h2>Languages and Utilities Used</h2>

- <b>Microsoft Azure: Setup Sentinel on a honeypot virtual machine</b>
- <b>PowerShell: Extract RDP failed logon logs from Windows Event Viewer</b> 
- <b><a href="https://ipgeolocation.io/">ipgeolocation.io</a>: IP Address to Geolocation API</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>

<h2>Overview</h2>

After creating a free Microsoft Azure account, I set up a live virtual machine configured as a honeypot to attract attackers. I implemented Azure Sentinel (SIEM) to monitor and map the global locations of these attacks using the third-party API ipgeolocation.io. A custom PowerShell script was utilized to collect the attackers' geolocation information, log it in a .txt file, and input the data into Sentinel for visual mapping.

<h1 align="center">
Recorded Brute Force RDP attempt: <br/>
<img src="https://i.imgur.com/oArZdLj.png" height="80%" width="80%" alt="Failed RDP Steps"/>
<br />
<br />
Real-time failed RDP in powershell: <br/>
<img src="https://i.imgur.com/h9Qv34B.png" height="80%" width="80%" alt="Failed RDP Steps"/>
<br />
<br />
World map of incoming attacks:  <br/>
<img src="https://i.imgur.com/BJ3JpNh.png" height="80%" width="80%" alt="Failed RDP Steps"/>
<br />
<br />
</h1>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
