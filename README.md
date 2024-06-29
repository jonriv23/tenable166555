<p align="center">
<img src="https://github.com/jonriv23/tenable166555/assets/143762386/b3cf6f42-dcf5-4058-adb8-15c755e004f3">
</p>

<h1>Tenable Vulnerability - Plugin ID 166555</h1>
Tenable Vulnerability Remediation

<h3>Technologies Used</h3>
- Tenable Nessus<br>
- Powershell<br>
- Registry Editor<br>
- Microsoft Windows
- NinjaOne

<h3>Tenable Scan</h3>
Tenable was used to scan multiple PC's for vulnerabilities. After Tenable's scan completed, results showed WinVerifyTrust Plugin 166555 to be one of the top vulnerabilities. <br>
<img src = "https://github.com/jonriv23/tenable166555/assets/143762386/3d4eda84-920d-4900-acde-fe918d202070">
<br>Next step is remediation. Solution can be found here: (https://www.tenable.com/plugins/nessus/166555)

<h3>Registry Editor</h3>
I checked the solution path within the Registry Editor to further understand the situtation. Sure enough, the Registry key was missing. 

<h3>Powershell</h3>
Since there were multiple devices with the same vulnerability I went ahead and created a Powershell script to add the missing folder and value key to the Registry. 
<img src = "https://github.com/jonriv23/tenable166555/assets/143762386/b4da2bb0-20b0-4041-a5c3-20dfcff3f971">
Powershell script successfully ran.<br>
I once again checked the path inside the Registry and confimred the key was now there.

<h3>NinjaOne</h3>
Once confirming the script was successful, I used the endpoint manager NinjaOne to automate the remaining vulnerable PCs.
<img src = "https://github.com/jonriv23/tenable166555/assets/143762386/c682b441-e370-4a5b-8587-0986024f8afe">

<h3>Results</h3>
After remediation, the vulnerability no longer appeared on Tenable's scan.<br>






