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

- Create a Resource Group
- Create a Windows 10 Virtual Machine (VM)
- Create a Linux (Ubuntu) VM
- Observe Your Virtual Network within Network Watcher

<h2>Deployment and Configuration Steps</h2>

<p>
  
  ![image](https://github.com/KevinVCruz26/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/139089937/ca8933fb-cb6f-4da2-b363-c1094d1966e4)
  
</p>
<p>
-In the search bar type in " resource group"

  -click on the +create tab

  ![image](https://github.com/KevinVCruz26/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/139089937/f1c13e9b-780e-4634-b124-a684e1772d23)

  -name the Resource group
  
  -Choose the Azure region that's right for you 
  
  -Then click on Reviwe + create


 <h1>Create a Windows 10 Virtual Machine (VM)</h1>

![image](https://github.com/KevinVCruz26/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/139089937/0a373329-68cf-4312-961b-616ecb5ba20f)


 -In the search bar type in "Virtual Machine"

 -click on +create tab

![image](https://github.com/KevinVCruz26/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/139089937/ebac7ed2-94d6-4f0d-acf0-d696e3f4af64)

-While creating the VM, select the previously created Resource Group

-Image is the base operating system or application for the VM, Click the down arrow and locate Widows 10

-While creating the VM, allow it to create a new Virtual Network (Vnet) and Subnet


<h1>Create a Linux (Ubuntu) VM</h1>

![image](https://github.com/KevinVCruz26/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/139089937/421b3d14-b8f3-4fc7-95de-6f9aa56c0f6b)

-While creating the VM, select the previously created Resource Group

-Image is the base operating system or application for the VM, Click the down arrow and locate Ubuntu

-While creating the VM, select the previously created Resource Group and Vnet

![image](https://github.com/KevinVCruz26/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/139089937/2bd0478a-f356-4f5c-a056-5f2abe54189b)

<h1>Observe Your Virtual Network within Network Watcher</h1>

![image](https://github.com/KevinVCruz26/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/139089937/4e26c257-0438-44ea-a6a9-b1afdf6a0092)

-In the search bar type in "Network Watcher"

-go to Diagnostic logs tab to see if both (Vm)s are there
