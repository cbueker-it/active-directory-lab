**Active Directory Lab**

Active Directory gives system administrators one central place to manage users, groups, access, and security policies. Because of that, it is a core part of many business environments. Without a centralized structure for the user directory, management can become inconsistent, permissions can be harder to control and standardize, and security settings can vary across the business.

I built this hands-on Windows Server lab in Oracle VM VirtualBox to practice solving these problems in a controlled environment. I configured the server and network, organized Active Directory users and organizational units, assigned users to security groups, and applied domain password policy. Finally, I used PowerShell from the command line to validate the configuration and confirm that the system was working as expected. This lab focuses on the connection between user identity, access control, networking, and security administration.

**Lab Objectives**

- Build a Windows Server virtual machine and promote it to a domain controller
- Configure a static IPv4 address and DNS settings
- Create and organize Active Directory organizational units and user accounts
- Create security groups and assign users to the appropriate groups
- Configure domain password policy and validate Active Directory settings with PowerShell

**Static Network Configuration**

- Configured a static IPv4 address for the Windows Server domain controller.
- Defined the subnet mask and default gateway for consistent network connectivity.
- Configured the server to use its local DNS service for Active Directory name resolution.

![Static Network Configuration](./images1/01-static-networking.png)


**Network Configuration Validation**

- Verified that DHCP was disabled and the server was using a static network configuration.
- Confirmed the assigned IPv4 address, subnet mask, and default gateway.
- Validated the active Ethernet adapter configuration through Windows Network Connection Details.

![Network Configuration Validation](./images1/02-network-validation.png)


**Active Directory Directory Structure**

- Organized Active Directory objects within the `Corporate` organizational unit.
- Created departmental OUs for Finance, HR, IT, Computers, Groups, and Users.
- Added user accounts to establish a structured directory environment for centralized administration.

![Active Directory Directory Structure](./images1/03-directory-structure.png)


**Helpdesk Group Membership**

- Assigned the Christopher Baker user account to the `Helpdesk-Tier1` security group.
- Used security-group membership to support role-based access control rather than assigning permissions directly to individual users.
- Maintained the default `Domain Users` membership while adding the helpdesk role.

![Helpdesk Group Membership](./images1/04-group-membership.png)


**Domain Password Policy**

- Configured password policy through the Default Domain Policy in Group Policy Management.
- Enforced password history, password-age requirements, and a minimum password length.
- Enabled password complexity requirements and disabled reversible password encryption.

![Domain Password Policy](./images1/05-password-policy.png)


**Active Directory User Validation**

- Used PowerShell Active Directory cmdlets to validate domain information and user-account configuration.
- Confirmed the `cbaker` account name and enabled status.
- Queried the user's Active Directory security-group membership from the command line.

![Active Directory User Validation](./images1/06-ad-user-membership-validation.png)


**Helpdesk Tier-1 Group Validation**

- Verified the Christopher Baker account and its distinguished Active Directory location with PowerShell.
- Queried the `Helpdesk-Tier1` security group and confirmed its assigned user accounts.
- Validated the Active Directory domain name, NetBIOS name, and domain functional mode.

![Helpdesk Tier-1 Group Validation](./images1/07-helpdesk-tier1-group-validation.png)

**Lessons Learned**

- I learned that a centralized directory makes it easier to manage users, groups, and security settings consistently within a business environment.
- I learned that organizational units help keep users and resources structured in a way that makes them much easier for system administrators to manage.
- I learned that security groups make access control easier to standardize compared to assigning permissions directly to individual end-user accounts and devices.
- I learned how network and DNS configuration come into play because Active Directory depends on reliable communication between networks and systems.
- I got to use PowerShell and see how useful it is for validating Active Directory settings and confirming that users, groups, and domain information are configured correctly.

Summary

This lab brought together the core pieces of Active Directory administration in one working environment. I configured the server and network, organized users and groups, applied security policy, and used PowerShell to validate the final configuration. The project helped reinforce how identity, access control, networking, and security settings work together to support a centralized Windows business environment.

Navigation

[`Back to GitHub Profile`](https://www.github.com/cbueker-it)
