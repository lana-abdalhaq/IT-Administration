# IT-Administration-
Active Directory Lab



Overview

This project demonstrates a basic IT administration environment using Active Directory Domain Services (AD DS).

The lab simulates a small company network where different departments have specific permissions, policies, and access control.

The environment was built using virtual machines to simulate a real enterprise network.

Lab Environment

The project was implemented using Oracle VM VirtualBox.

Two virtual machines were created to simulate a domain environment:

VM	Role	Description
VM1	Domain Controller / Admin	Hosts Active Directory, manages users, groups, and policies
VM2	Client Computer	Employee workstation joined to the domain
Domain Configuration

Domain Name: moon.com

The domain controller manages authentication, policies, and access control for all users in the network.

Organizational Structure

An Organizational Unit (OU) called:

Staff

was created to organize all domain users.

Departments inside the organization:

HR

Finance

IT

Users
HR Department

Yazeed Ahmad

Finance Department

Sara Ahmad

IT Department

Mohammad Ahmad

Haya Ahmad

Yousef Ahmad

Groups

A security group was created:

Deny GPO

Purpose:

Prevent IT members from being affected by specific Group Policy Objects (GPOs).

Client Computer

Client VM configuration:

User logged in:

Sara Ahmad – Finance Department

Configuration:

Computer joined to domain moon.com

User authenticated through Active Directory

Group Policy Configuration

A Group Policy Object (GPO) was created to restrict system functionality.

Policy Applied

Task Manager access is disabled for users.

Purpose:

Prevent users from terminating system processes

Improve workstation control

Shared Folder Setup

Shared folder created:

Calc

The folder contains a file that opens the Calculator application.

Access Permissions
Department	Permission
HR	Read & Execute
Finance	Read
IT	Full Control

Rules:

All users can open the file

Only IT members can modify the folder

Skills Demonstrated

This project demonstrates the following IT administration skills:

Active Directory Domain Services

Domain Controller configuration

Organizational Units (OU)

User and Group management

Group Policy Management

File server permissions

Domain joining

Virtual lab environment using VirtualBox

Project Team

Lana

Qasem

Omar Alfaroq
