<h1>Cyber Threat Intelligence: SOC Alert Analysis</h1>


<h2>Description</h2>
This project, conducted during my internship at CYBLACK x LetsDefend SOC Academy, focuses on the integration and analysis of Cyber Threat Intelligence (CTI) within Security Operations Center (SOC) environments. The aim was to enhance incident response capabilities by evaluating SOC alerts and their associated threat intelligence.

Throughout the internship, I explored various SOC alert scenarios, dissecting them to understand their implications and potential responses. By leveraging CTI, I aimed to improve threat detection and mitigation strategies, providing valuable insights into how organizations can bolster their cybersecurity posture.




<h2>Organization</h2>
- <b>CYBLACK</b>

<h2>Utilities Used</h2>

- <b>AnyRun</b>
- <b>VirusTotal</b>
- <b>Talos</b>

<h2>Environments Used </h2>

- <b>LetsDefend</b>


<h2>Program walk-through:</h2>

<p align="center">
Incident Alert: <br/>
<img src="https://i.imgur.com/NX2pqVV.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h2>Understanding the Alert:</h2>
The alert suggest that this event was triggered because of a request to a (TI) flagged URL. The URL seems to be a shortened link, which can be marked suspicious or malicious.
<br />
<br />

Create a Case for the event:  <br/>
<img src="https://i.imgur.com/ft4tDFD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/yejawwC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
First we'll use ANYRUN to run analysis on the URL to determine if it is malicious: <br/>
<img src="https://i.imgur.com/S1ONzV1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/fiJcTnJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/ptm1yrs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/RvNtSQt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/piJh8WI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Next we'll check the destination IP address for any IOC:  <br/>
<img src="https://i.imgur.com/JLJRr9q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

From this Analysis we can conclude that the URL and Destination IP address are not malicious. No vendors has flagged the IP address as being a malicious one.

Next we'll add Artifacts and  create Analysis Note for our findings
<img src="https://i.imgur.com/oXTKBxN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/pr7G8E5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Then we can close the alert:  <br/>
<img src="https://i.imgur.com/zfHEAof.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/DInoDhe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<h2>Conclusion:</h2>
In this project, I identified that the SOC alerts was false positive. This highlights the need for thorough analysis in cybersecurity operations to improve threat detection and ensure efficient resource allocation.
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
