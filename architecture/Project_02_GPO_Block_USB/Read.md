Project 02 – Group Policy: Block USB Devices

This project configures a Group Policy Object (GPO) to block USB device access for domain users, simulating a common security hardening task in enterprise environments.

---

Summary

This policy disables USB storage devices to prevent data leakage and enforce compliance.

---

Steps Completed

Step 1: Open Group Policy Management Console  
Opened the Group Policy Management Console from Server Manager.  
![Step1_Open_Group_Policy_Management_Console](https://github.com/user-attachments/assets/2e3b5731-d2b7-4690-84dc-2458a9d97bbb)


---

Step 2: Create an OU and Move the Test Computer  
Created a new Organizational Unit (OU) named `TestOU` and moved the test computer into it.  
![Step2_Test_Computer_Moved_to_TestOU](https://github.com/user-attachments/assets/7f99d7d0-a1ca-40a2-90d1-426155cce542)


---

Step 3: Create and Link a New GPO  
Created a new GPO named `Block_USB_GPO` and linked it to the `TestOU`.  
![Step3_Create_And_Link_Block_USB_GPO](https://github.com/user-attachments/assets/6aae6782-a5fc-44bc-ae60-f05e5214221f)


---

Step 4: Edit the GPO to Block USB Access  
Opened the GPO editor and navigated to:  
`Computer Configuration > Policies > Administrative Templates > System > Removable Storage Access`

- Screenshot of opening the policy editor:  
 ![Step 4a_Initial_GPO_Editor_View](https://github.com/user-attachments/assets/4314496c-6076-4afe-9d52-82ae403c1ee4)


- Enabled the setting: **All Removable Storage Classes: Deny All Access**  
  ![Step 4b_Enable_DEny_All_Removable_Access](https://github.com/user-attachments/assets/8b6a095a-be6f-401d-8115-1977ac9e0e90)


---

Step 5: Update Group Policy on the Client  
Ran `gpupdate /force` on the Windows 10 Client to pull the new policy.  
![Step5_gpupdate_force_confirmation](https://github.com/user-attachments/assets/e2d23a7c-546d-440a-9711-36b04115b5b7)


---

Step 6: Verify Policy was Applied  
Used the `gpresult` command to confirm that `Block_USB_GPO` was successfully applied.  
![Step6_gpresult_Block_USB_verification](https://github.com/user-attachments/assets/61ea8749-310f-49a0-ad10-ed98121560f6)


---

Folder Contents

- `/screenshots/` – Visual walkthrough of each step
- `Project2_GPO_Block_USB_Guide.pdf` – Full PDF lab walkthrough (if included)

---

## ✅ Status:  
🟩 **Complete**
