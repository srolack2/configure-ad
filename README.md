<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1: Setting Up Resources in Azure (Create the Domain Controller VM)
- Step 2: Ensure Connectivity Between the Client and Domain Controller
- Step 3: Install Active Directory
- Step 4: Creating Admin and Normal User Accounts

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/K98HslW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<h2>Setup Resources in Azure</h2>
<ul> 
  <li> Create the Domain Controller VM (Windows Server 2022) named “DC-1” </li>
  <li> Set Domain Controller’s NIC Private IP address to be static </li>
  <li> Create the Client VM (Windows 10) named “Client-1”. Note: Use the same Resource Group and Vnet that was created in Step 1 </li>
  <li> Ensure that both VMs are in the same Vnet (you can check the topology with Network Watcher) </li>
</ul>

<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<h2> Ensure Connectivity between the client and Domain Controller </h2>
<ul>
  <li>Login to Client-1 with Remote Desktop and ping DC-1’s private IP address with ping -t <ip address> (perpetual ping) </li>
  <li>Login to the Domain Controller and enable ICMPv4 in on the local windows Firewall </li>
  <li>Check back at Client-1 to see the ping succeed </li>
</ul>
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
