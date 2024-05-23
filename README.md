<h1>Pi-Hole</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
Project consists of a simple PowerShell script that walks the user through "zeroing out" (wiping) any drives that are connected to the system. The utility allows you to select the target disk and choose the number of passes that are performed. The PowerShell script will configure a diskpart script file based on the user's selections and then launch Diskpart to perform the disk sanitization.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Ubuntu Terminal</b> 
- <b>Pi-Hole</b>

<h2>Environments Used </h2>

- <b>Windows 11 VM</b> (the device to monitor)
- <b>Ubuntu 22.14 VM</b> 

<h2>Program walk-through:</h2>

<p align="center">
Step 1: Updating repositories and libraries <br/>
<img src="https://i.imgur.com/RIA2Tmj.png" height="80%" width="80% alt="Pi-Hole steps"/>
<br />
<br />
Step 2: Changing the IP address to Static  <br/>
<img src="https://i.imgur.com/K0Ikpv0.png" height="80%" width="80%" alt="Pi-Hole steps"/>
<br />
<br />
Step 3: sudo nano /etc/netplan/00-installer-config.yaml <br/>
<img src="https://i.imgur.com/JCSj5aZ.png" height="80%" width="80%" alt="Pi-Hole steps"/>
<br />
<br />
Step 4: sudo netplan apply (This will give us many warnings as we’re making our IP static)  <br/>
<img src="https://i.imgur.com/dqJlWrI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
As per below image, the IP has been changed and it is now static  <br/>
<img src="https://i.imgur.com/AOi74kF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
