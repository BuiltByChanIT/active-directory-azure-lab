# Active Directory Deployment in Microsoft Azure

## Project Overview
This project demonstrates the deployment of a Windows Server 2022 Domain Controller in Microsoft Azure to simulate an on-premises enterprise environment.

The lab includes:
- Active Directory Domain Services (AD DS)
- DNS configuration
- Domain join of a Windows client machine
- Organizational Unit (OU) and user account management
- Tier 1 help desk tasks (password reset, account unlock, disable)

---

## Architecture

- 1x Windows Server 2022 VM (dc-01) – Domain Controller
- 1x Windows Client VM (client-01) – Domain-joined workstation
- Azure Virtual Network (VNet)
- Custom DNS configuration pointing to Domain Controller
- Domain: corp.local

---

## Technologies Used

- Microsoft Azure
- Windows Server 2022
- Active Directory Domain Services (AD DS)
- DNS
- Remote Desktop (RDP)

---

## Deployment Steps (High-Level)

1. Created Azure Resource Group
2. Created Virtual Network
3. Deployed Domain Controller VM
4. Installed and configured AD DS
5. Promoted server to Domain Controller (corp.local)
6. Configured VNet DNS to DC private IP
7. Deployed client VM
8. Joined client to domain
9. Created OUs and user accounts
10. Performed help desk account management tasks

---

## Validation

Screenshots in the `/screenshots` folder demonstrate:

- Azure infrastructure configuration
- Active Directory setup
- Successful domain join
- Domain user authentication
- User management tasks

---

## Skills Demonstrated

- Active Directory deployment and configuration
- DNS setup for domain environments
- Domain join troubleshooting
- User account lifecycle management
- Basic enterprise identity management

---

## Purpose

This lab simulates real-world Tier 1 IT Support responsibilities within a controlled Azure environment.
