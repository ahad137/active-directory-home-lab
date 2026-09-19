# Windows Server & Active Directory Home Lab

A hands-on Windows Server home lab focused on Active Directory administration, Group Policy, file services, access control, and Windows security.

This project is being built through practical implementation and testing in a virtualized lab environment.

---

## 🖥️ Lab Environment

| Component | Details |
|---|---|
| Server | Windows Server 2022 |
| Client | Windows 10/11 |
| Virtualization | VMware / Virtual Machine |
| Directory Service | Active Directory Domain Services |
| Management | Group Policy |
| File Services | Windows File Server |
| Resource Management | FSRM |

---

## 🎯 Project Objectives

The goal of this project is to build and administer a small enterprise-style Windows environment and gain practical experience with:

- Active Directory Domain Services
- Users, Groups and Organizational Units
- Group Policy
- Domain-joined Windows clients
- Windows file sharing
- NTFS and Share permissions
- Permission inheritance
- Effective permissions
- Mapped network drives
- File Server Resource Manager (FSRM)
- Access-Based Enumeration (ABE)
- Security policies
- Service accounts
- Windows security monitoring
- SIEM integration

---

# 🏗️ Lab Architecture

```text
                    Windows Server 2022
                   ┌─────────────────────┐
                   │  Active Directory   │
                   │  Domain Controller  │
                   │  File Server        │
                   │  GPO / FSRM         │
                   └──────────┬──────────┘
                              │
                         Domain Network
                              │
                   ┌──────────▼──────────┐
                   │   Windows Client    │
                   │    Domain Joined    │
                   └─────────────────────┘

1. Active Directory
Installed Active Directory Domain Services
Created the Active Directory domain
Configured the Domain Controller
Created Organizational Units
Created domain users
Created security groups
Joined the Windows client to the domain
2. Group Policy
Created and configured Group Policy Objects
Linked GPOs to Organizational Units
Tested GPO application from the domain client
3. File Sharing & Permissions
Created shared folders
Configured Share permissions
Configured NTFS permissions
Tested user access from the domain client
Implemented mapped network drives
Configured GPO-based drive mapping
Tested mapped drive persistence after restart/logon
4. File Server Resource Manager
Implemented FSRM
Configured and tested FSRM functionality
🚧 In Progress

The following areas are currently being implemented and tested:

Advanced NTFS permissions
Permission inheritance
Effective permissions
Access-Based Enumeration
Security policies
Service accounts
🔜 Planned

The lab will later be extended into a Windows security monitoring environment.

Planned components:

Windows Event Logs
Sysmon
PowerShell logging
Security event analysis
Splunk
Wazuh
Detection rules
Incident investigation
📚 Documentation

Each major component of the lab will be documented with:

Objective
Configuration
Implementation
Testing
Results
Screenshots

The purpose is to demonstrate practical implementation rather than simply completing tutorials.

🔐 Security Focus

The long-term goal is to connect Windows administration with security monitoring:

Active Directory
       ↓
Windows Clients
       ↓
GPO / Permissions / File Services
       ↓
Windows Event Logs
       ↓
Sysmon
       ↓
Splunk / Wazuh
       ↓
Detection
       ↓
Investigation
       ↓
Incident Documentation
