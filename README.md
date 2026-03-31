Active Directory Home Lab Integrating PowerShell Project 

## Objective: 

This project demonstrates the deployment and management if a Windows Active Directory environment with integrated PowerShell automation, It replicaets real-world IT tasks such as user provisioning, access control, and troubleshooting in a domain-based infrastructure. 

## Key Contribution 
- Deployed and configured a Windows Server Active Directory domain, including domain controller setup, Organizational Units (OUs), user/group management, and Group Policy enforcement
- Developed PowerShell automation scripts to streamline adminstrative tasks such as bulk user creation, password resets, account unlocks, and group assignments.
- Simulated real-world help desk scenarious, including onboarding users, resolving login/account lockouts, and troubleshooting permissions/access issues across the domain

## Skills Learned 
- Domain Controllers
- Configuring Group Policys
- Troubleshooting
- Security Administration
- User account Creation and Management
- Understanting Organizational Units

## Tech Stack 
- Windows Server (Active Directory Domain Services)
- Windows 10/11 Client
- PowerShell
- Group Policy Management
- Virtualization (Parallels Desktop)

## Lab Architecture 
[ Windows 10 Client ]
          |
          | (Domain Join)
          |
[ Domain Controller (Windows Server) ]
          |
   -------------------------
   |           |           |
 [Users]     [Groups]     [GPOs]

 ## Setup and Configuration 
 1. Domain Controller Setup
- Installed Active Directory Domain Services (AD DS)
- Promoted server to Domain Controller
- Created custom domain

2. User and Group Management
- Created Organizational Units (OUs) for structure
- Added users and assigned group memberships
- Applied least privilege access principles
3. Group Policy Configuration
- Enforced password policies
- Configured security settings
- Applied restrictions to simulate enterprise environment

## Key Skills Demonstrated 
- Active Directory Adminstration
- Identity and Access Management (IAM)
- PowerShell Scripting and Automation
- Troubleshooting (Login Issues, Permissions,Lockouts)
- Enterprise IT Support Workflows

 ## What I Did 

 - Deployed and configured a Windows Server Active Directory environment, inlcuding domain controller setup, OU structure, and User/group management and Group Policy enforcement
 - Built Powershell automation scripts to streamline user provisioning, password resets, account unlocks, and group assignments, reducing manual administrative effort
 - Simulated real world IT support scenarios such as onboarding users, troubleshooting login issues, resolving account lockouts, and validading access permissions across the domain.

## What I learned 

This project gave not only hands-on experience with using Active Directory administration and supporting IT workflows, but it also really opened my eyes to how interesting and how much there is to learn with automation. In the process I was also about to stregnthen my ability to use Powershell to automate repetitive tasks and troubleshoot identity/access issues efficiently. 

## Future Improvements 
- Integrate Azure AD / Entra ID (Hybrid Environment)
- Add SIEM monitoring (Splunk / Wazuh)
- Expand PowerShell scripts for reporting and auditing 

The process will be in the Write Up portion 

