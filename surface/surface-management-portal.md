---
title: Surface Management Portal 
description: Discover how the Surface Management Portal, integrated within the Microsoft Intune admin center, offers a centralized platform to efficiently manage, monitor, and maintain Surface devices at scale, ensuring compliance and streamlined support.
ms.service: surface
ms.localizationpriority: medium
author: coveminer
ms.author: chauncel
ms.topic: how-to
ms.date: 08/02/2024
ms.reviewer: rohitmannan
manager: frankbu
appliesto:
- Windows 10
- Windows 11
ms.collection: essentials-manage
---
# Surface Management Portal overview

Built into Microsoft Intune admin center, the Surface Management Portal provides a centralized solution to self-serve, manage, and monitor Surface devices at scale.

## Introduction

As a single environment for the end-to-end visibility of corporate or user-owned Surface devices, the Surface Management Portal lets you quickly see any issues that need prompt attention before they hit your help desk.

Get insights into device compliance, support activity, and warranty coverage. Quickly see the status of each device, which ones are still in warranty or expiring soon, and the status of active support requests with your hardware providers.

When you [enroll Surface devices](/mem/intune/user-help/enroll-windows-10-device) into Microsoft Intune and users sign in for the first time, information from these Surface devices automatically flows into the Surface Management Portal, giving you a single pane of glass for Surface-specific device admin activities.

>[!TIP]
>To learn more about accessing the Surface Management Portal or the Microsoft 365-based [Surface Support Portal](surface-support-portal.md),see [Streamline access to Surface Portals for commercial customers](streamline-access-surface-portals.md). 

## Get started

### If you don't have an Intune subscription:

1. To sign up for Intune, go to the [Intune product page](https://www.microsoft.com/security/business/endpoint-management/microsoft-intune) to learn more about the service.
2. Select **Start a free trial** to initiate the sign-up process, as described in [Try Microsoft Intune for free](/mem/intune/fundamentals/free-trial-sign-up).
3. Follow the prompts to create an account and choose a [subscription plan](https://www.microsoft.com/security/business/microsoft-intune-pricing) that fits your organization's needs.
4. Follow the setup wizard to configure your Intune environment. Add users, set up device policies, and configure security settings as needed.
5. You can manage a wide range of OEM (Original Equipment Manufacturer) devices with Intune but need to [enroll at least one Surface device](/mem/intune/user-help/enroll-windows-10-device) in order to access the Surface Management Portal.
6. Once you subscribe to Intune and [enroll](/mem/intune/user-help/enroll-windows-10-device) at least one Surface device, proceed to the next section.

### If you have an Intune subscription:

1. Sign in to [Microsoft Intune admin center](https://endpoint.microsoft.com), select **All services** > **Surface Management Portal**.

   :::image type="content" source="images/surface-management-portal/surface-management-portal-start.png" lightbox="/surface/images/surface-management-portal/surface-management-portal-start.png" alt-text="Start Surface Management Portal":::

<a name='azure-ad-roles-for-surface-management-portal'></a>

## Microsoft Entra roles for Surface Management Portal


| Role                                      | Permissions                                                                                                                                                                                 |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Microsoft Hardware Warranty Administrator<sup>1</sup> | View all service requests<br>Create/manage device replacement requests<br>Add/edit/delete ship-to addresses<br>Read-only access to the Microsoft 365 tenant outside of the Surface Support Portal |
| Microsoft Hardware Warranty Specialist<sup>1</sup>     | View own service requests<br>Create/manage device replacement requests<br>Read-only access to the Microsoft 365 tenant outside of the Surface Support Portal                                        |
| Global Admin                              | View service requests<br>Create/manage device replacement requests<br>Add/edit/delete ship-to addresses<br>Create/manage users and their roles                                            |
| Service Support Admin                     | View service requests<br>Create/manage device replacement requests                                                                                                                          |
| Billing Admin                             | View service requests<br>Create/manage device replacement requests<br>Add/edit/delete ship-to addresses                                                                                   |

1. *Requires **Read Only Operator** role for access*.

> [!IMPORTANT]
> Microsoft recommends that you use roles with the fewest permissions. This helps improve security for your organization. Global Administrator is a highly privileged role that should be limited to emergency scenarios when you can't use an existing role.

## Monitor Surface devices

Select **Monitor** to display insights for all your Surface devices, including:

- Devices out of compliance, which could mean users can’t access information requiring Microsoft Entra sign-in.
- Devices that aren’t registered.
- Devices with critically low storage available on disk, a leading indicator of potential user experience issues.
- Devices requiring updates.
- Devices without drive encryption enabled.
- Devices that are currently inactive.

Select **View report** to see details on each insights category, giving you diagnostic information that you can customize and export.

:::image type="content" source="images/surface-management-portal/surface-management-portal-view-report.png" lightbox="/surface/images/surface-management-portal/surface-management-portal-view-report.png" alt-text="Get Surface device insights and view report":::

> [!TIP]
> The portal shows device information for your top four registered devices with all others listed under **Other**. Select **View report** to see all your devices. 

## Device warranty and coverage

If you manage hundreds or thousands of devices, having direct access to the warranty status of each device is especially useful, letting you quickly see the following information:

- Devices within the warranty period
- Devices expiring
- Devices out of warranty
- Devices eligible for optional coverage

## Support requests

The Surface Management Portal gives complete visibility into support activity along with the status of each request.

:::image type="content" source="images/surface-management-portal/surface-management-portal-support.png" lightbox="/surface/images/surface-management-portal/surface-management-portal-support.png" alt-text="Get information about support activity along with the status of each request.":::

### Create Support Requests

Newly added to the portal is the ability to create and submit new requests for one device or many.

1. Select **Create support request**.
2. Select the Product (Device) from the drop-down list.
3. Based on the Product selected, pick the device model.
4. Select the device or devices based on the serial number (SN).
5. Provide details and supporting information about the issue.
6. Provide your contact information and a contact preference.
7. Review and submit the request.  

   :::image type="content" source="images/surface-management-portal/smp-submit-support-request.png"  alt-text="Submit support request.":::

> [!TIP]
> Track request status using the current insights and detailed views.

## Try for free

Surface Management Portal is available to customers who use Microsoft Intune admin center and enroll at least one Surface device through Intune. If you’re new to Intune, set up your Intune tenant today by visiting [Try Microsoft Intune for free](/mem/intune/fundamentals/free-trial-sign-up).

## Learn more

- [What is Microsoft Surface Management Portal?](/mem/intune/fundamentals/surface-management-portal?)
- [Microsoft Mechanics](https://youtu.be/_MmutkqNudk)
- [Surface IT Pro Blog post: Surface Management Portal](https://techcommunity.microsoft.com/t5/surface-it-pro-blog/surface-management-portal/ba-p/1419017)
