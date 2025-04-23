# Project 04 – DNS Setup & Domain Join Verification

This project demonstrates how to configure DNS settings on a Windows Server 2019 Domain Controller and properly connect a client machine to the domain using those DNS settings. This forms the foundation of name resolution and domain-level communication within the enterprise environment.

---

## 🧠 Summary

We configured the Domain Name System (DNS) on our Windows Server, ensured our client machine pointed to it for name resolution, joined the client to the domain, and verified successful communication through DNS queries. These steps are essential for enabling directory-based network services such as Active Directory.

---

## ✅ Steps Completed

### 1. **Checked DNS Settings on the Server**
- Confirmed the domain controller was running the DNS Server role.
- Verified that a Forward Lookup Zone for the domain (`lab.local`) existed.
- ![Step 1_ DNS_Settings_On_Server](https://github.com/user-attachments/assets/ba3e41ed-7132-4625-9055-85c1e39cb632)


### 2. **Set Client Computer's DNS**
- Updated the client VM’s IPv4 settings to **obtain an IP address automatically** and **manually set the Preferred DNS Server to the domain controller’s IP (192.168.1.2)**.
- ![Step 2_Network_Settings_DNS_Configuration](https://github.com/user-attachments/assets/bfb303b9-e879-403b-97b7-0d4e28179827)


### 3. **Joined the Client to the Domain**
- Navigated to **System Properties** > **Change Settings**.
- Selected the **Domain** option and joined the client to `lab.local`.
- Restarted the machine upon successful domain join prompt.
- ![Step 3_Domain_join-confirmation ](https://github.com/user-attachments/assets/d3ee5d68-9b74-42a5-8ba1-4852525eeead)


### 4. **Tested the DNS Connection**
- Ran `nslookup lab.local` from the client to verify domain resolution.
- Successfully resolved the domain controller's hostname and IP, confirming proper DNS connectivity.
- ![Step 4_Success_Ping_NSlookup_Connection_Test ](https://github.com/user-attachments/assets/5afa23b9-3bc6-4f5f-bf09-961cd25333d2)


---

## 📂 Folder Contents

- `screenshots/` – Visual walkthrough of each step.
- `Project4_DNS_Domain_Join_Guide.pdf` – Full step-by-step documentation.

---

## 🛠️ Tools Used

- Windows Server 2019 (Domain Controller & DNS Server)
- Windows 10 Client (VirtualBox)
- VirtualBox NAT/Internal Network Mode

---

## 🧠 Key Concepts Practiced

- DNS configuration and verification
- Domain joining process in Active Directory environments
- Name resolution using `nslookup` and DNS testing
