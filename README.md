<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Set Up Domain Controller
- Create Resource Group, Virtual Network/Subnet, Then Create Domain Controller
- Set the Domain Controller's NIC Private IP address to be static.
- Step 4

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://github.com/user-attachments/assets/02373e16-e996-4b19-9d19-39f0de23ee7c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
As you can see here, my Virtual Network, Active-Directory-vnet, has been set up and deployed successfully. Following this set-up and deployment, I then went in to create my Virtual Machine.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/923439fc-a81f-47fa-ae04-7410ac828fc2" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here is where I have opened the IP Configuration settings for the Domain Controller and have set the Private NIC IP Address to Static. 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/566e7358-feab-428f-98a9-7e97e44f4b4f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here shows that I am logged into CLient-1, the second Virtual Machine I created within Azure, and I have pinged '10.0.0.4' which is the private IP address for my Domain Controller. The ping in Powershell shows that the IP Address was set up to Client-1 correctly and also shows the DNS servers as Domain Controller-1.
</p>
<br />
