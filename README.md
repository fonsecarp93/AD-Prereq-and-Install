# AD-Prereq-and-Install
These are the steps needed to create your active directory and begin creating users.

# Active Directory Prerequisites

<p align="center">
<img src="https://i.imgur.com/Aw0e5rl.png" alt="osTicket logo"/>
</p>

<h1>Active Directory - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Active Directory Domain Services
-

h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)
- Windows Server 2022

<h2>Installation Steps</h2>
 1.) Create a Domain Controller Virtual Machine (Windows Server 2022) and set the DC's NIC Private IP address to static
<p></p>Take note of your Resource group and Virtual Network that are created. They will be used again.
<img src="https://i.imgur.com/jpeAVJZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/dh9bOvY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

 2.) Create the Client Virtual Machine (Windows 10) in the same Resource group and Virtual Network as the Domain Controller.
   Note: Ensure both of the Virtual Machines are in the same Virtual Network within the Network Watcher)

<img src="https://i.imgur.com/46kSGU0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/KCk7qE5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

3.)  Establish connectivity between the Client and Domain Controller by enabling the ICMPv4 within the Domain Controller's local firewall.
<p></p>
Ensure connectivity is established by pinging the DC's private IP address from within the Client's local command prompt.
<p> 
<img src="https://i.imgur.com/WJrSGc4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/mnF7nxC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
4.) Within the Domain Controller VM, install Active Directory Domain Services.
</p>
<img src="https://i.imgur.com/KNQgoKt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
</p>

5.) Promote the same Virtual Machine as a DC: Set up a forest as mydomain.com

<img src="https://i.imgur.com/fTbn8PV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

6.)Restart then log back into DC-1 as mydomain.com/username
<p>Note: When installation is successful, the remote desktop will restart.
 
<img src="https://i.imgur.com/KNQgoKt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/KREI53A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<br />
