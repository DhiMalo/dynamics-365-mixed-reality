---
author: amaraanigbo
description: Set up Microsoft Teams so a Dynamics 365 Remote Assist worker can work collaboratively 
ms.author: soanigbo
ms.date: 04/07/2020
ms.topic: article
title: Set up Microsoft Teams for Dynamics 365 Remote Assist 
ms.reviewer: v-bholmes
---

# Set up Microsoft Teams with Dynamics 365 Remote Assist  

A technician or inspector can use Remote Assist to work collaboratively with a remote colleague (typically an expert in a particular field) who uses Microsoft Teams. 
The remote collaborator may only want to [join a Remote Assist call on an ad hoc, one-time basis](common-deployment-scenarios.md#scenario-3-vendors-and-customers-join-one-time-call). Or, they may want to collaborate with a Remote Assist user long-term.  
 
This document explains the deployment required for different scenarios.

## Enable someone to join a Remote Assist call on a one-time basis using the Teams desktop app 

**Recommended**: [One-time call](one-time-call.md) makes it easy for Remote Assist users to invite collaborators to join a call using Remote Assist mobile or Teams desktop! To enable someone to join the call using Teams desktop, the licensed Remote Assist user must use the Remote Assist mobile web app to set up a one-time call and share the one-time call link with the Teams desktop user. The Remote Assist user can then join the call using Remote Assist mobile or Remote Assist HoloLens.

**Alternatively,** the licensed Remote Assist user can [set up a Teams meeting](./join-meeting-hololens.md) and invite the collaborator. Then, the licensed Remote Assist HoloLens user will [join the meeting using the Remote Assist HoloLens app](join-meeting-hololens.md). The Teams desktop user will see the meeting invitation in their Outlook calendar or Teams calendar. They right-click the meeting invitation and select **Join Teams meeting**. (The web browser may launch and display options for joining the meeting. To join via Teams application, select **Launch it now**.)

> [!Note] 
> Only a Remote Assist user and Teams desktop users can join a meeting. Remote Assist mobile users and Teams mobile users cannot join a meeting.

## Enable someone to make calls to and receive calls from a Remote Assist user long-term

| Scenario                                                                                                                                                                                                                                                                                                                    | How to enable someone to use Teams dessktop app or Teams mobile app                                                                                                                                                                         |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| People who want to use Dynamics 365 Remote Assist and people who want to use Teams are both currently in your tenant                                                                                                                                                                                                                | [Assign Teams licenses to people in your tenant](/MicrosoftTeams/user-access).                                                             |
| Advanced deployment: [Multi-tenant company deployment using federation](./multi-tenant-deployment.md) | The administrator of the tenant with users who want to use Teams must [assign Teams licenses to people in their tenant](/MicrosoftTeams/user-access).                      |
| Advanced deployment: [Multi-tenant company deployment using guesting](./multi-tenant-deployment.md)      | The administrator of the tenant with Dynamics 365 Remote Assist users must [use Teams guesting](/microsoftteams/guest-access-checklist) to enable people outside their tenant to use Teams.  |
| Advanced deployment: [Vendors and contractors are outside your tenant and want to use Dynamics 365 Remote Assist](vendor-use-ra.md)                                                                                                                                                                                                                                        | [Assign Teams licenses to people in your tenant](/MicrosoftTeams/user-access).                                                             |

Need more help? Check out [Dynamics 365 Remote Assist FAQs](faq-deploy.md) for answers to common questions, or check out the [Microsoft Teams admin documentation](/microsoftteams).


[!INCLUDE[footer-include](../includes/footer-banner.md)]
