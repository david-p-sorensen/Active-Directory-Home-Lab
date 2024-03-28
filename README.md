# Active-Directory-Home-Lab

## Summary
In this project, I am simulating the same type of Windows netowrking environment used by companies and universities with Active Directory. 

**Active Directory** is a centralized and hierarchical database system developed by Microsoft for managing and organizing network resources, such as computers, users, groups, printers, and other objects, within a network. It provides services for authentication, authorization, and directory services, allowing administrators to efficiently manage and secure their network infrastructure.




<!--

 

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
