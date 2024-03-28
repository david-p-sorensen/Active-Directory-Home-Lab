# Active-Directory-Home-Lab

## Summary
In this project, I am simulating the same type of Windows networking environment used by companies and universities with Active Directory.

**Active Directory** is a centralized and hierarchical database system developed by Microsoft for managing and organizing network resources, such as computers, users, groups, printers, and other objects, within a network. It provides services for authentication, authorization, and directory services, allowing administrators to efficiently manage and secure their network infrastructure.

The process followed in this project involves setting up Active Directory on a virtual machine as a domain controller. Two network adapters are configured on the domain controller: one for connecting to the internet, and another for internal clients. IP addressing, NAT (Network Address Translation), routing, and DHCP (Dynamic Host Configuration Protocol) are configured for an internal server. A PowerShell script is then used to create 1,000 user accounts on the internal server. Additionally, another virtual machine is created using VirtualBox, connected to the internal server, and logged in as one of the created users, demonstrating successful integration with the simulated Active Directory environment.

This project aims to replicate a real-world Active Directory setup, providing hands-on experience in configuring and managing a Windows networking environment. It serves as a valuable learning resource for IT professionals, system administrators, and anyone interested in understanding and working with Active Directory.

## Technologies Used

- Active Directory Domain Services
- VirtualBox
  - Windows 10 ISO
  - Server 2019 ISO
- IP Adressing
- NAT (Network Address Translation)
- Routing
- DHCP (Dynamic Host Configuration Protocol)
- PowerShell

## Project Walkthrough

 1. Download and install Oracle VirtualBox from the official website.
[Oracle Virtual Box](https://www.virtualbox.org/)

 2. Download the Windows 10 and Server 2019 ISO files.
[Windows 10 iso](https://www.microsoft.com/en-us/software-download/windows10ISO)
[Windows Server 2019](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)

 3. Create a new virtual machine by clicking on "New" in VirtualBox, naming it "Domain Controller," and selecting the "Windows Server 2019" ISO file as the boot media.

 4. Configure the virtual machine by giving it two network adapters: one for connecting to the internet and the other for the private network.

 5. Install Server 2019 on the virtual machine and assign IP addressing for the internal network.

 6. Name the server and install Active Directory to create the domain.

 7. Configure routing so that clients on the private network can access the internet through the domain controller.

 8. Set up DHCP on the domain controller.

 9. Run the PowerShell script to create 1000 users in Active Directory.

[Power Shell script for creating users](https://github.com/joshmadakor1/AD_PS)

 10. Create a new virtual machine named "Client1" and install Windows 10 on it.

 11. Connect the client machine to the private network and join it to the domain.

 12. Log into the client machine with a domain account.
<!--
# Active-Directory-Home-Lab

## Summary
In this project, I am simulating the same type of Windows netowrking environment used by companies and universities with Active Directory. 

**Active Directory** is a centralized and hierarchical database system developed by Microsoft for managing and organizing network resources, such as computers, users, groups, printers, and other objects, within a network. It provides services for authentication, authorization, and directory services, allowing administrators to efficiently manage and secure their network infrastructure.

 ## Summary

In this project, I've created an Active Directory home lab to simulate a Windows networking environment akin to those used by organizations. Through setting up Active Directory on a virtual machine as a domain controller, I've established a centralized system for managing and organizing network resources.

To facilitate connectivity and access, I've configured two network adaptors on the domain controller, segregating one for internet access and the other for internal clients. Additionally, I've handled IP addressing, configured NAT (Network Address Translation), routing, and DHCP (Dynamic Host Configuration Protocol) for an internal server.

Taking advantage of PowerShell automation, I executed a script to efficiently generate 1,000 users on the internal server, enabling scalability and testing scenarios with a large user base. Furthermore, I expanded the lab environment by creating another virtual machine using VirtualBox, establishing connectivity to the internal server, and successfully logging in as one of the users.

Through this process, I've not only simulated the complexities of an Active Directory environment but also gained practical experience in network administration, server configuration, and user management. This GitHub repository serves as a comprehensive guide and resource for setting up and understanding Active Directory in a home lab environment.





I set up a virtual machine on Azure with a publically routable IP address and configure the firewalls to allow hackers from anywhere to attempt to log in. Then, I use a Geolocation API with a powershell script to extract the IP addresses of hackers and display them on a Sentiel world map.

## Technologies Used

- Azure
  - Virtual Machine
  - Log Analytics
  - Security Center
  - Sentinel
- Windows Defender Firewall
- Powershell
- Event Viewer
- [ipgeolocation.io](https://ipgeolocation.io/) API Key

## Project Walk-through
 1. Create Azure Subscription
 2. Create Virtual Machine
 3. Publicly route VM IP address
 4. Create Log Analytics Workspace
 5. Enable gathering of VM logs in Security Center
 6. Connect Log Analytics to VM
 7. Setup Azure Sentinel
 8. Log into VM with Remote Desktop
 9. Observe Event viewer Logs in VM
 10. Disable firewall on VM
 11. Run powershell script
 12. Get Geolocation.io API Key to convert hacker IP addresses int Geo data with script
 13. Create custom log in Log Analytics Workspace to manage Geo data
 14. Extract fields from raw custom log data
 15. Setup map in Sentinel with Latitude and Longitude
 16. Display data on map

## The Result
