Project 01 – Active Directory Deployment (Windows Server)

This project serves as the foundation of my SOC lab build by configuring a Windows Server 2019 machine as a Domain Controller using Active Directory Domain Services (AD DS). This forms the authentication backbone for future infrastructure projects within the lab environment.

---

Key Objectives

- Provision a Windows Server 2019 Virtual Machine (VM) in VirtualBox
- Configure static IP addressing for consistency and network control
- Install AD DS and promote the server to a Domain Controller
- Create a local domain `lab.local`
- Establish a test Organizational Unit (OU)
- Create a sample user for login testing
- Validate successful domain promotion

---

 Folder Contents

- `Project01_AD_Deployment_With_GitHub_FINAL.pdf` — Complete step-by-step documentation with
- 
- `screenshots/` — Visual walkthrough of the build process

---

Screenshots (Click to Enlarge)

1. Windows Server Lab VM Settings  
Basic configuration setup for the Windows Server 2019 VM in VirtualBox  
![VM Settings](../../screenshots/Windows_Server_Lab_VM_Settings.png)

---

2. Static IP Configuration  
Static IP setup to avoid DHCP lease changes  
![Static IP](../../screenshots/Static_IP_Creation.png)

---

3. Installing Windows Server Features  
Successful installation of key Windows Server roles and features  
![Server Install](../../screenshots/Installed_Windows_Server_Complete.png)

---

4. Adding Active Directory Domain Services (AD DS)  
Screenshot showing successful role selection and setup  
![AD Role](../../screenshots/Active_Directory_Role_Installation.png)

---

5. Promoting to Domain Controller  
Confirmation of domain promotion and readiness  
![Domain Controller Creation](../../screenshots/Domain_Controller_Creation_Completion.png)

---

 6. Domain Promotion Confirmation  
Final confirmation of successful promotion to Domain Controller  
![Domain Promotion Completed](../../screenshots/Domain_Promotion_Completed-Confirmation.png)

---

Summary

This build marks the beginning of my hands-on Security Operations Center (SOC) project. Through this Active Directory deployment, I’ve laid the groundwork to manage users, authenticate devices, and simulate a realistic enterprise network. Every step reflects both my learning and my commitment to mastering cybersecurity fundamentals through self-built infrastructure.

