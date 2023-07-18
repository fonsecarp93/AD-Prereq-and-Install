# AD-Prereq-and-Install
These are the steps needed to create your active directory and begin creating users.

# osticket-prereqs

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

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

 2.) Create the Client Virtual Machine (Windows 10) in the same Resource group and Virtual Network as the Domain Controller.
   Note: Ensure both of the Virtual Machines are in the same Virtual Network within the Network Watcher)


3.)  Establish connectivity between the Client and Domain Controller by enabling the ICMPv4 within the Domain Controller's local firewall.
<p></p>
Ensure connectivity is established by pinging the DC's private IP address from within the Client's local command prompt.
<p> 

4.) Within the Domain Controller VM, install Active Directory Domain Services.
</p>
    <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>

</p>
<br />
