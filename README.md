# Active Directory Deployment in Microsoft Azure

## Project Overview

This project demonstrates the deployment of a **Windows Server 2022 Active Directory Domain Services (AD DS) environment** in Microsoft Azure to simulate a corporate IT infrastructure.

The lab includes domain controller deployment, DNS configuration, domain joining a client workstation, and performing common **Tier 1 help desk administrative tasks**.

This environment replicates a simplified enterprise identity infrastructure used in many corporate networks.

---

## Technologies Used

* Microsoft Azure
* Windows Server 2022
* Active Directory Domain Services (AD DS)
* DNS
* Windows Client Virtual Machine
* Remote Desktop (RDP)

---

## Lab Architecture

Azure Infrastructure:

* **1x Windows Server 2022 VM (dc-01)** – Domain Controller
* **1x Windows Client VM (client-01)** – Domain-joined workstation
* **Azure Virtual Network (VNet)**
* **Custom DNS configuration pointing to Domain Controller**

Domain configuration:

Domain Name:

```
corp.local
```

---

## Implementation Steps

1. Created Azure Resource Group and Virtual Network
2. Deployed Windows Server 2022 virtual machine
3. Installed **Active Directory Domain Services (AD DS)**
4. Promoted server to **Domain Controller**
5. Configured **DNS services**
6. Created Organizational Units (OUs), users, and security groups
7. Deployed Windows client virtual machine
8. Configured custom DNS settings on the client
9. Joined client machine to the domain
10. Verified domain authentication and user login
11. Simulated Tier 1 help desk tasks

Help desk tasks included:

* Password reset
* Account unlock
* Account disable/enable
* User group membership management

---

## Validation

Screenshots in the `/screenshots` directory demonstrate:

* Azure infrastructure configuration
* Domain controller promotion
* Active Directory Users and Computers management
* Successful domain join
* Domain user authentication
* User account administration tasks

---

## Skills Demonstrated

* Active Directory deployment and configuration
* DNS configuration and troubleshooting
* Domain join troubleshooting
* Organizational Unit (OU) management
* User and group administration
* Authentication validation
* Tier 1 help desk account management

---

## Future Improvements

Potential enhancements for this lab include:

* Implement **Group Policy Objects (GPOs)**
* Automate administration tasks using **PowerShell**
* Integrate **Azure AD / Entra ID hybrid identity**
* Implement **role-based access control (RBAC)**

---

## About

This project demonstrates practical identity management skills by deploying Active Directory Domain Services in Microsoft Azure, configuring DNS, joining a client workstation to the domain, and performing common help desk administrative tasks.
