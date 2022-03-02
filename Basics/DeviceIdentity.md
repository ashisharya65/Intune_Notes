## Device Identity in Azure AD 

### What is a device identity?

A device identity is an object in Azure Active Directory (Azure AD). This device object is similar to users, groups, or applications. A device identity gives administrators information they can use when making access or configuration decisions.

There are three ways to get a device identity:

- Azure AD registration
- Azure AD join
- Hybrid Azure AD join

Device identities are a prerequisite for scenarios like device-based Conditional Access policies and Mobile Device Management with Microsoft Endpoint Manager (Intune).

Users are identified based on their credentials, where as devices are identified by certificates. In other words, a device certificate represents the device registered to Azure AD. These certificates are created during the registration process.

### Modern device scenario
The modern device scenario focuses on two of these methods:

 - Azure AD registration
    - Bring your own device (BYOD)
    - Mobile device (cell phone and tablet)
 - Azure AD join
    - Windows 11 and Windows 10 devices owned by your organization
    - Windows Server 2019 and newer servers in your organization running as VMs in Azure

Hybrid Azure AD join is seen as an interim step on the road to Azure AD join. Hybrid Azure AD join provides organizations support for downlevel Windows versions back to Windows 7 and Server 2008. All three scenarios can coexist in a single organization.


### Join Types

There are three different registration types, which are called Join Types.

|          JoinTypes            |              Purpose              |
|-------------------------------|-----------------------------------|
| Registered|Devices that are Azure AD registered are typically personally owned or mobile devices and are signed in with a personal Microsoft account or another local account.
|Joined | Devices that are Azure AD joined are owned by an organization and are signed in with an Azure AD account belonging to that organization. They exist only in the cloud.
| Hybrid Joined	|Devices that are hybrid Azure AD joined are owned by an organization and are signed in with an Active Directory Domain Services account belonging to that organization. They exist in the cloud and on-premises.

