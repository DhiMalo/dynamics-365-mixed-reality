---
author: amaraanigbo
description: Answers to common questions about deploying Microsoft Dynamics 365 Remote Assist.
ms.author: soanigbo
ms.date: 04/14/2022
ms.topic: article
title: Frequently asked questions for deploying Dynamics 365 Remote Assist 
ms.reviewer: v-bholmes
---

# Frequently asked questions for deploying Dynamics 365 Remote Assist

Here are some answers to common questions about deploying Dynamics 365 Remote Assist on HoloLens, HoloLens 2, and mobile devices.

## What are the technical requirements for deploying Dynamics 365 Remote Assist?

[Learn about technical requirements](requirements.md)

## How do I enable map visualization on the Dynamics 365 Remote Assist Calls Dashboard?

Map visualization is available in all regions except Europe. To enable map visualization, you must [enable the Power BI Azure Maps visual](/azure/azure-maps/power-bi-visual-manage-access#tenant-admin-options). [Learn more about the Calls Dashboard](calls-dashboard.md).

## Can I use Dynamics 365 Remote Assist to collaborate with a Microsoft Teams user outside my tenant, or vice versa?

Yes. Learn how to [set up multi-tenant company deployments](multi-tenant-deployment.md), [enable vendors and contractors to use Remote Assist](vendor-use-ra.md), or [enable vendors and contractors to use Teams](vendor-use-teams.md).

## How do I set up Dynamics 365 Field Service to work with Dynamics 365 Remote Assist?

To learn how to set up Dynamics 365 Field Service integration with Dynamics 365 Remote Assist so that a firstline worker can call an expert in the context of a Field Service booking, see [Integrate Dynamics 365 Field Service with Dynamics 365 Remote Assist](troubleshoot-field-service.md).

## Will any Teams license work when communicating with a Dynamics 365 Remote Assist user?

Yes. Anyone that can sign in and use the Teams application on a Windows 10 PC or mobile device can communicate with a Dynamics 365 Remote Assist user if their tenants are set up correctly. If the Teams user and Dynamics 365 Remote Assist user are not in the same tenant, learn how to [set up multi-tenant company deployments](multi-tenant-deployment.md), [enable vendors and contractors to use Dynamics 365 Remote Assist](vendor-use-ra.md), or [enable vendors and contractors to use Teams](vendor-use-teams.md). 

## Can I assign a Dynamics 365 Remote Assist license to a user using [Azure AD B2B](/azure/active-directory/b2b/what-is-b2b)?

No.  Dynamics 365 Remote Assist licenses must be assigned to an AAD account created in the tenant where Dynamics 365 Remote Assist will be used.

## How do I file a support ticket?

If you encounter an issue that blocks you from using the application and you don't see an answer on our user forum, please file a support ticket. Support will work directly with you and communicate daily until the issue is resolved. [Learn more about support options](/dynamics365/get-started/support/).

[!INCLUDE[footer-include](../includes/footer-banner.md)]
