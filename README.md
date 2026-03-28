# Active Directory Lab

This project documents a hands-on Windows Server lab built in Oracle VM VirtualBox to practice core Active Directory administration tasks. The lab includes domain controller setup, static IP configuration, DNS configuration, organizational unit design, user and group administration, and Group Policy security settings.

Lab Objectives
- Install Windows Server in Oracle VM VirtualBox
- Promote the server to a domain controller
- Configure a static IPv4 address and DNS settings
- Create organizational units for departments
- Create users and assign them to groups
- Review password policy and account lockout settings

Virtual Lab Environment

This lab was built in Oracle VM VirtualBox using Windows Server 2022. The virtual machine provided an isolated environment for practicing server deployment and Active Directory administration.

<img src="images/Oracle VM VirtualBox Manager.png" alt="Oracle VM VirtualBox Manager" width="700"/>
Network Configuration

A static IPv4 address was configured before promoting the server to a domain controller. This ensures reliable communication for DNS and Active Directory services.

<img src="images/Internet Protocol Version 4 Properties.png" alt="Internet Protocol Version 4 Properties" width="700"/>
Network Verification

After assigning the static address, network details were reviewed to confirm the IPv4 address, subnet mask, and default gateway.

<img src="images/Network Connection Detals.png" alt="Network Connection Details" width="700"/>
Active Directory Structure

Organizational units were created to separate departments and organize administrative objects inside the domain.

<img src="images/AD Users and Computers.png" alt="AD Users and Computers" width="700"/>
Group Membership Management

User accounts were assigned to security groups to simulate role-based administration inside the domain.

<img src="images/User Properties Active Directory.png" alt="User Properties Active Directory" width="700"/>
Group Policy Configuration

Password policy settings were reviewed and configured to strengthen account security across the domain.

<img src="images/Group Policy Management Editor.png" alt="Group Policy Management Editor" width="700"/>

Skills Practiced
- Windows Server installation
- Active Directory domain services
- DNS configuration
- Static IP assignment
- Organizational unit design
- User and group administration
- Group Policy review
- Summary

This lab demonstrates practical experience with Windows Server administration in a virtual environment. It connects core infrastructure tasks that are commonly used in entry-level IT support and systems administration roles.
