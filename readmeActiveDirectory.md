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
* CLIENT02 (planned)

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

### Networking

* DHCP Configuration
* DNS Configuration
* IP Address Management
* Client-to-Server Connectivity
* Domain Authentication

---

## Screenshots

### Active Directory Deployment

*Add screenshots here*

### DNS Configuration

*Add screenshots here*

### DHCP Scope Configuration

*Add screenshots here*

### Domain Join Process

*Add screenshots here*

### Domain User Authentication

*Add screenshots here*

---

## Future Enhancements

* Implement Group Policy Objects (GPOs)
* Create Security Groups
* Configure Folder Redirection
* Add Additional Domain-Joined Clients
* Implement Password Policies
* Create DHCP Reservations
* Deploy Shared Network Resources

---

## Author

Built as part of a hands-on Windows Server and Networking lab focused on enterprise infrastructure administration.
