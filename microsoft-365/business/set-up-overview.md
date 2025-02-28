---
title: "Overview of set up"
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- 'O365E_M365SetupBanner'
- 'BCS365_M365SetupBanner'
ms.service: o365-administration
localization_priority: Normal
ms.collection: 
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: "Overview of the set up steps for Microsoft 365 Business."
---

# Overview of setup

Most of the set up steps can be done in the setup wizard, but the other options are also listed.


## Step 1: Add your domain and users

   - **[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)

    - **Add users**. You can do this in any of the three ways:
        - In the [wizard](set-up.md#add-users-in-the-wizard).
        - Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.
        - You can also [add users later](add-users-m365b.md) in the admin center.
## Step 2: Set up security policies and configure devices 

  - Use the [Setup wizard](set-up.md#protect-data-and-devices) to configure device and security policies. 
  - You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:

      - **Email malware protection**
      - **Advanced Threat Protection (ATP) Safe links**
      - **ATP Safe Attachments**
      - **ATP anti-phishing**
      - **Exchange Online Archiving**
      - **Data Loss Prevention (DLP)**
      - **Azure Information Protection (Plan1**)

          To get started see, [set up advanced security policies](set-up-advanced-security.md).

        See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.

## Step 3: Set up and manage Windows 10 devices

   When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.

   - Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - Use the [Setup wizard](set-up.md#protect-data-and-devices) to configure policies for Windows 10 devices.

## Stes 4: Install Office 365 Business
- You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).
- Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.
- Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.
     
## Advanced
- **Use Autopilot to set up new devices**
            
     You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you. You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.

- **Access on-premises resources**

     - If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication. Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up. This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.

    - If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).

  