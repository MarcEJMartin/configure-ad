<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com/playlist?list=PLAnyL2H5UDKJMvD8S6Tw0vygNQYxSWuRe)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Install Active Directory Domain Services on DC-1, promote it to a Domain Controller with a new forest (e.g., mydomain.com), and log in using domain credentials.
- Create Organizational Units (_EMPLOYEES and _ADMINS) in Active Directory and add a new Domain Admin user jane_admin to the “Domain Admins” group.
- Log in as jane_admin and use it as the main admin account going forward for managing your domain environment.
- Join Client-1 to the domain by logging in as the local admin, connecting it to mydomain.com, restarting it, and moving it into a new “_CLIENTS” Organizational Unit in Active Directory Users & Computers.
- Enable Remote Desktop access for Domain Users on Client-1 to allow non-administrative users to log in remotely.
- Use a PowerShell script on DC-1 to create multiple employee accounts in the “_EMPLOYEES” OU and test login with one of the new user accounts on Client-1.
- Verify that all newly created user accounts appear in Active Directory, and confirm successful domain logins and access permissions on Client-1.
  
<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To begin configuring your on-premises Active Directory infrastructure, log into the DC-1 virtual machine and install the Active Directory Domain Services (AD DS) role. After installation, promote the server to a Domain Controller by creating a new forest (e.g., mydomain.com). Once the server restarts, you can log in using your domain credentials (e.g., mydomain.com\labuser) to manage your new AD environment.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
L
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
