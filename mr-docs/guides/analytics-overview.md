---
author: BryceHo
description: Get an overview of how to analyze guides using Microsoft Dynamics 365 Guides
ms.author: cynielse
ms.date: 06/17/2022
ms.topic: overview
title: Overview of analyzing and integrating Dynamics 365 Guides usage data
ms.reviewer: v-bholmes
---

# Overview of analyzing and integrating Dynamics 365 Guides usage data

> [!IMPORTANT]
> We recently identified an issue with an update where Dynamics 365 Guides operator sessions data (for both authors and operators) has not been saved to Microsoft Dataverse. Users may notice that session data was not being recorded as early as October 15, depending on region. [Learn more](known-issues-hololens-app.md)

When operators use the Microsoft Dynamics 365 Guides HoloLens app, data about app and guide usage is automatically stored in your private and secure Dynamics 365 environment where it can be analyzed in either of the following ways:

- Using the [Guides Analytics Power BI templates](analytics-guide.md)

- Integrated into your own custom workflows. For example, you could create a custom workflow in Microsoft Power Automate or by using third-party visualization tools or systems.

Data capture has the following limitations:

- Data will not be collected if an operator is working in offline mode.

- Data might be lost if an internet connection is intermittent.

- For best data capture results, after an intermittent internet connection is restored, wait for data to be uploaded to Microsoft Dataverse before closing the app.

## How it works

### 1. Sign in to Dynamics 365 Guides

Data for all users is automatically stored in the MR App Session table (described in more detail below).

### 2. Author a guide in the PC or HoloLens app

Data for all authors is automatically stored in the Guide Author Session table (described in more detail below).

### 3. Operate a guide

**Next** and **Back** button interactions are recorded to determine the time spent on each step. Operator data is automatically stored in the Guide Session table and the Guide Session Step Visit table. Both tables are described in more detail below. 

### 4. Trigger alerts or visualize data

Use the Power Platform to analyze and act on your data.

![Power Platform example.](media/analytics-alerts-visualize-data-1.PNG "Power Platform example")

> [!NOTE]
> Guides operations data is intended to help supervisors and managers derive insights regarding operational efficiencies and usage of Dynamics 365 Guides. This feature is not intended for use in making (and should not be used to make) decisions that affect the employment of an employee or group of employees, including compensation, rewards, seniority, or other rights or entitlements. Customers are solely responsible for using Dynamics 365, this feature, and any associated feature or service in compliance with all applicable laws, including laws relating to accessing individual employee analytics and monitoring. Customers are encouraged to have a mechanism in place to inform their users that analytics relating to their guides usage is collected. 

### MR App Session table

Dynamics 365 Guides includes an MR App Session table that you can use to determine the overall usage of the product in your organization. This is useful so you can determine where to assign Dynamics 365 Guides licenses. 

The MR App Session table stores a record whenever a user signs into an instance. The table stores information about when the user signed in, the session type (log-in or suspend, which tracks when a user resumes using the device), device class (PC or HoloLens), and the User ID. For more information, [see the Microsoft Dataverse table (entity) reference](developer-entity-reference.md). 

> [!NOTE]
> Data in the MR App Session table is accessible by admin users or by scripted actions that act as admin users. 

### Guide Author Session table

Each row in the Guide Author Session table corresponds to a HoloLens or PC app interaction with a guide in Authoring mode. Information about the session, such as User ID, guide name, start time, end time, and device class is recorded. For more information, see the [Microsoft Dataverse table (entity) reference](developer-entity-reference.md).

### Guide Session table 

Each row in the Guide Session table corresponds to an operation of a guide in HoloLens Operate mode, whether completed from beginning to end of the guide or involving just a few steps. Information about the guide session, such as start and end time, total operating time, and different options that define completion (for example, if the completion step was visited, or the percentage of steps that the operator visited) are also recorded. For more information, [see the Microsoft Dataverse table (entity) reference](developer-entity-reference.md).

> [!IMPORTANT]
> When a user **enters a Completion step,** that information is logged in the Guide Session table. This is different from the RunEnd event in the [Guide Event table](developer-entity-reference.md#dynamics-365-guides-tables), which is generated when an **operator closes a guide.** 

### Guide Session Step Visit table 

Each row in the Guide Session Step Visit table corresponds to an operator’s visit to a step in HoloLens Operate mode. Information is recorded for each step visit such as start and end time and step operating time. If an operator visited a step multiple times, perhaps by navigating backward and forward in the guide, each visit would result in a separate row in this table. For more information, [see the Microsoft Dataverse table (entity) reference](developer-entity-reference.md). 

## What can you do with the data? 

Storing data about the operations of your guides in easy-to-access Microsoft Dataverse tables gives you the flexibility to analyze and integrate this data into your workflows in ways that make sense for your business. You can get started by:

- Using the [Guides Analytics Power BI templates](analytics-guide.md)

- Building your own custom integrations with this data. 

Here are some examples of what you can do: 

- **Monitor completion status of a guide and trigger workflows.** The Guide Session table includes measurements of guide completion status that you can use with Microsoft Power Automate to, for example, send notifications when an operator has completed a guide. Given that there are many ways to define whether a guide session is complete, the Guide Session table provides two different measurements that you can use individually or together as appropriate for your use case:

    - The first guide completion measurement is stored in the **Percent Of Steps Visited** column and is calculated by taking the number of unique visited steps in a session and dividing by the total number of steps in the guide. This measurement is particularly useful for linear guides in which you expect operators to visit every step. 
    
    - The second completion measurement is stored in the **Visited Completion Step** column and defines whether a completion step was visited during the guide session. If the guide has multiple completion steps, this will be a **Yes** value if any one of the completion steps was visited during the session.  

- **Analyze session and step times to optimize process.** By analyzing operating times across all guide sessions and steps, you can identify processes that are taking more than a given target time or have high time variability or outliers that may indicate areas for process improvement. The [Guides Analytics Power BI templates](analytics-guide.md) can help you get started with these analyses. 

   > [!TIP]
   > When the HoloLens app is suspended manually or due to inactivity, the current step visit is ended and a new step visit is created once the app resumes. This means that app suspension time is not included in the values of the **Step Duration Seconds** column. These step visit durations for a session are summed together and recorded in the Guide Session table’s **Active Session Duration Seconds** column. As a result, the **Active Session Duration Seconds** values do not include any app suspension time and offer a higher quality measurement of operation time than the simple difference between session start and end time stamps.   

## Getting started 

**Guides model-driven app.** You can use the **Active Guide Sessions** view in the Guides model-driven app to inspect guide sessions. To access the model-driven app, sign in to Microsoft Power Apps and go to the **Apps** tab. 

![Guide Sessions view.](media/analytics-data-stored-automatically-2.jpg "Guide Sessions view")

Double-clicking on an individual session row in this view provides more details about the session as well as access to a **Session History** tab that contains information about individual step visits.  

![Session History tab.](media/analytics-session-history-tab.PNG "Session History tab")

**Guides Analytics Power BI templates.** You can start analyzing your guide session and step visit data with the [Guides Analytics Power BI templates](analytics-guide.md). For information on setting up Guide Analytics, see [Set up Guides Analytics reports](analytics-ga-setup.md).  

## See also

- [Overview of Guides Analytics Power BI templates](analytics-guide.md)
- [Set up Guides Analytics reports](analytics-ga-setup.md)
- [Take a tour of Guides Analytics reports](analytics-ga-reports.md)
- [Share Guides Analytics reports](analytics-ga-share-reports.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
