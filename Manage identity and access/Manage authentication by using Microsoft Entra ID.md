- Configure Microsoft Entra Verified ID to establish a trusted identity verification process
- Implement multifactor authentication (MFA) to add an extra layer of security for user authentication
- Implement passwordless authentication to provide a more convenient and secure login experience
- Implement password protection measures to safeguard against password-related security risks
- Implement single sign-on (SSO) to simplify user access to multiple applications and services
- Integrate SSO with identity providers to facilitate seamless access across various platforms
- Recommend and enforce modern authentication protocols to enhance security and user experience


#

#

### Microsoft Entra connect features

#

- Password hash synchronization
- Pass-through authentication
- Federation integration
- Synchronization
- Health Monitoring


#

- Enhanced security
- Get alerted on all critical ADFS system issues
- Easy to deploy and manage
- Rich usage metrics
- Great user experience



#

#

### Microsoft Entra Cloud Sync

#

Features

- Connect to single on-premises AD forest
- Connect to multiple on-premises AD forests
- Connect to multiple disconnected on-premises AD forests
- Lightweight agent installation model
- Multiple active agents for high availabilit
- Support for user objects
- Support for group objects
- Support for contact objects
- Allow basic customization for attribute flows
- Synchronize Exchange online attributes
- Synchronize extension attributes 1-15
- Synchronize customer defined AD attributes (directory extensions)
- Support for Password Hash Sync
- Support for federation
- Seamless Single Sign-on
- Supports installation on a Domain Controller
- Support for Windows Server 2016
- Filter on Domains/OUs/groups
- Allow minimal set of attributes to be synchronized (MinSync)
- Allow removing attributes from flowing from AD to Microsoft Entra ID
- Support for password writeback
- Support for group writeback
- Exchange hybrid writeback
- Support for up to 150,000 objects per AD domain
- Groups with up to 50,000 members
- Cross domain references
- On-demand provisioning
Support for US Government



#

#

### Authentication options

Authentication method you choose, is configured by using **Microsoft Entra Connect**, which also provisions users in the cloud


#

**Federated authentication**

#

![image](https://github.com/user-attachments/assets/9c32b22c-0002-4584-a5ca-886a03b5d3f8)

#

#

Microsoft Entra ID can 

- handle sign-in for users without relying on on-premises components to verify passwords
- hand off user sign-in to a trusted authentication provider such as Microsoft's AD FS

Microsoft Entra ID requires some on-premises components for user-level Active Directory security policies 

- account expired, disabled account, password expired, account locked out, sign-in hours on each user sign-in


Sign-in features **not natively supported** by Microsoft Entra ID:

- Sign-in using third-party authentication solution
- Multi-site on-premises authentication solution

#

**Microsoft Entra ID Protection** 

- requires **Password Hash Sync** regardless of which sign-in method
- Organizations can **fail over to Password Hash Sync** if their primary sign-in method fails and it was configured before the failure event



#

#

**Microsoft Entra Conditional Access** require **Microsoft Entra ID P1** licenses.

#

#

### Architecture diagrams

#

#

![image](https://github.com/user-attachments/assets/75102627-2ac5-4b36-9a68-7fabc5906e39)

#

#

![image](https://github.com/user-attachments/assets/161a2582-1b70-4a6d-be3b-657f7bd49ab0)

#

#

![image](https://github.com/user-attachments/assets/3b252478-73dc-41f1-8ff0-e242e11d9758)

#

#

**Recommendations**

High availability and disaster recovery

On-premises outage survival

Identity protection (Microsoft Entra ID Protection with Microsoft Entra ID P2)


#

#

#

### Password hash synchronization with Microsoft Entra ID

#

Only new leaked credentials found after enable PHS will be processed against tenant\
Verifying against previously found credential pairs is not performed

Set up password hash synchronization as a backup if decide to use Federation with Active Directory Federation Services (AD FS) as your sign-in method

To use password hash synchronization in your environment, you need to:

1. Install Microsoft Entra Connect
2. Configure directory synchronization between your on-premises Active Directory instance and your Microsoft Entra instance
3. Enable password hash synchronization











































