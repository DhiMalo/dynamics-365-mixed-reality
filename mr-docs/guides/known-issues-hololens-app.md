---
author: Mamaylya
description: Learn about known issues with the Microsoft Dynamics 365 Guides HoloLens app.
ms.author: mamaylya
ms.date: 03/24/2022
ms.topic: article
title: Known issues with the Dynamics 365 Guides HoloLens app
ms.reviewer: v-bholmes
---

# Known issues with the Dynamics 365 Guides HoloLens app

## Why did my HoloLens display go blank for a few seconds when I placed a 3D model in the HoloLens app?

If you place a large 3D model in the HoloLens app, the display may go blank for several seconds while the model is being processed by Dynamics 365 Guides.

## Why isn't my operator sessions data being saved to Microsoft Dataverse? 

We recently identified an issue with an update where Dynamics 365 Guides operator sessions data (for both authors and operators) has not been saved to Microsoft Dataverse. Users may notice that session data was not being recorded as early as October 15, depending on region.

This issue doesn’t affect the ability to operate a guide, but it does affect all Dynamics 365 Guides customers who [analyze their guide session data](analytics-overview.md) or use the StepEnd event for integrations. 

A fix will be deployed to all customers during the week of December 6, 2021, during regional maintenance hours. There is no action required to receive the fix. Additionally, Microsoft is updating the Dynamics 365 Guides 7.0 HoloLens app with a hotfix on December 2, 2021, to enable customers to begin saving sessions data before the general fix is ready. To apply this fix, see [Update your solution](upgrade.md).

If you have any questions, contact Microsoft Support.

## Telemetry data not stored for operators with **Restricted Operator** role in certain cases

Operators with the **Restricted Operator** role that don't have the appendTo privilege can access and operate guides but their session data (telemetry) is not stored for time-tracking purposes.

## The account picker becomes unresponsive if you stay on it for more than 25 seconds during HoloLens sign-in 

On the page where you can select among the different accounts that are saved on [!include[pn-hololens](../includes/pn-hololens.md)], you must select an option within 25 seconds. After 25 seconds, the page becomes unresponsive, and you must restart the app. This issue has been fixed on RS5 but still exists on RS4 if you have that version installed.

## When you place large assets on HoloLens, you might experience minor loading delays

The [!include[pn-hololens](../includes/pn-hololens.md)] app currently loads the guide right after you open it. As you use the guide, the app loads it in the background. If your guide contains large 3D models and media, you might experience loading delays of a few seconds.

## An incorrect profile picture is shown in the app 

If an incorrect profile picture is shown, make sure that you're signed in. Select the profile picture, sign out, and then sign back in by using your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] credentials. Your profile picture should appear correctly.

By using the correct credentials to sign in, you ensure that your work progress is correctly tracked in [!include[pn-dyn-365](../includes/pn-dyn-365.md)].

## The video preview on a step is blurry

The PC app video may appear to be blurry when an author previews a video in the HoloLens app. The PC app converts and resizes videos when they're uploaded to ensure optimal performance on HoloLens. This transcoding process depends on the codecs installed on the PC and errors can occur if codecs are removed from the PC. The  HoloLens app currently uses an optimized video specification of 853×480 H.264. If your video was recorded at a very high resolution, or if it's very large, the transcoding process on the PC might degrade the quality, making it appear blurry. To fix this issue, record and upload a new video, keeping its length and resolution in mind. Note that only the 853x480 video file will be stored on Microsoft Dataverse.

## When the see-through style is applied to a 3D model, it might show gray areas instead of correctly rendering textures 

There are rendering issues for the "see through" style on some 3D models. Some surfaces on these models will look gray. If you experience this issue, use another style. If you **must** use this style and need help with it, contact customer service.

## See also

- [Known issues with Dynamics 365 Guides generally](known-issues.md)
- [Known issues with the PC app](known-issues-pc-app.md)
- [Dynamics 365 Guides FAQ](faq.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
