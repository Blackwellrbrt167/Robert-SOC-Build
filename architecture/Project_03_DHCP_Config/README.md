# Project 03 – DHCP Configuration in Windows Server

This project demonstrates how to configure the **Dynamic Host Configuration Protocol (DHCP)** service on a Windows Server 2019 Domain Controller. DHCP automatically assigns IP addresses and related network configuration to client devices in the domain.

---

## 🔧 Summary

We installed and configured the DHCP Server role, created a DHCP scope, and successfully allowed a domain-joined client machine to receive its network settings via dynamic assignment.

---

## ✅ Steps Completed

1. **Installed DHCP Server Role**  
   - Added the DHCP role via the Server Manager's Add Roles and Features Wizard.  
   - Launched and completed the post-install configuration wizard.
   - ![Step 1_DHCP Role_Installed](https://github.com/user-attachments/assets/6dac5082-88e2-4bf3-af32-f9d71d244919)


2. **Authorized the DHCP Server**  
   - Authorized the server in Active Directory to allow it to hand out IP addresses.
   - ![Step_2_DHCP Console_Server Listed](https://github.com/user-attachments/assets/f04f3d1a-8c35-4ee7-b0cd-ecaa4a6b365d)


3. **Created a New DHCP Scope**  
   - Defined an IP address range for the internal lab network.  
   - Configured subnet mask, lease duration, and default gateway.
   - ![Step_3_New Scope Created ](https://github.com/user-attachments/assets/9de9bb75-e307-4276-8887-6c181d9f8ac2)


4. **Activated the Scope**  
   - Verified that the new scope was active and ready to lease addresses.
   - ![Step 4_Scope_Router_and_DNS_configured ](https://github.com/user-attachments/assets/fa93b78d-d3f4-43f5-a2ed-e12a208acb33)


5. **Tested DHCP on Client VM**  
   - Ensured the client VM was set to **Obtain IP address automatically**.  
   - Ran `ipconfig /release` and `ipconfig /renew` to verify dynamic IP assignment.  
   - Verified IP address was successfully issued from the DHCP scope.
   - ![Step 5_Ipconfig results_correctly_assigned_IP ](https://github.com/user-attachments/assets/bb462855-e1f7-44a9-b7fb-2903dfd88cab)


