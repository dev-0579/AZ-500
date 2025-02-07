- Secure user identities in Microsoft Entra ID to prevent unauthorized access and protect user accounts.
- Implement security measures to protect groups in Microsoft Entra ID, ensuring proper access control and group management.
- Make informed recommendations on when to use external identities and how to securely manage them.
- Implement security measures to protect external identities, maintaining confidentiality and integrity.
- Implement Microsoft Entra ID Protection to proactively identify and respond to identity-related security threats and vulnerabilities.

#

#

### cloud-based identity and access management service

#

#

Automate user provisioning between your existing Windows Server AD and your cloud apps, including Microsoft 365

- IT admins use Microsoft Entra ID to control access to apps and app resources
- App developers can use Microsoft Entra ID as a standards-based authentication
- Microsoft 365, Office 365, Azure, or Dynamics CRM Online subscribers already use Microsoft Entra ID

#

#

- Microsoft Entra ID Free
- Microsoft Entra ID P1
- Microsoft Entra ID P2
- Pay as you go" feature license



#

#

Which features work in Microsoft Entra ID?

- Application management
- Authentication
- Microsoft Entra ID for developers
- Business-to-Business (B2B)
- Business-to-Customer (B2C)
- Conditional Access
- Device Management
- Domain services
- Enterprise users
- Hybrid identity
- Identity governance
- Identity protection
- Managed identities for Azure resources
- Privileged identity management (PIM)
- Monitoring and health	
- Workload identities	

#

#

Single tenant\
Azure tenants that access other services in a dedicated environment are considered single tenant.

Multitenant\
Azure tenants that access other services in a shared environment, across multiple organizations, are considered multitenant.

MSA\
Microsoft account (Outlook, OneDrive, Xbox LIVE, or Microsoft 365)


#

#

#

### Secure Microsoft Entra users

#

#

![image](https://github.com/user-attachments/assets/aab87c69-bc5a-45ff-938f-eff5e1943f4b)



#

#

**Internal member**: most likely full-time employees in your organization.

**Internal guest**: have account in your tenant, guest-level privileges. Created within your tenant prior to the availability of B2B collaboration.

**External member**: users authenticate using external account, have member access to your tenant. Common in multitenant organizations.

**External guest**: users are true guests of your tenant who authenticate using an external method and who have guest-level privileges

#

#

### Secure Microsoft Entra groups

#

#

Some groups can't be managed in the Azure portal:

- Groups synced from on-premises Active Directory can be managed only in on-premises Active Directory.
- Distribution lists and mail-enabled security groups are managed only in Exchange admin center or Microsoft 365 admin center.


#

#

### How access management in Microsoft Entra ID works

#

![image](https://github.com/user-attachments/assets/90b80b27-0ff3-472f-85ea-2d3dfcf049e5)


#

#

Ways to assign access rights


- Direct assignment

- Group assignment

- Rule-based assignment

- External authority assignment. Access comes from an external source, such as an on-premises directory or a SaaS app

#

Can users join groups without being assigned?

The group owner can let users find their own groups to join, instead of assigning them

The owner can also set up the group to automatically accept all users that join or to require approval

If you have multiple owners and one of them disapproves, the user is notified, but isn't added to the group


#

#

**Recommend when to use external identities**

- Microsoft Entra B2B

- The partner uses their own identities and credentials, whether or not they have a Microsoft Entra account

For B2B collaboration with other Microsoft Entra organizations, use cross-tenant access settings.

Cross-tenant access settings, you can also trust multi-factor (MFA) and device claims (compliant claims and Microsoft Entra hybrid)


#

#

Easily invite guest users from the Azure portal

#

Allow self-service sign-up

#

Let application and group owners manage their own guest users

#

#

### Secure external identities

Microsoft Entra entitlement management, an identity governance feature that lets you manage identity and access for external users

Automating access request workflows, access assignments, reviews, and expiration

#

#

**Workforce tenant configuration** is a standard Microsoft Entra tenant that contains your employees, internal business apps, and other organizational resources. 

In a workforce tenant, your internal users can collaborate with external business partners and guests using B2B collaboration.

**External tenant configuration** is used exclusively for apps you want to publish to consumers or business customers. 

It contains your app registrations and a directory of consumer or customer accounts.


#

#

**B2B direct connect**

**Shared channel** owner can search within Teams for allowed users from the external organization and add them to the shared channel.

**External users** access Teams shared channel without having to switch organizations or sign in with a different account. 

External user can access files and apps through the Files tab. The shared channel’s policies determine the user’s access.


#

#

#

### Implement Microsoft Entra Identity protection

#

![image](https://github.com/user-attachments/assets/617c87f3-870e-4c0f-83a7-f941a355a0a9)

#

Detect risks

Investigate

Automatic remediation


#

Required roles

Identity Protection requires users be assigned one or more of the following roles in order to access.


**Security Administrator**	Full access to Identity Protection

**Security Operator**	View all Identity Protection reports and Overview, Dismiss user risk, confirm safe sign-in, confirm compromise

**Security Reader**	View all Identity Protection reports and Overview

**Global Reader**	Read-only access to Identity Protection

**User Administrator**	Reset user passwords

Currently, **Security Operator role can't access the Risky sign-ins report**.

**Requires Microsoft Entra ID P2 license**


#

#


Check your knowledge

#

<img width="668" alt="image" src="https://github.com/user-attachments/assets/fb3ed206-bb3c-4e8b-a42d-f34fe6e66bbb" />


#

<img width="663" alt="image" src="https://github.com/user-attachments/assets/37513697-b3e5-4c6e-a900-ae85077b4a50" />

#

<img width="668" alt="image" src="https://github.com/user-attachments/assets/7e8d51cd-7690-4f8e-8d69-701aa64fae40" />

#

<img width="668" alt="image" src="https://github.com/user-attachments/assets/7effa0c8-ea7d-4206-b5dd-159330a83b77" />

#

<img width="672" alt="image" src="https://github.com/user-attachments/assets/57d88c05-ff29-4e20-b6b9-aa782a626adb" />







