<h1>Azure Sentinel : Live Attack</h1>


<h2>Description</h2>
I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot. We will observe live attacks (RDP Brute Force) from all around the world. We will use a custom PowerShell script to look up the attackers Geolocation information and plot it on the Azure Sentinel Map!
<br />


<h2>Environments, Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Microsoft Azure</b>
- <b>Azure Sentinel</b>
- <b>Log Analytics Workspaces</b>
- <b>Windows 11</b> (21H2)


<h2>Program walk-through:</h2>

<h3>Deploay Virtual Machine</h3>

<p align="left">
 
- Create an account on Microsoft  Azure
- Deploy a Windows 11 Virtual Machine and assign requisite resources: https://portal.azure.com/
- Create a Security to allow all traffic inbound
 
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 
<h3>Setup Log Analyitics Workspaces</h3>
- The Purpose of this is to ingest logs from the VM into the analytics space
- THE SIEM (Azure Sentinel) will connect to this work Space to dispay the GEO data on the Map<br/>


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
