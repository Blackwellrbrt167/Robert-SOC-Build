Architecture – SOC Lab Foundation

This section documents the **core infrastructure** of my home-lab Security Operations Center (SOC) build. It includes all base-level systems needed to simulate a real-world enterprise environment where security controls, detection, and monitoring can take place.

---

Projects in This Section

| Project | Description | Status |
|--------|-------------|--------|
| [Project_01_AD_Deployment](./Project_01_AD_Deployment) | Built and configured a Windows Server 2019 Domain Controller using Active Directory Domain Services (AD DS). This creates the authentication backbone for the lab. | Complete |
| Project_02_GPO_Block_USB | Create and link Group Policy Objects (GPO) to manage device control such as disabling USB drives for domain users. | In Progress |
| Project_03_DHCP_Config | Setup of DHCP services for dynamic IP assignment to networked devices. | In Progress |
| Project_04_DNS_Config | Configure DNS zones and name resolution internally for the lab network. | Upcoming |

---

Purpose

This architecture layer provides:

- **User identity & authentication** (via Active Directory)
- **Group policy management** (via GPO)
- **Network infrastructure components** (DHCP, DNS, etc.)
- A foundation for SIEM, endpoint logging, and incident simulation

---

What You’ll See in Each Subproject

Each folder contains:

- `README.md` file that explains what was built, why it matters, and what was learned
- Screenshot walkthroughs
- PDF documentation of all steps taken

---

> This architecture layer is a critical first step in building out my SOC—from identity to infrastructure—and sets the stage for SIEM deployment, threat simulation, and security automation in later stages.
