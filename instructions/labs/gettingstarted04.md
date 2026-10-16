# Day 4 – Advanced Mobility Solutions in Microsoft Intune Suite

### Overall Estimated Duration: 4 Hours

## Overview

In this hands-on lab, you will secure mobile access and data for managed and unmanaged devices. You will configure and validate device compliance, create app protection policies that keep corporate data safe in apps on iOS and iPadOS, and then configure Microsoft Tunnel VPN profiles for Android and iOS devices. Along the way, you will learn about Microsoft Tunnel architecture, MDM and MAM Tunnel scenarios, and Microsoft Cloud PKI for certificate-based access.

**Scenario:** Contoso employees use Windows, iOS and Android devices to reach company email and internal resources. The security team wants only compliant devices to reach email, wants corporate data in Outlook protected on iPhones and iPads, and wants VPN settings delivered to Android and iOS devices automatically. As the Contoso Intune administrator, you set all three up.

## Objectives

In this lab, you will:

- Configure and validate device compliance, and use it in a Conditional Access policy.
- Configure app protection policies for iOS and iPadOS devices.
- Configure Microsoft Tunnel and a VPN policy for Android devices.
- Configure a VPN policy for iOS and iPadOS devices.

## Pre-requisites

Participants should have:

- A basic understanding of Microsoft Intune and Microsoft Entra ID, including users, groups and device enrollment.
- A basic understanding of iOS/iPadOS and Android Enterprise management.
- Familiarity with VPN concepts and certificate-based authentication.
- Awareness of Microsoft Entra Conditional Access and how device compliance affects access.

**Your lab environment already provides:**

- A Microsoft 365 tenant with Microsoft Intune. You sign in with the **Username** and **Temporary Access Pass** shown on the **Environment** tab. This account is a Global Administrator.
- **LabVM**, a Windows Server virtual machine that opens in your browser. Use it for the Microsoft Intune admin center and for the "unmanaged device" test.
- **TestVM**, a Windows 11 Enterprise virtual machine. You reach it with Remote Desktop from LabVM, using the **TestVM Private IP**, **LabVM Admin Username** and **LabVM Admin Password** from the Environment tab.
- **Demo User 01**, the test user for the compliance and Conditional Access labs. Its user name and Temporary Access Pass are shown on the **Environment** tab as **User 01 UPN** and **User 01 Password**. The user is licensed for Microsoft Intune, Microsoft Entra ID P1 and Exchange Online.

**You do not need:** an iPhone, iPad or Android device (steps that use one are marked optional), or a Linux server. Labs 19 and 20 create the Microsoft Tunnel configuration only.

> **Note:** Each lab runs in its own new tenant. Nothing from Days 1 to 3 exists in it, so each lab starts with a short preparation task where it needs one.

## Architecture

This architecture demonstrates an end-to-end workflow for secure mobility. Devices are evaluated against compliance policies, and Conditional Access uses the compliance result to allow or block access to email. App protection policies secure corporate data inside managed apps. VPN profiles deliver Microsoft Tunnel connectivity to Android and iOS devices, giving enrolled (MDM Tunnel) and unenrolled (MAM Tunnel) devices secure access to on-premises resources, with Microsoft Cloud PKI supporting certificate-based authentication.


## Explanation of Components

The architecture for this lab involves the following key components:

- **Mobile Devices:** Represent the iOS and Android devices that receive compliance, app protection, and VPN policies.

- **Microsoft Intune:** Deploys compliance policies, app protection policies, and VPN profiles to devices.

- **Compliance Policies:** Define requirements such as minimum OS version and antimalware for devices.

- **Conditional Access:** Uses device compliance to allow or block access to Exchange Online.

- **App Protection Policies (MAM):** Protect corporate data within managed apps, for example by restricting copy/paste.

- **Microsoft Tunnel:** A VPN gateway for Intune that gives iOS and Android devices secure access to on-premises apps and resources.

- **MDM Tunnel:** Tunnel connectivity for devices fully enrolled in Intune, delivered through VPN profiles.

- **MAM Tunnel:** Tunnel connectivity for unenrolled devices, scoped to protected apps such as Microsoft Edge.

- **VPN Profiles:** Intune configuration profiles that deploy VPN connection settings to Android and iOS devices.

- **Microsoft Cloud PKI:** A cloud-based certificate authority in the Intune Suite that issues and manages device certificates.

## Getting Started with the Lab

### Accessing Your Lab Environment

Once you're ready to dive in, your virtual machine and **Guide** will be right at your fingertips within your web browser.

![Image](media/n1.png)

### Virtual Machine & Lab Guide

Your virtual machine is your workhorse throughout the workshop. The guide is your roadmap to success.

### Exploring Your Lab Resources

To get a better understanding of your lab resources and credentials, navigate to the **Environment** tab.

![Image](media/gs3.png)

### Managing Your Virtual Machine

Feel free to **start, restart, or stop (2)** your virtual machines as needed from the **Resources (1)** tab. LabVM has an **open in new window** button; TestVM does not, so you open it from LabVM (see Lab 17).

![Image](./media/gs5.png)

### Utilizing the Split Window Feature

For convenience, you can open the lab guide in a separate window by selecting the **Split Window** button from the top right corner.

![Image](./media/gs4.png)

### Lab Guide Zoom In/Zoom Out

To adjust the zoom level for the environment page, click the **A↕ : 100%** icon located next to the timer in the lab environment.

![Image](media/gs2.png)

### Resize the Virtual Machine View

Use the **slider (three vertical dots)** located between the **Virtual Machine** and the **Lab Guide** panes to adjust the display size, allowing you to customize the layout based on your preference.

![](./media/ss12.png)

## Let's Get Started with the Microsoft Intune Admin Center

You do all the portal work in the **Microsoft Intune admin center**.

1. On **LabVM**, open **Microsoft Edge** and go to **https://intune.microsoft.com**.

2. For **Username**, enter the **Username** from the **Environment** tab, and select **Next**.

3. Enter the **Temporary Access Pass** from the **Environment** tab, and select **Sign in**. If asked to stay signed in, select **Yes**.

4. Wait until the **Home** page of the Microsoft Intune admin center appears. It can take a minute to load.

> **Note:** The lab user does not need an Intune licence to use the admin center. Both the lab user and Demo User 01 sign in with a **Temporary Access Pass**. On the **Environment** tab, the value labelled **User 01 Password** is Demo User 01's Temporary Access Pass.

## Support Contact

The CloudLabs support team is available 24/7, 365 days a year, via email and live chat to ensure seamless assistance at any time. We offer dedicated support channels tailored specifically for both learners and instructors, ensuring that all your needs are promptly and efficiently addressed.

Learner Support Contacts:

- Email Support: cloudlabs-support@spektrasystems.com
- Live Chat Support: https://cloudlabs.ai/labs-support

## References

- [Microsoft Intune licensing plans and options](https://learn.microsoft.com/en-us/intune/fundamentals/licensing)
- [Learn about the Microsoft Tunnel VPN solution for Microsoft Intune](https://learn.microsoft.com/en-us/intune/intune-service/protect/microsoft-tunnel-overview)
- [Prerequisites for the Microsoft Tunnel VPN for Microsoft Intune](https://learn.microsoft.com/en-us/intune/device-security/microsoft-tunnel/prerequisites)
- [Learn about using Microsoft Tunnel with Mobile Application Management](https://learn.microsoft.com/en-us/intune/device-security/microsoft-tunnel/mam)

Click **Next >>** from the bottom right corner to embark on your Lab journey!

![Image](./media/gs12.png)

### Happy Learning!
