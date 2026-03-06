# IT Administration – Active Directory Lab

## Overview
This project demonstrates a basic IT administration environment using **Active Directory Domain Services (AD DS)**.

The lab simulates a small company network where different departments have specific permissions, policies, and access control.

The environment was built using virtual machines to simulate a real enterprise network.

---

## Lab Environment

The lab environment was built using **Oracle VM VirtualBox**.

Two virtual machines were created to simulate a domain environment:

| VM  | Role | Description |
|-----|------|-------------|
| VM1 | Domain Controller / Admin | Hosts Active Directory and manages users, groups, and Group Policies |
| VM2 | Client Computer | Employee workstation joined to the domain |

---

## Domain Configuration

| Setting | Value |
|--------|------|
| Domain Name | moon.com |
| OU Name | Staff |

The domain controller manages authentication, policies, and access control for all users in the network.

---

## Departments

| Department | Members |
|-----------|---------|
| HR | Yazeed Ahmad |
| Finance | Sara Ahmad |
| IT | Mohammad Ahmad, Haya Ahmad, Yousef Ahmad |

---

## Client Computer

| User | Department | Status |
|-----|------------|--------|
| Sara Ahmad | Finance | Domain Joined |

---

## Group Policy

A **Group Policy Object (GPO)** was configured to restrict system access.

| Policy | Description |
|------|-------------|
| Disable Task Manager | Prevents users from accessing Task Manager |

---

## Shared Folder

Shared folder created: **Calc**

| Department | Permission |
|-----------|-------------|
| HR | Read & Execute |
| Finance | Read |
| IT | Full Control |

Rules:
- All users can open the calculator file.
- Only IT members can modify the folder.

---

## Skills Demonstrated

- Active Directory Domain Services
- Domain Controller Setup
- Organizational Units (OU)
- User & Group Management
- Group Policy Management
- File Server Permissions
- Domain Joining
- Virtual Lab using VirtualBox

---

## Project Team

- Lana  
- Qasem  
- Omar Alfaroq
