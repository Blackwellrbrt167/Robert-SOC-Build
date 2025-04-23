# Project 04 – DNS Configuration & Domain Join Verification

This project focuses on configuring DNS within the lab domain and verifying successful client integration by joining a Windows 10 machine to the Active Directory domain hosted on the Windows Server 2019 Domain Controller.

---

## 🧠 Summary

We configured internal DNS to support Active Directory functionality, verified that the domain controller handled name resolution, and successfully joined a Windows 10 client to the domain (`lab.local`). This simulates a standard enterprise setup in which clients are domain-joined and rely on internal DNS for resolution.

---

## ✅ Steps Completed

1. **Verified DNS Installation on Server**
   - Confirmed that the DNS role was installed during AD DS setup.
   - Opened DNS Manager and validated forward lookup zones were created (e.g., `lab.local`).

2. **Verified DNS Records**
   - Checked for key records: `A`, `NS`, `SRV` entries for the domain controller under `lab.local`.
   - Ensured the domain controller’s IP matched the DNS host record.

3. **Configured Client DNS Settings**
   - Opened the Windows 10 client’s network adapter settings.
   - Manually configured the IPv4 settings to use the **domain controller’s IP address as the DNS server** (e.g., `192.168.1.2`).

4. **Tested DNS Resolution**
   - Opened Command Prompt on the client.
   - Ran `nslookup lab.local` and `ping lab.local` to ensure successful name resolution.
   - Verified that the client could reach the domain controller via hostname.

5. **Joined Client to the Domain**
   - Opened **System Properties** > **Computer Name** tab > clicked **Change**.
   - Selected **Domain**, entered `lab.local`, and provided domain credentials.
   - Restarted the client to complete domain join.

6. **Validated Domain Join**
   - Logged in using domain credentials.
   - Checked Active Directory to ensure the client appeared in the correct OU (e.g., `TestOU`).
   - Ran `gpresult /r` and confirmed domain group policy application.

---

## 📁 Folder Contents

- `screenshots/` – Visual walkthroughs for each step
- `Project4_DNS_Config_Domain_Join_Guide.pdf` – Full documentation with detailed instructions and troubleshooting

---

## 🔐 Skills Demonstrated

- DNS configuration and zone verification
- Internal IP and DNS settings management
- Active Directory domain join troubleshooting
- Command-line verification (`nslookup`, `ping`, `gpresult`)

