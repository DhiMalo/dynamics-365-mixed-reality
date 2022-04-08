---
title: Making calls between Dynamics 365 Remote Assist mobile and Teams
author: amaraanigbo
description: Making calls between Dynamics 365 Remote Assist mobile and Teams desktop or mobile 
ms.author: soanigbo
ms.date: 04/13/2022
ms.topic: article
ms.reviewer: v-bholmes
---

# Make calls between Dynamics 365 Remote Assist mobile and Microsoft Teams

Technicians using Dynamics 365 Remote Assist mobile can diagnose and resolve issues with remote specialists or collaborators using Microsoft Teams desktop or the Teams mobile app. Both call participants can place mixed-reality annotations in each other's space to collaborate effectively. 

> [!NOTE]
> This article shows how to make a one-to-one call between a Dynamics 365 Remote Assist mobile user and a Teams desktop or mobile user. [Learn about group calls with at least two Teams desktop users](group-calling.md).

## Prerequisites

- Technicians must have a [Dynamics 365 Remote Assist free trial](../try-remote-assist.md) or a [Dynamics 365 Remote Assist subscription](../buy-remote-assist.md).

- Remote collaborators must have a Dynamics 365 Remote Assist free trial or subscription and/or [Microsoft Teams free trial or subscription](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software). [Learn how to set up Dynamics 365 Remote Assist with Teams desktop](../teams-pc-all.md) or [Teams mobile](../teams-mobile-all.md).

## How it works

1. Launch and sign into Dynamics 365 Remote Assist on an iOS or Android phone or tablet.

    > [!IMPORTANT]
    > The mixed reality toolbar will not appear if the Dynamics 365 Remote Assist user joins the call from two different devices.

2. Search for the remote collaborator's name.

    ![Screenshot of Dynamics 365 Remote Assist mobile, showing the contacts screen and highlighting the search icon.](./media/calls_2.png "Search")

3. Select the remote collaborator's name, and then select **Launch Call**.

    ![Screenshot of Dynamics 365 Remote Assist mobile showing the Launch Call button.](./media/calls_3.png)
    
     > [!NOTE]
    > If Dynamics 365 Remote Assist Mobile and Teams mobile are both installed on the same device, [learn where incoming call notifications are received](remote-assist-mobile-to-teams-calls.md#What-happens-when-Dynamics-365-Remote-Assist-mobile-and-Teams-mobile-are-installed-on-the-same-device).

4. If the remote collaborator answers the call on **Teams desktop or mobile**, the technician's live video feed is shared with the remote collaborator's device screen.

    ![Screenshot of a Dynamics 365 Remote Assist mobile to Microsoft Teams call.](./media/ram-teams-video.png)

5. Both call participants can place annotations in the shared environment either in their own environment or by selecting **Start editing**. 

    > [!NOTE] 
    > After the remote collaborator selects **Start editing**, the remote collaborator can add mixed-reality annotations on a frozen frame of the shared environment. When the remote collaborator selects **Stop editing**, the annotation appears in the technician's shared environment. 

    ![Side-by-side screenshots of Dynamics 365 Remote Assist mobile and Microsoft Teams, showing annotations appearing in both screens.](./media/ram-teams-remote-collab.png "Place Annotations")

6. The technician can use the call controls toolbar to change between a video call and an audio-only call, mute or unmute the microphone, turn the speaker on or off, add participants, share spaces (environments), start/stop a recording, or end the call. The following table describes each button in the call controls toolbar.

    |Button|Description|
    |--------|--------------------------|
    |![Video button.](./media/ra-video-button.PNG)|Change between video call and audio-only call|
    |![Microphone button.](./media/ra-microphone-button.PNG)|Mute or unmute the microphone|
    |![Speakers button.](./media/ra-speaker-button.PNG)|Turn the speaker on or off|
    |![More menu button.](./media/ra-more-menu.PNG)|Display the **More** menu to add participants, share spaces (environment), or start/stop a recording|
    |![End call button.](./media/ra-end-call.PNG)|End the call|
    
7. During the call, call participants can capture and annotate snapshots, send messages, share files, and more.

## What happens when Dynamics 365 Remote Assist mobile and Teams mobile are installed on the same device

### iOS

If the remote collaborator receives the call on a mobile device with both Dynamics 365 Remote Assist mobile and Teams mobile installed, the remote collaborator will get incoming call notifications only on Teams mobile. 

### Android

If the remote collaborator receives the call on a mobile device with both Dynamics 365 Remote Assist mobile and Teams mobile installed, the remote collaborator will get incoming call notifications: 

- Only on Teams mobile if Teams mobile incoming call notifications are enabled in the **Settings** page.
 
- Only on Remote Assist mobile, if Teams mobile incoming call notifications are disabled in the **Settings** page. 

    ![Screenshot of Teams Settings page.](./media/teams-settings.jpg)

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
