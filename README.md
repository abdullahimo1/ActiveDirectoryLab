<h1>Active Directory Lab</h1>

<h2>Description</h2>

This Active Directory (AD) home lab demonstrates how an enterprise domain infrastructure is built and managed using Windows Server 2019 and Windows 10 clients within a virtualized network (VMware Workstation).
The goal of the lab is to simulate a realistic corporate environment for user authentication, resource management, and centralized policy control—core functions of any modern IT network.

<h2>Key objectives</h2>

- Install and configure Active Directory Domain Services (AD DS).
- Deploy and configure DHCP to automate IP address management.
- Implement Routing and Remote Access (RRAS) to enable connectivity between internal and external networks.
- Use PowerShell automation to create multiple users efficiently.
- Integrate network services such as DNS, Group Policy, and Organizational Units (OUs).
<br />

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Windows Server</b> (2019)

<h2>Languages Used</h2>

- <b>PowerShell</b>
<h2>Program walk-through:</h2>

<p>
<b>🧩 AD Installation</b><br/>
This screenshot displays the <b>Server Manager – Add Roles and Features Wizard</b>, where the 
<b>Active Directory Domain Services (AD DS)</b> role is being installed. 
This installation is a key step in transforming the Windows Server into a <b>Domain Controller</b>, 
enabling centralized authentication, user management, and domain-wide policy control.
</p>
<p align="center">
  <img src="https://i.imgur.com/WYDdXxU.png" alt="Active Directory Installation" width="80%" height="80%">
</p>

<p>
<b>DHCP Configuration</b><br/>
This Screenshot displays the DHCP Management Console, where the IPv4 scope is defined (172.16.0.100–172.16.0.200).
</p>
<p align="center">
  <img src="https://i.imgur.com/j5LPDwE.png" alt="Active Directory Installation" width="80%" height="80%">
</p>

<p>
<b>Routing and Remote Access Configuration</b><br/>
Routing and Remote Access has been enabled on the domain controller.
It allows the server to route network traffic between multiple subnets or virtual networks.
This is crucial for enabling internal communication between the domain controller, clients, and possibly external networks.
</p>
<p align="center">
  <img src="https://i.imgur.com/j5LPDwE.png" alt="Active Directory Installation" width="80%" height="80%">
</p>

<p>
<b>PowerShell User Creation Scriptn</b><br/>
This PowerShell ISE script automates the creation of user accounts in Active Directory.
</p>
<p align="center">
  <img src="https://i.imgur.com/xD0z22M.png" alt="Active Directory Installation" width="80%" height="80%">
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
