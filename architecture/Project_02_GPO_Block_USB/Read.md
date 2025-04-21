Project 02 – Group Policy: Block USB Devices

This project configures a Group Policy Object (GPO) to block USB device access for domain users, simulating a common security hardening task in enterprise environments.

---

Summary

This policy disables USB storage devices to prevent data leakage and enforce compliance.

---

Steps Completed

Step 1: Open Group Policy Management Console  
Opened the Group Policy Management Console from Server Manager.  
![Step 1](./screenshots/Step1_Open_Group_Policy_Management_Console.png)

---

Step 2: Create an OU and Move the Test Computer  
Created a new Organizational Unit (OU) named `TestOU` and moved the test computer into it.  
![Step 2](./screenshots/Step2_Test_Computer_Moved_to_TestOU.png)

---

Step 3: Create and Link a New GPO  
Created a new GPO named `Block_USB_GPO` and linked it to the `TestOU`.  
![Step 3](./screenshots/Step3_Create_And_Link_Block_USB_GPO.png)

---

Step 4: Edit the GPO to Block USB Access  
Opened the GPO editor and navigated to:  
`Computer Configuration > Policies > Administrative Templates > System > Removable Storage Access`

- Screenshot of opening the policy editor:  
  ![Step 4a](./screenshots/Step4a_Initial_GPO_Editor_View.png)

- Enabled the setting: **All Removable Storage Classes: Deny All Access**  
  ![Step 4b](./screenshots/Step4b_Enable_DEny_All_Removable_Access.png)

---

Step 5: Update Group Policy on the Client  
Ran `gpupdate /force` on the Windows 10 Client to pull the new policy.  
![Step 5](./screenshots/Step5_gpupdate_force_confirmation.png)

---

Step 6: Verify Policy was Applied  
Used the `gpresult` command to confirm that `Block_USB_GPO` was successfully applied.  
![Step 6](./screenshots/Step6_gpresult_Block_USB_verification.png)

---

Folder Contents

- `/screenshots/` – Visual walkthrough of each step
- `Project2_GPO_Block_USB_Guide.pdf` – Full PDF lab walkthrough (if included)

---

## ✅ Status:  
🟩 **Complete**
