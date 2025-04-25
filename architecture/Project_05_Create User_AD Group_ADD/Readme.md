# Project 05 – Create Test User and Add to Active Directory Group

This project demonstrates how to create a new user in Active Directory (AD) and assign them to a specific security group. It simulates a common task performed by IT administrators to manage user access, enforce role-based permissions, and streamline domain-based user control.

---

## 🧩 Summary

We created a test user account using the Active Directory Users and Computers (ADUC) console, placed the user in the appropriate Organizational Unit (OU), and added the account to a security group. This type of administrative task ensures that domain users are structured for proper access, policy enforcement, and authentication within the enterprise environment.

---

## ✅ Steps Completed

1. **Opened Active Directory Users and Computers**
   - Launched the ADUC console from Server Manager or by running `dsa.msc`.

2. **Created a New User Account**
   - Navigated to the `TestOU` created in earlier projects.
   - Right-clicked the OU and selected **New > User**.
   - Entered the user's first name, last name, and username (e.g., `TestUser1`).
   - Set an initial password and chose to **uncheck** "User must change password at next logon" for lab simplicity.

3. **Created or Selected a Security Group**
   - Created a new **Security Group** called `Lab_Users` or used an existing one.
   - Set group scope to **Global** and type to **Security**.

4. **Added the User to the Group**
   - Right-clicked the `TestUser1` account.
   - Selected **Add to a group…** and typed/select `Lab_Users`.

5. **Verified Group Membership**
   - Opened the user’s properties and confirmed `Member Of` included `Lab_Users`.

---

## 📁 Folder Contents

- `screenshots/` – Step-by-step screenshots showing user creation and group assignment.
- `Project5_AD_User_Group_Guide.pdf` – Full documentation of steps for offline review.

---

## 🔧 Skills Applied

- Active Directory user management  
- Role-based access control (RBAC) fundamentals  
- Organizational Unit (OU) and group structuring  
- Lab environment account provisioning  


