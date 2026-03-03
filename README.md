# Active Directory Deployment in Microsoft Azure

## Project Overview
This project demonstrates the deployment and configuration of a Windows Server 2022 Domain Controller in Microsoft Azure to simulate an enterprise on-premises Active Directory environment.

The lab replicates real-world Tier 1 IT Support responsibilities including domain deployment, DNS troubleshooting, user account management, and domain join configuration.

---

## Architecture

- 1x Windows Server 2022 VM (dc-01) – Domain Controller
- 1x Windows Client VM (client-01) – Domain-joined workstation
- Azure Virtual Network (10.0.0.0/16)
- Custom DNS configuration pointing to Domain Controller (10.0.0.4)
- Domain: corp.local

---

## Technologies Used

- Microsoft Azure
- Windows Server 2022
- Active Directory Domain Services (AD DS)
- DNS
- Remote Desktop Protocol (RDP)

---

## Deployment & Configuration Steps

1. Created Azure Resource Group
2. Created Virtual Network and Subnet
3. Deployed Windows Server 2022 VM (dc-01)
4. Installed Active Directory Domain Services (AD DS)
5. Promoted server to Domain Controller (corp.local)
6. Verified DNS configuration on Domain Controller
7. Configured VNet DNS to point to DC private IP (10.0.0.4)
8. Deployed Windows client VM (client-01)
9. Updated client DNS settings to use Domain Controller
10. Joined client machine to domain
11. Restarted and validated domain authentication

---

## Active Directory Configuration

- Created Organizational Units (OUs)
- Created security groups
- Created domain user accounts
- Assigned users to security groups
- Verified group membership

---

## Help Desk Task Simulation

Performed common Tier 1 IT support tasks:

- Password reset
- Account unlock
- Account disable/enable
- Verified domain user RDP login

---

## Troubleshooting Performed

- Resolved domain join failure caused by incorrect DNS configuration
- Verified DNS using `ipconfig /all`
- Restarted VMs after DNS changes
- Resolved RDP login authorization issue by adjusting group membership
- Confirmed domain connectivity before authentication testing

---

## Validation

Screenshots located in the `/screenshots` folder demonstrate:

- Azure infrastructure deployment
- Active Directory installation
- Successful domain join
- DNS configuration validation
- Domain user authentication via RDP
- Help desk account management tasks

---

## Skills Demonstrated

- Active Directory deployment and configuration
- DNS setup and troubleshooting
- Azure networking fundamentals
- Domain join troubleshooting
- User account lifecycle management
- Identity and access management fundamentals
- Remote Desktop troubleshooting

---

## Purpose

This lab simulates real-world enterprise IT Support responsibilities within a controlled Azure environment. It demonstrates foundational knowledge required for Help Desk, IT Support Specialist, and Junior Systems Administrator roles.
