---
author: BryceHo
description: Get an overview of how to analyze guides using Microsoft Dynamics 365 Guides
ms.author: cynielse
ms.date: 11/08/2021
ms.topic: overview
title: Overview of analyzing guides created with Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# Overview of analyzing and integrating Dynamics 365 Guides operations data

> [!IMPORTANT]
> We recently identified an issue with an update where Dynamics 365 Guides operator sessions data (for both authors and operators) has not been saved to Microsoft Dataverse. Users may notice that session data was not being recorded as early as October 15, depending on region. [Learn more](known-issues-hololens-app.md)

When operators use the Microsoft Dynamics 365 Guides HoloLens app in Operate mode, data about guide usage is automatically stored in your private and secure Dynamics 365 environment where it can be analyzed in either of the following ways:

- Using the [Guides Analytics Power BI templates](analytics-guide.md)

- Integrated into your own custom workflows. For example, you could create a custom workflow in Microsoft Power Automate or by using third-party visualization tools or systems.

The operations data, which includes information about time spent on each step and whether an operator completed a guide, is stored in Microsoft Dataverse tables just like your Dynamics 365 Guides content. These tables make it easy to analyze guide usage across your organization, gain insights into process efficiency, or trigger workflows outside of Dynamics 365 Guides.

### How it works

#### 1. Operate a guide

**Next** and **Back** button interactions are recorded to determine the time spent on each step.

![HoloLens operator at work.](media/analytics-hololens-operator-1.PNG "HoloLens operator at work")

#### 2. Data is automatically stored

Step time data is stored in your **private and secure** Dynamics 365 environment.

![Screen shot of saved step time data .](media/analytics-data-stored-automatically-1.PNG "Screen shot of saved step time data")

#### 3. Trigger alerts or visualize data

Use the Power Platform to analyze and act on your data.

![Power Platform example.](media/analytics-alerts-visualize-data-1.PNG "Power Platform example")

> [!NOTE]
> Guides operations data is intended to help supervisors and managers derive insights regarding operational efficiencies and usage of Dynamics 365 Guides. This feature is not intended for use in making (and should not be used to make) decisions that affect the employment of an employee or group of employees, including compensation, rewards, seniority, or other rights or entitlements. Customers are solely responsible for using Dynamics 365, this feature, and any associated feature or service in compliance with all applicable laws, including laws relating to accessing individual employee analytics and monitoring. Customers are encouraged to have a mechanism in place to inform their users that analytics relating to their guides usage is collected. 

## See also

- [What data is collected and how can you use it?](analytics-data-collected.md)
- [Overview of Guides Analytics Power BI templates](analytics-guide.md)
- [Set up Guides Analytics reports](analytics-ga-setup.md)
- [Take a tour of Guides Analytics reports](analytics-ga-reports.md)
- [Share Guides Analytics reports](analytics-ga-share-reports.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
