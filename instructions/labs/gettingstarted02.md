# Day 2 – Cloud-based Unified Endpoint Security and Management with Microsoft Intune

### Overall Estimated Duration: 6 Hours

## Overview  

In this hands-on lab, you will secure the devices and data you enrolled on Day 1. You will integrate Microsoft Defender for Endpoint with Intune, create and deploy compliance policies, and configure endpoint security policies such as antivirus, firewall, and disk encryption. You will then configure update management for Windows devices and enable Endpoint Data Loss Prevention with Microsoft Purview. Finally, you will protect corporate data in apps with Mobile Application Management (MAM) and configure Endpoint Privilege Management (EPM) so standard users can run approved tasks with elevated rights.

## Objectives

In this lab, you will:
 
- Integrate Microsoft Defender for Endpoint with Microsoft Intune and onboard devices.
- Create and deploy compliance policies and review device compliance status.
- Configure endpoint security using Microsoft Intune, including antivirus, firewall, and disk encryption.
- Configure update management for Windows devices using update rings and update policies.
- Enable Endpoint Data Loss Prevention with Microsoft Purview.
- Enable Mobile Application Management (MAM) using app protection policies.
- Configure Endpoint Privilege Management (EPM) for controlled elevation.

## Pre-requisites

Participants should have:

- Completion of Day 1, with Intune set up and at least one device enrolled.
- Basic understanding of Microsoft Defender for Endpoint and the Microsoft Defender portal.
- Awareness of Microsoft Purview Data Loss Prevention and sensitive information types.
- Familiarity with assigning Intune policies to users and device groups.

## Architecture

This architecture demonstrates an end-to-end workflow for securing managed endpoints. Devices enrolled in Intune are connected to Microsoft Defender for Endpoint so that device risk feeds into compliance. Intune then deploys compliance, endpoint security, and update policies, while Microsoft Purview applies Endpoint DLP to protect sensitive data. App protection policies secure corporate data inside apps, and Endpoint Privilege Management controls elevation on Windows devices.

## Explanation of Components

The architecture for this lab involves the following key components:

- **Endpoint:** Represents the Windows device enrolled in Intune that receives security, compliance, and update policies.

- **Microsoft Intune:** Deploys and manages compliance, endpoint security, update, app protection, and EPM policies.

- **Microsoft Defender for Endpoint:** Protects endpoints with EDR, detects threats, and shares device risk levels with Intune.

- **Compliance Policies:** Define the health and configuration requirements a device must meet to be considered compliant.

- **Endpoint Security Policies:** Configure antivirus, firewall, disk encryption (BitLocker), and attack surface reduction settings.

- **Update Management:** Uses Windows Update for Business rings and policies to control how and when devices are updated.

- **Microsoft Purview Endpoint DLP:** Monitors and restricts actions such as copying, printing, or uploading sensitive files on devices.

- **Mobile Application Management (MAM):** Protects corporate data at the app level using app protection policies, even on unenrolled devices.

- **Endpoint Analytics & Graph API:** Provide device performance insights and programmatic access to Intune reports and properties.

- **Endpoint Privilege Management (EPM):** An Intune Suite capability that lets standard users perform approved tasks with elevated rights.

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
