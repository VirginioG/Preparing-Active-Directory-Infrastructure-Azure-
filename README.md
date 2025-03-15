<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
In this tutorial, you'll set up a Domain Controller (DC) and a Client Virtual Machine (VM) in Azure, where the Domain Controller serves as the DNS server for the Client VM. You'll also configure basic network settings, Active Directory, and ensure proper DNS resolution for seamless communication between both machines.<br />


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

- Begin by creating a Resource Group to organize your resources effectively. Then, set up a Virtual Network (VNet) with an appropriate address space, and configure a subnet for connectivity between the Domain Controller and Client VM.
- Create a Windows Server 2022 virtual machine (VM) named DC-1 within the same resource group and VNet. Configure the VM with necessary admin credentials, and assign a static private IP to the network interface card (NIC) to ensure consistent addressability.
- Connect to the DC-1 VM using Remote Desktop (RDP). Disable the Windows Firewall temporarily on DC-1 to facilitate testing of network connectivity and rule out firewall restrictions.
- In the Azure portal, deploy a Windows 10 VM named Client-1 in the same region and VNet as DC-1. Ensure that Client-1’s DNS settings point to the private IP address of DC-1 to use the Domain Controller as the DNS server.
- After restarting Client-1, perform a ping to DC-1’s IP address to verify network connectivity. Then, run ipconfig /all on Client-1 to ensure the DNS server is correctly configured to point to DC-1’s static IP, confirming proper name resolution.

<h2>Deployment and Configuration Steps</h2>

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
