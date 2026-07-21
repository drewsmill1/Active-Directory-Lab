# Active Directory Lab

Active Directory homelab built on AWS EC2 using Windows Server, PowerShell, and Active Directory Domain Services (AD DS).

This project simulates a small business Active Directory environment where users, organizational units, and security groups are managed using standard system administration practices.

---

# Technologies Used

- AWS EC2
- Windows Server
- Active Directory Domain Services (AD DS)
- Active Directory Users and Computers
- PowerShell
- Remote Desktop Protocol (RDP)
- GitHub Documentation

---

# Project Objectives

The goal of this project was to build hands-on experience with Windows Server administration and Active Directory management.

Objectives completed:

- Deploy a Windows Server instance in AWS EC2
- Configure Windows Server as an Active Directory Domain Controller
- Create and manage an Active Directory domain
- Create Organizational Units (OUs)
- Create and manage security groups
- Create and manage user accounts
- Assign users to security groups
- Perform common help desk administration tasks
- Document administrative tasks using ticket-style documentation

---

# Environment Setup

## Infrastructure

Cloud Provider:
```
AWS EC2
```

Operating System:
```
Windows Server
```

Server Role:
```
Active Directory Domain Controller
```

Domain:
```
lab.local
```

---

# PowerShell Commands Used

The following PowerShell commands were used during the setup process:

```powershell
Install-WindowsFeature AD-Domain-Services -IncludeManagementTools

Install-ADDSForest -DomainName "lab.local"
```

These commands installed Active Directory Domain Services and promoted the Windows Server instance to a Domain Controller.

---

# Active Directory Structure

The Active Directory environment was organized using Organizational Units to separate users and resources.

Example structure:

```
lab.local

├── Employees
│
│   ├── IT
│   │
│   ├── HR
│   │
│   ├── Sales
│   │
│   └── Managers
│
└── Security Groups
```

---

# Completed Tasks

## Active Directory Configuration

Completed:

* Created Windows Server EC2 instance  
* Connected to server using Remote Desktop Protocol (RDP)  
* Installed Active Directory Domain Services  
* Promoted server to Domain Controller  
* Created lab.local domain  

---

# Organizational Unit Management

Created Organizational Units to organize users:

- IT
- HR
- Sales
- Managers

Organizational Units were used to separate users based on department and improve Active Directory organization.

---

# User Management

Created Active Directory user accounts and organized them into appropriate departments.

Tasks completed:

- Created user accounts
- Assigned users to Organizational Units
- Configured account settings
- Managed user memberships

---

# Security Group Management

Created Active Directory security groups:

- IT-Admins
- HR-Users
- Sales-Users
- Accounting-Users
- HelpDesk

Group configuration:

- Group Scope: Global
- Group Type: Security

Users were assigned to security groups based on department responsibilities.

---

# Help Desk Ticket Documentation

The `tickets` folder contains simulated IT support requests documenting common Active Directory administration tasks.

Completed tickets:

| Ticket | Description |
|---|---|
| Ticket #001 | Create Active Directory security groups |
| Ticket #002 | Create user accounts |
| Ticket #003 | Assign users to security groups |
| Ticket #004 | Remove temporary security groups |
| Ticket #005 | Reset user passwords |
| Ticket #006 | Disable user accounts |

These tickets demonstrate documentation practices used in IT support environments.

---

# Screenshots

Screenshots documenting the project can be found in the `screenshots` folder.

Included examples:

- Active Directory organizational structure
- Organizational Units
- User accounts
- Security groups
- Group memberships
- Account management tasks

Example:

![Active Directory Structure](screenshots/active-directory-structure.png)

---

# Repository Structure

```
Active-Directory-Lab

├── README.md
│
├── screenshots
│   ├── Active Directory screenshots
│   └── Configuration screenshots
│
├── tickets
│   ├── ticket-001-create-groups.md
│   ├── ticket-002-create-user-accounts.md
│   ├── ticket-003-assign-group-membership.md
│   ├── ticket-004-remove-test-group.md
│   ├── ticket-005-password-reset.md
│   └── ticket-006-disable-user-account.md

```

---

# Skills Demonstrated

Through this project I practiced:

- Windows Server administration
- Active Directory administration
- Domain Controller configuration
- User lifecycle management
- Security group management
- Organizational Unit design
- PowerShell administration
- Remote Desktop administration
- IT documentation practices
- Basic troubleshooting workflows

---

# Future Improvements

Potential additions to expand this lab:

- Join client machines to the domain
- Configure Group Policy Objects (GPOs)
- Implement shared folders and NTFS permissions
- Add additional Windows Server roles
- Configure automated user creation with PowerShell
- Create additional AWS resources for a larger simulated environment
