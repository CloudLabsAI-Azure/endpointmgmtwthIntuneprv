# Day 4 – Advanced Mobility Solutions in Microsoft Intune Suite

### Overall Estimated Duration: 4 Hours

## Overview  

In this hands-on lab, you will secure mobile access and data for managed and unmanaged devices. You will configure and validate device compliance for mobile platforms and create app protection policies that keep corporate data safe in apps on iOS and Android. You will then configure VPN policies for Android and iOS devices, using Microsoft Tunnel to give devices secure access to on-premises resources. Along the way, you will learn about Microsoft Tunnel architecture, MDM and MAM Tunnel scenarios, and Microsoft Cloud PKI for certificate-based access.

## Objectives

In this lab, you will:
 
- Configure and validate device compliance for mobile devices.
- Configure app protection policies for iOS and Android devices.
- Configure VPN policies for Android devices.
- Configure VPN policies for iOS devices.

## Pre-requisites

Participants should have:

- Completion of Days 1–3, with familiarity creating and assigning Intune policies.
- Basic understanding of iOS/iPadOS and Android Enterprise management.
- Familiarity with VPN concepts and certificate-based authentication.
- Awareness of Microsoft Entra Conditional Access and how compliance affects access.

## Architecture

This architecture demonstrates an end-to-end workflow for secure mobility. Mobile devices are evaluated against compliance policies, and app protection policies secure corporate data inside managed apps. VPN profiles deliver Microsoft Tunnel connectivity to Android and iOS devices, giving enrolled (MDM Tunnel) and unenrolled (MAM Tunnel) devices secure access to on-premises resources, with Microsoft Cloud PKI supporting certificate-based authentication.

## Explanation of Components

The architecture for this lab involves the following key components:

- **Mobile Devices:** Represent the iOS and Android devices that receive compliance, app protection, and VPN policies.

- **Microsoft Intune:** Deploys compliance policies, app protection policies, and VPN profiles to mobile devices.

- **Compliance Policies:** Define requirements such as minimum OS version, passcode, and jailbreak/root detection for mobile devices.

- **App Protection Policies (MAM):** Protect corporate data within managed apps, for example by restricting copy/paste and requiring a PIN.

- **Microsoft Tunnel:** A VPN gateway for Intune that gives iOS and Android devices secure access to on-premises apps and resources.

- **MDM Tunnel:** Tunnel connectivity for devices fully enrolled in Intune, delivered through VPN profiles.

- **MAM Tunnel:** Tunnel connectivity for unenrolled devices, scoped to protected apps such as Microsoft Edge.

- **VPN Profiles:** Intune configuration profiles that deploy VPN connection settings to Android and iOS devices.

- **Microsoft Cloud PKI:** A cloud-based certificate authority in the Intune Suite that issues and manages device certificates.

## Accessing Your Lab Environment
Once you're ready to dive in, your virtual machine and **Guide** will be right at your fingertips within your web browser.

![Image](media/n1.png)

## Virtual Machine & Lab Guide
Your virtual machine is your workhorse throughout the workshop. The guide is your roadmap to success.

## Lab Guide Zoom In/Zoom Out

To adjust the zoom level for the environment page, click the **A↕ : 100%** icon located next to the timer in the lab environment.

![Image](media/gs2.png)

## Exploring Your Lab Resources
To get a better understanding of your lab resources and credentials, navigate to the **Environment** tab.

![Image](media/gs3.png)

## Managing Your Virtual Machine
Feel free to **start, restart, or stop (2)** your virtual machine as needed from the **Resources (1)** tab. Your experience is in your hands!

![Image](./media/gs5.png)

## Utilizing the Split Window Feature
For convenience, you can open the lab guide in a separate window by selecting the **Split Window** button from the top right corner.

![Image](./media/gs4.png)

## Resize the Virtual Machine View

Use the **slider (three vertical dots)** located between the **Virtual Machine** and the **Lab Guide** panes to adjust the display size, allowing you to customize the layout based on your preference.

![](./media/ss12.png)

## Support Contact

The CloudLabs support team is available 24/7, 365 days a year, via email and live chat to ensure seamless assistance at any time. We offer dedicated support channels tailored specifically for both learners and instructors, ensuring that all your needs are promptly and efficiently addressed.

Learner Support Contacts:

- Email Support: cloudlabs-support@spektrasystems.com
- Live Chat Support: https://cloudlabs.ai/labs-support

Click **Next >>** from the bottom right corner to embark on your Lab journey!

![Image](./media/gs12.png)

### Happy Learning!!
