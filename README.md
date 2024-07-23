<h1>Failed RDP to IP Geolocation Information</h1>

The PowerShell script in this repository is designed to extract information from Windows Event Logs regarding failed Remote Desktop Protocol (RDP) attacks. It then uses a third-party API to gather geographic details about the attacker's location.
<br />
<br />
In this demonstration, I configure <strong>Azure Sentinel (SIEM)</strong> and link it to a live virtual machine functioning as a honeypot. We will monitor real-time RDP brute force attacks originating from various global locations. By using a custom PowerShell script, we can retrieve the attackers' geolocation information and display it on an Azure Sentinel map.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Microsoft Azure: Setup Sentinel on a honeypot virtual machine</b>
- <b>PowerShell: Extract RDP failed logon logs from Windows Event Viewer</b> 
- <b>ipgeolocation.io: IP Address to Geolocation API</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>

<h2>Program walk-through:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
