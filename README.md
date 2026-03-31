**Active Directory Lab**

I built this hands-on Windows Server lab in Oracle VM VirtualBox to practice core Active Directory administration tasks. This shows domain controller setup, static IP configuration, DNS configuration, organizational unit design, user and group administration, and Group Policy security settings.

Lab Objectives
- Install Windows Server in Oracle VM VirtualBox
- Promote the server to a domain controller
- Configure a static IPv4 address and DNS settings
- Create organizational units for departments
- Create users and assign them to groups
- Review password policy and account lockout settings

Virtual Lab Environment

I built this lab in Oracle VM VirtualBox using Windows Server 2022 to create an isolated practice environment. This shows how virtualization supports server deployment and Active Directory administration.

<img src="images/Oracle VM VirtualBox Manager.png" alt="Oracle VM VirtualBox Manager" width="700"/>

Network Configuration

I configured a static IPv4 address before promoting the server to a domain controller. This shows how stable addressing supports DNS and Active Directory services.

<img src="images/Internet Protocol Version 4 Properties.png" alt="Internet Protocol Version 4 Properties" width="700"/>

Network Verification

I verified the IPv4 address, subnet mask, and default gateway after assigning the static address. This shows that the server network settings were correctly applied before domain services were installed.

<img src="images/Network Connection Detals.png" alt="Network Connection Details" width="700"/>

Active Directory Structure

I created organizational units to separate departments and organize objects inside the domain. This shows how directory structure supports clean administration.

<img src="images/AD Users and Computers.png" alt="AD Users and Computers" width="700"/>

Group Membership Management

I assigned user accounts to security groups to simulate role-based administration. This shows how permissions are organized through group membership.

<img src="images/User Properties Active Directory.png" alt="User Properties Active Directory" width="700"/>

Group Policy Configuration

I reviewed and configured password policy settings to strengthen account security across the domain. This shows how Group Policy supports centralized security control.

<img src="images/Group Policy Management Editor.png" alt="Group Policy Management Editor" width="700"/>

Skills Practiced
- Windows Server installation
- Active Directory domain services
- DNS configuration
- Static IP assignment
- Organizational unit design
- User and group administration
- Group Policy review

Summary

This lab demonstrates practical Windows Server administration in a virtual environment. It shows how core infrastructure tasks connect across identity, networking, and security management in entry-level systems administration work.

Navigation

[`Back to GitHub Profile`](https://www.github.com/cbueker-it)
