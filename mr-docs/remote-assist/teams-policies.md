---
description: Learn which Microsoft Teams policies are supported by Dynamics 365 Remote Assist and the effect of disabling those policies.
title: Microsoft Teams policies supported by Dynamics 365 Remote Assist
author: amaraanigbo
ms.author: soanigbo
ms.date: 04/13/2022
ms.topic: article
ms.reviewer: v-bholmes
---

# Microsoft Teams policies supported by Dynamics 365 Remote Assist

Dynamics 365 Remote Assist supports the following Microsoft Teams policies: 

- Video
- Call recording
- Chat messaging
- File sharing
 
Users in your organization will automatically get the global policy unless you create and assign a custom policy. You can edit the settings in the global policy or 
create and assign one or more custom policies to turn the features that you want on or off.  

> [!NOTE]
> You can't set policies for specific applications (for example, Dynamics 365 Remote Assist vs. Teams).  

## Video policies

Video policies are used to control video stream capabilities. Video policies do not disable:

- The camera because the user can use [mixed reality capture (MRC)](/hololens/holographic-photos-and-videos)
- The low-bandwidth feature
- The asset capture feature 

> [!IMPORTANT]
> If video is disabled, users will not be able to see mixed-reality annotations from remote participants.  

### User experience in the HoloLens app

When video is disabled, the **Video** button is unavailable.

![HoloLens app screenshot with Video button disabled.](media/teams-policies-hololens-video-button.PNG "HoloLens screenshot with Video button disabled")

If the user selects the **Video** button, they see the following message that explains why outgoing video is unavailable.

![HoloLens app screenshot showing video message.](media/teams-policies-hololens-video-message.PNG "HoloLens screenshot showing video message")

### User experience in the mobile app

When video is disabled, the **Video** button is unavailable and the Mixed Reality toolbar is also unavailable.

![Mobile app screenshot with Video button disabled.](media/teams-policies-mobile-video-button.PNG "Mobile app screenshot with Video button disabled")

If the user selects the **Video** button, they see the following message that explains why video is unavailable.

![Mobile app screenshot showing video message.](media/teams-policies-mobile-video-message.PNG "Mobile app screenshot showing video message")

## Call-recording policies 

Call-recording policies are used to control call-recording capabilities. This allows admins to disable call recording for privacy purposes. If call recording is disabled through policy, the Dynamics 365 Remote Assist user will not be able to start a recording.  

> [!NOTE]
> This policy does not affect other participants on a call. Other participants will still be able to start/stop recordings.  

### User experience in the HoloLens app

When call recording is disabled, the **Recording** button is unavailable.

![HoloLens app screenshot with Recording button disabled.](media/teams-policies-hololens-call-recording-button.PNG "HoloLens screenshot with Recording button disabled")

If the user selects the **Recording** button, they see the following message that explains why recording is not available.  
 
![HoloLens app screenshot showing recording message.](media/teams-policies-hololens-call-recording-message.PNG "HoloLens screenshot showing recording message")

### User experience in the mobile app

When call recording is disabled, the **Start recording** command is unavailable.

![Mobile app screenshot with Start recording button disabled.](media/teams-policies-mobile-call-recording-command.PNG "Mobile app screenshot with Start recording button disabled")

If the user selects the **Start recording** command, they see the following message that explains why recording is not available.

![Mobile app screenshot showing recording message.](media/teams-policies-mobile-call-recording-message.PNG "Mobile app screenshot showing recording message")

## Chat-messaging policies

Chat-messaging policies are used to control which chat and channel messaging features are available to [users (owners and members)](/microsoftteams/assign-roles-permissions) in Microsoft Teams.  

If chat messaging is disabled, Dynamics 365 Remote Assist users can read but not send chat messages. Voice recording and photo capture are also disabled since these features require chat.  

### User experience in the HoloLens app

When chat messaging is disabled, the Chat window and keyboard are disabled and the user sees **Chat unavailable** in the Chat window.  

![HoloLens app screenshot showing Chat unavailable in Chat window.](media/teams-policies-hololens-chat-button.PNG "HoloLens app screenshot showing Chat unavailable in Chat window")
 
If the user tries to enter text in the Chat window, they see the following message that explains why chat is unavailable.

![HoloLens app screenshot showing chat message.](media/teams-policies-hololens-chat-message.PNG "HoloLens app screenshot showing chat message")

### User experience in the mobile app

When chat messaging is disabled, the Chat window and keyboard are disabled and the user sees **Chat disabled by admin** in the Chat window.

![Mobile app screenshot showing Chat unavailable.](media/teams-policies-mobile-chat-unavailable.PNG "Mobile app screenshot showing Chat unavailable")

If the user tries to enter text in the Chat window, they see the following message explaining why chat is unavailable. 

![Mobile app screenshot showing xhat message.](media/teams-policies-mobile-chat-message.PNG "Mobile app screenshot showing chat message")

## File-sharing policies

File-sharing policies are used to control whether Teams users and Dynamics 365 Remote Assist users can share files. 

- If file sharing is disabled for the Teams user, the **Attach** button is removed from the Teams text chat user interface. The Teams user on the other end of a call/chat can continue to send attachments and files without any changes. 

- If file sharing is diabled for Dynamics 365 Remote Assist user, the **Insert file** button is removed from the mixed-reality toolbar. The user will see a message that says "File sharing is unavailable because your admin has disabled this feature. Please contact your admin for support." 


