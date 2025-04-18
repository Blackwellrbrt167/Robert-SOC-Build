Project 01 – Active Directory Deployment (Windows Server)

This project marks the foundational stage of building out my SOC (Security Operations Center) lab. Here, I configure a Windows Server 2019 virtual machine and promote it to a Domain Controller using Active Directory Domain Services (AD DS). This sets up the authentication backbone needed for future SOC operations.

---

Objective

To successfully install and configure a Windows Server VM, assign it a static IP, and promote it to a Domain Controller with `lab.local` as the root domain.

---

Key Milestones Completed

- Installed Windows Server 2019 in VirtualBox  
- Assigned a static IP address  
- Promoted the server to Domain Controller  
- Created a domain: `lab.local`  
- Created an Organizational Unit (OU) called `TestOU`  
- Added a sample user: `TestUser1` for login testing  
- Re-promoted Domain Controller to capture confirmation screen

---

Folder Contents

- `Project1_AD_Deployment_With_GitHub_FINAL.pdf` – Step-by-step PDF guide for beginners  
- `screenshots/` – Visual walkthroughs of the process with clear, labeled steps  

---

Screenshots of Setup Process

Click any image below to enlarge.

---

1. Windows Server Lab VM Settings**  
![VM Settings](./screenshots/Windows_Server_Lab_VM_Settings.png)

---

2. Static IP Configuration**  
![Static IP](./screenshots/Static_IP_Creation.png)

---

3. Installing Windows Server Features**  
![Server Install](./screenshots/Installed_Windows_Server_Complete.png)

---

4. Adding Active Directory Domain Services**  
![AD Role](./screenshots/Active_Directory_Role_Installation.png)

---

5. Promoting to Domain Controller**  
![Domain Controller](./screenshots/Domain_Controller_Creation_Completion.png)

---

6. Domain Promotion Confirmation**  
![Confirmation](./screenshots/Domain_Promotion_Completed-Confirmation.png)

---

Reflections

This project was my first real-world implementation of Active Directory. While it may seem basic, it represents a major leap forward in my IT/cybersecurity learning journey. I ran into errors, overcame setbacks, and even re-promoted the Domain Controller to ensure complete and accurate documentation.

---

What's Next?

With AD deployed, my next projects include:

- Setting up DHCP & DNS  
- Implementing Group Policy Objects (GPOs)  
- Connecting endpoints to the domain  
- Simulating real-world SOC security workflows

---

Every step, mistake, and fix is part of my blueprint to mastery in cybersecurity. This is Project 01 — and just the beginning.
