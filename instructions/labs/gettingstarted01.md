# Day 1 – Unified Endpoint Management with Microsoft Intune

### Overall Estimated Duration: 4 Hours

## Overview  

In this hands-on lab, you will set up Microsoft Intune as the foundation for cloud-native, Zero Trust endpoint management. You will configure the Intune tenant and administrator access, manage how devices register with Microsoft Entra ID, and configure enrollment settings and restrictions for corporate and personal devices. Finally, you will enroll a Windows device into Microsoft Intune and verify that it is managed and reporting correctly in the Microsoft Intune admin center.

## Objectives

In this lab, you will:
 
- Set up Microsoft Intune, including the MDM authority, licensing, and administrator roles.
- Manage Microsoft Entra device registration and control which users can register and join devices.
- Configure and manage device enrollment, including enrollment restrictions for corporate and personal devices.
- Enroll a Windows device into Microsoft Intune and verify its status in the Intune admin center.

## Pre-requisites

Participants should have:

- Basic understanding of Microsoft 365 services and administration.
- Familiarity with Microsoft Entra ID users, groups, and device identities.
- General knowledge of Windows, macOS, iOS, Android, and Linux device management.
- Awareness of Zero Trust principles for endpoint security.

## Architecture

This architecture demonstrates an end-to-end workflow for bringing devices under cloud management. It starts with setting up the Intune tenant and administrator access, then configures Microsoft Entra device registration and enrollment settings. A Windows device is then enrolled into Intune, where it becomes visible and manageable from the Microsoft Intune admin center, ready for policies on the following days.

## Explanation of Components

The architecture for this lab involves the following key components:

- **Endpoint:** Represents the Windows device used in the lab that is registered with Microsoft Entra ID and enrolled into Microsoft Intune.

- **Microsoft Intune:** A cloud-based endpoint management solution that manages devices and apps across Windows, macOS, iOS, Android, and Linux.

- **Microsoft Intune admin center:** The single web console used to configure enrollment, policies, apps, and reports for all managed devices.

- **Microsoft Entra ID:** Provides user, group, and device identities (registered, joined, and hybrid joined) that Intune uses for targeting and access.

- **Device Registration:** Creates a device identity in Microsoft Entra ID so the device can be recognized and governed by organizational policies.

- **Enrollment Restrictions:** Define which platforms, OS versions, and ownership types (corporate or personal) are allowed to enroll.

- **Device Enrollment:** Brings a device under Intune MDM management so that configuration, compliance, and app policies can be applied.

- **Zero Trust:** A security model that verifies every device and user explicitly before granting access to corporate resources.

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
