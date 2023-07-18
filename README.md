<h1>Vulnerability Analysis, Management and Remediation</h1>

<h2>Description</h2>
This Project will use a virtual machine to show how to manage and remediate vulnerabilities and assets using Nessus Essentials on Windows 10. Vulnerability Management is a huge part of Cyber Security and this project will show you why.
<br />


<h2>Programs and Utilities Used</h2>

- <b>VMWare</b> 
- <b>Windows 10</b>
- <b>Nessus Essentials</b> 

<h2>Environments Used </h2>

- <b>Windows 10 on both Virtual Machine and Host machine</b> (21H2)

<h2>Lab Overvoew:</h2>

<p align="center">
  [Quick Note: After I installed the Virtual Machine with a Windows 10 iso I made sure to bridge the VM and my host machine together so that they could communicate easier for the sake of demonstration. I HIGHLY recommend NOT doing this at home because it can compromise security for your system if not done correctly.]
  
After installing the VM and briding the networks, it's time to conduct our first basic network scan. We used no credentials and are essentially limited in scope. I chose the name Windows 10 Single Host and inserted the VM's IP address because that is what we will be analyzing. <br/>
<img src="https://i.imgur.com/t8AC1sE.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/5tqMOzg.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The results of our first scan are a success albeit barebones. Also note that you can check the scan whilst it is ongoing. It is reassuring that not much is happening. We receive feedback of mostly low and info-related vulnerabilities that can easily be fixed.  <br/>
<img src="https://i.imgur.com/uvz9WWg.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/7YCVTzA.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
This wouldn't be much of a lab if we stopped here so let's have some fun and BASICALLY BREAK MY VIRTUAL MACHINE. In order to get some more vulnerabilities I decided to remove the firewall, mess with user account settings, the registry and allow much more alarming traffic into the network.. you know... for the sake of science. <br/>
<img src="https://i.imgur.com/Gq2jp1t.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/VLfFKay.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/qkX6LYc.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Before you go thinking I'm some kind of masochist or dummy or something, it should be noted that: 1. I'm doing for demonstration. 2. Tenable (the creators of Nessus Essentials) actually have posts on their site explaining ways to test their practice with step by step walkthroughs on how to do so. You can find it here https://community.tenable.com/s/article/Scanning-with-non-default-Windows-Administrator-Account  <br/>
<img src="https://i.imgur.com/iWeU8Zd.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/cXuPltX.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
With all of that BORING stuff out of the way, we can get back to the real fun... scanning for weaknesses in our system! This time we will run a scan with credentials. We use the username and password from our VM to do this. This will allow us to run a deeper and more robust scan! YAY!  <br/>
<img src="https://i.imgur.com/yHDYIge.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wow.. would you look at that. Critical alerts...gee... who would've thought? Nessus Essentials is great because the dashboard shows you more than just the raw data of the scan. It provides you with pie charts, ways to sort vulnerabilities and even ways to remediate them! Clicking on one even shows a description on what exactly it is and the steps to cure it.  <br/>
<img src="https://i.imgur.com/bwZvgAW.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/NCaV3gc.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/TkvnbmP.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Thankfully we can remediate these vulnerabilities because we're super smart experts. If I've learned anything about Cybersecurity from all my studying, practice and real world applicating it's that we should probably just listen to our program and just run some updates and let windows fix this for us :). Notice how after something as simple as updating Windows, many of these problems just... go away. This is because old software has many holes to expose and it is in best practice to make sure things are ALWAYS up to date, secure and remediated immediately! Hope you enjoyed my TEDxTALK.. I Know I did.  <br/>
<img src="https://i.imgur.com/nWoepzg.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Cxm849C.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
