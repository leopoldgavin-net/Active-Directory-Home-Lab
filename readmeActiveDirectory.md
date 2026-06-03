# Active Directory Home Lab

## Overview

This project demonstrates the deployment and configuration of a Windows-based enterprise environment using VMware Workstation. The lab simulates a small business network and includes Active Directory, DNS, DHCP, domain-joined clients, and centralized user management.

The goal of this project is to gain hands-on experience with common Windows Server administration tasks used in Help Desk, Systems Administration, Infrastructure Support, and IT Operations roles.

---

## Lab Environment

### Hypervisor

* VMware Workstation Pro

### Server

* Windows Server 2022
* Domain Controller (DC01)
* Active Directory Domain Services (AD DS)
* DNS Server
* DHCP Server

### Clients

* Windows 11 Pro
* CLIENT01
* CLIENT02 (Planned)

---

## Network Architecture

```text
VMware Workstation
        |
      VMnet1
        |
 ┌─────────────┐
 │    DC01     │
 │192.168.60.10
 │AD / DNS / DHCP
 └──────┬──────┘
        |
 ┌─────────────┐
 │  CLIENT01   │
 │192.168.60.101
 └─────────────┘
```

---

## Network Configuration

### Domain Information

| Setting           | Value                           |
| ----------------- | ------------------------------- |
| Domain Name       | corp.local                      |
| Domain Controller | DC01                            |
| Server IP         | 192.168.60.10                   |
| DHCP Scope        | 192.168.60.100 - 192.168.60.200 |

### Services Configured

* Active Directory Domain Services
* DNS
* DHCP
* Organizational Units (OUs)
* User Management
* Domain Authentication

---

## Active Directory Structure

### Organizational Units

* IT
* HR
* Computers

### Users

* gleopold

### Domain Computers

* CLIENT01

---

## Project Objectives

* Deploy Windows Server 2022
* Configure a Domain Controller
* Install and configure Active Directory
* Configure DNS for domain name resolution
* Configure DHCP for automatic IP assignment
* Create Organizational Units and users
* Join Windows clients to the domain
* Validate centralized authentication

---

## Skills Demonstrated

### Windows Administration

* Active Directory Administration
* User and Group Management
* Organizational Unit Management
* Domain Services Deployment
* DNS Administration
* DHCP Administration
* Domain Controller Deployment
* Domain Join Management

### Networking

* DHCP Configuration
* DNS Configuration
* IP Address Management
* Client-to-Server Connectivity
* Domain Authentication
* Network Troubleshooting

---

## Deployment Process

### 1. Windows Server Installation

* Installed Windows Server 2022
* Assigned static IP address
* Renamed server to DC01

### 2. Active Directory Deployment

* Installed Active Directory Domain Services
* Promoted server to Domain Controller
* Created the corp.local domain

### 3. DNS Configuration

* Configured DNS service
* Verified Forward Lookup Zone creation
* Validated name resolution for domain resources

### 4. DHCP Configuration

* Created DHCP scope
* Configured DNS options
* Authorized DHCP server
* Validated automatic client address assignment

### 5. Active Directory Administration

* Created Organizational Units
* Created domain users
* Managed computer objects

### 6. Client Deployment

* Installed Windows 11 Pro
* Joined CLIENT01 to corp.local
* Verified domain authentication

---

## Screenshots

### 1. Active Directory Domain Deployment

Successful deployment of the corp.local Active Directory domain.

![Active Directory Domain](screenshots/01-active-directory-domain.png)

---

### 2. Organizational Unit Structure

Custom Organizational Units created for administrative organization.

![OU Structure](screenshots/02-ou-structure.png)

---

### 3. User Account Creation

Domain user account created within the IT Organizational Unit.

![User Account](screenshots/03-user-account.png)

---

### 4. DNS Configuration

Forward Lookup Zone configured for corp.local.

![DNS Configuration](screenshots/04-dns-zone.png)

---

### 5. DHCP Scope Configuration

DHCP scope configured to automatically assign IP addresses to clients.

![DHCP Scope](screenshots/05-dhcp-scope.png)

---

### 6. DHCP Lease Assignment

CLIENT01 successfully receiving network configuration from DC01.

![DHCP Lease](screenshots/06-client-ipconfig.png)

---

### 7. Domain Join Success

CLIENT01 successfully joined to the corp.local domain.

![Domain Join](screenshots/07-domain-join-success.png)

---

### 8. Computer Object in Active Directory

CLIENT01 created and managed as an Active Directory computer object.

![Computer Object](screenshots/08-client01-ad-object.png)

---

### 9. Domain User Authentication

Successful authentication using a domain user account.

![Domain Login](screenshots/09-domain-login.png)

---

## Key Takeaways

One of the most important lessons from this project was understanding the dependency chain within enterprise environments:

```text
Networking
    ↓
DHCP
    ↓
DNS
    ↓
Active Directory
    ↓
Authentication
```

The project demonstrated how Active Directory relies heavily on DNS and networking services. Successful domain joins and user authentication depend on proper DHCP configuration, DNS resolution, and communication with the Domain Controller.

---

## Future Enhancements

* Implement Group Policy Objects (GPOs)
* Create Security Groups
* Configure Folder Redirection
* Add CLIENT02 to the domain
* Implement Password Policies
* Configure DHCP Reservations
* Deploy Shared Network Resources
* Configure Network File Shares
* Implement Role-Based Access Control (RBAC)

---

## Author

Built as a hands-on Windows Server and Networking project focused on enterprise infrastructure administration, Active Directory, DNS, DHCP, and domain-based authentication.
