# Active Directory Home Lab

A hands-on Active Directory home lab built with Windows Server 2022 and a Windows 10 client to practice enterprise identity management, organizational structure, Group Policy, authentication, authorization, and Windows administration.

## Lab Environment

- Windows Server 2022
- Windows 10 Client
- VMware Workstation
- Active Directory Domain Services (AD DS)
- DNS
- Group Policy Management
- Active Directory Users and Computers (ADUC)

## Domain

```text
AHAD.local
Active Directory Structure
AHAD.local
│
├── Asia
├── Europe
├── USA
│   ├── Computers
│   ├── Server
│   └── Users
│       ├── HR
│       ├── IT
│       └── SALES
│
└── Domain Controllers

The lab uses Organizational Units (OUs) to organize users, computers, and servers according to their role and department.

Users and Security Groups

Created and managed:

Domain users
Department-based user organization
Security groups
HR group
User membership in security groups
User and group management through ADUC

Example:

USA
└── Users
    ├── HR
    ├── IT
    └── SALES
Domain-Joined Client

A Windows 10 workstation was joined to the AHAD.local domain.

Domain: AHAD.local
Client: COMP01

The client was successfully managed as a domain member through Active Directory.

Group Policy

Multiple Group Policy Objects (GPOs) were created and tested.

Account Lockout Policy

Configured account lockout settings to control repeated failed authentication attempts.

Password Policy

Configured domain password-related security settings.

Desktop Wallpaper

Configured a centralized desktop wallpaper policy through Group Policy.

Drive Mapping

Configured network drive mapping through Group Policy.

Restrict Control Panel

Configured a policy to restrict access to Control Panel.

User Rights Assignment

Configured user rights policies, including logon restrictions.

Example:

Deny Log on Locally
        ↓
GG-HR

This was used to understand how security groups can be incorporated into Windows user-rights policies.

GPO Scope and Troubleshooting

Practiced understanding the difference between:

User Configuration
Computer Configuration
User OU placement
Computer OU placement
GPO linking
Security Group membership
Group Policy scope

GPO application was tested using:

gpupdate /force

and verified using:

gpresult /r
Active Directory Administration

Practical administration tasks included:

Creating Organizational Units
Creating users
Creating security groups
Organizing users by department
Managing computer objects
Joining a Windows client to the domain
Managing Group Policy
Testing policy application
Troubleshooting GPO behavior
Security Concepts Practiced

This lab provided hands-on practice with:

Authentication
Authorization
Security groups
User rights
Password policies
Account lockout
Access control
Group Policy
Domain administration
Screenshots

Screenshots in this repository document the actual configurations and tests performed during the lab.

Project Outcome

This project provided practical experience administering a Windows Active Directory environment, including domain users, Organizational Units, security groups, domain-joined clients, Group Policy, and Windows security controls.

Future Security Integration

The Active Directory environment can later be used as a Windows enterprise environment for generating and investigating security telemetry through SIEM and EDR technologies.


