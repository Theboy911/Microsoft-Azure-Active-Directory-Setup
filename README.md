# Microsoft-Azure-Active-Directory-Setup
Microsoft Azure Active Directory Setup
<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- 1.) Create Microsoft azure account and VM's
- 2.) Install Active directory
- 3.) Create Admin acccount
- 4.) Join client machine to AD forrest.
- 5.) Create Users 

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/sX33sgm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This lab begins with creating a microsoft Azure account. There is usually a free tier for the first month of use which we'd like to take advantage of if not then it should be relatively cheap to finish the lab and then delete. Once an active Azure account has been created you must then navigate to or search for "create a resource group". ONce there name the resource group whatever you would like but take note of whatever you decide. Be sure to pick a region according to wherever you live. 
</p>
<br />

<p>
<img src="https://i.imgur.com/k7SMw9p.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once your resource group has been succesfully created you will then create 2 virtual machines with that same resource group, so essentially this step will be completed twice. The first machine you create should be the domain controller for your active directroy service which is basically a server that will host all of your accounts and information and allow for expedited and closed communication within an enterprise environment. When creating the domain controller be sure to also take note of the virtual network, you will want the virtual networks to be the same for this lab to ensure communication is possible between the two machines. Also be sure to pick the applicable operating systems in the drop downs to for the vm you are creating. Domain controller = Windows Server 2022 and Client Machine = Windows 10. Be sure to take note of the username and password that you used when creating your virtual machines as you will use this to RDP into your VM's. 
</p>
<br />

<p>
<img src="https://i.imgur.com/GdvEA0u.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This step is essentially redundant as we can just next through this page but it is important to just make sure that our virtual networks are the same. 
</p>
<br />

<p>
<img src="https://i.imgur.com/gctcYeG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once both vms have been succesfully created it is now time to log into both of them using RDP or remote desktop protocol. When logging into your machines be sure to use the public IP address not the private as there is no way for RDP to differentiate between the many private IP addresses on the internet. 
</p>
<br />

<p>
<img src="https://i.imgur.com/1p8Ug7u.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/aKTFVgF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/VIwz922.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/SygvKje.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/Qy0qWh9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/sZHhkk4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
