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

- Setup Resources in Azure
- Ensure Connectivity between the client and Domain Controller
- Install Active Directory
- Create an Admin and Normal User Account in AD
- Join Client-1 to your domain (mydomain.com)
- Setup Remote Desktop for non-administrative users on Client-1
- Create a bunch of additional users and attempt to log into client-1 with one of the users

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/if9dTzg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To begin, first thing is to create your resources in azure. Creating a virtual machine named "DC-1" will automatically create a resource group and virtual network. Next, we will set domain controllers NIC Private IP address to be static.A second virtual machine called "client-1" will need to be made with the same reource group and virtual network making sure the vnet is the same.
</p>
<br />

<p>
<img src="https://i.imgur.com/9E28t92.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, we must ensure connectivity between the client and the domain controller.To test, we can first login into the domain controller and enable ICMPv4 on the local windows firewall.Go into command prompt and type in ping -t <ip address> and it should perpetually ping on the command prompt.
</p>
<br />

<p>
<img src="https://i.imgur.com/WnwmxVi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
