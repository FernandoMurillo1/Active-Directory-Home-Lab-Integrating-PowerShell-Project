# Active Directory Home Lab with PowerShell Automation

## Objective

This project demonstrates the deployment and management of a Windows Active Directory environment with integrated PowerShell automation. It replicates real-world IT tasks such as user provisioning, access control, and troubleshooting in a domain-based infrastructure.

## Key Contributions

- Deployed and configured a Windows Server Active Directory domain, including domain controller setup, Organizational Units (OUs), user/group management, and Group Policy enforcement
- Developed PowerShell automation scripts to streamline administrative tasks such as bulk user creation, password resets, account unlocks, and group assignments
- Simulated real-world help desk scenarios, including onboarding users, resolving login/account lockouts, and troubleshooting permissions/access issues across the domain

## Tech Stack

- Windows Server (Active Directory Domain Services)
- Windows 10/11 Client
- PowerShell
- Group Policy Management
- Virtualization (Parallels Desktop)

## Lab Architecture

```
+------------------+          Domain Join          +----------------------------------+
|  Windows 10       |  ----------------------->     |  Domain Controller                |
|  Client            |                               |  (Windows Server)                 |
+------------------+                               +----------------------------------+
                                                        |
                                                        |-- Organizational Units (OUs)
                                                        |-- Users
                                                        |-- Security Groups
                                                        |-- Group Policy Objects (GPOs)
```

## Setup and Configuration

1. **Domain Controller Setup**
   - Installed Active Directory Domain Services (AD DS)
   - Promoted server to Domain Controller
   - Created custom domain

2. **User and Group Management**
   - Created Organizational Units (OUs) for structure
   - Added users and assigned group memberships
   - Applied least privilege access principles

3. **Group Policy Configuration**
   - Enforced password policies
   - Configured security settings
   - Applied restrictions to simulate an enterprise environment

## PowerShell Scripts

See [`/scripts`](./scripts) for the automation scripts used in this lab:

- `New-BulkUsers.ps1` — bulk user creation from a CSV list
- `Reset-UserPassword.ps1` — password reset and forced change at next logon
- `Unlock-UserAccount.ps1` — account unlock and lockout status check
- `Add-UserToGroup.ps1` — group assignment automation

## Key Skills Demonstrated

- Active Directory Administration
- Identity and Access Management (IAM)
- PowerShell Scripting and Automation
- Troubleshooting (login issues, permissions, lockouts)
- Enterprise IT Support Workflows

## What I Did

- Deployed and configured a Windows Server Active Directory environment, including domain controller setup, OU structure, user/group management, and Group Policy enforcement
- Built PowerShell automation scripts to streamline user provisioning, password resets, account unlocks, and group assignments, reducing manual administrative effort
- Simulated real-world IT support scenarios such as onboarding users, troubleshooting login issues, resolving account lockouts, and validating access permissions across the domain

## What I Learned

This project gave me hands-on experience with Active Directory administration and IT support workflows, and it deepened my interest in automation. I strengthened my ability to use PowerShell to automate repetitive tasks and to troubleshoot identity/access issues efficiently.

## Future Improvements

- Integrate Azure AD / Entra ID (hybrid environment)
- Add SIEM monitoring (Wazuh) for domain activity
- Expand PowerShell scripts for reporting and auditing

## Screenshots

See [`/screenshots`](./screenshots) for full-size images.

| Screenshot | Description |
|---|---|
| AD structure | Active Directory environment with organized OUs, users, and security groups configured to simulate a real enterprise structure |
| PowerShell execution | Execution of PowerShell scripts used to automate administrative tasks such as bulk user creation, password resets, and account management |
| Domain-joined client | Windows client successfully joined to the domain, validating authentication, applied policies, and access to domain resources |

Full process write-up: [`Write-Up.md`](./Write-Up.md)
