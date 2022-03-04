---
title: Dynamics 365 Remote Assist mobile overview
author: amaraanigbo
description: Get an overview of the Dynamics 365 Remote Assist mobile app capabilities.
ms.author: soanigbo
ms.date: 10/01/2020
ms.topic: overview
ms.reviewer: v-bholmes
---

# Dynamics 365 Remote Assist mobile overview



Dynamics 365 Remote Assist enables technicians with mobile devices to connect to a remote collaborator on Dynamics 365 Remote Assist mobile or Microsoft Teams (desktop and mobile). Using live video calling, mixed-reality annotations, and high-resolution snapshots, they can share what they see with the remote collaborator to troubleshoot problems together, faster.

Dynamics 365 Remote Assist mobile is beneficial in scenarios where technicians may need physical access to confined or hard-to-reach spaces, or access to other mobile apps that are part of their organizations' workflows. With the availability and familiarity with mobile devices, technicians can use Dynamics 365 Remote Assist mobile during repairs and inspections with ease. Furthermore, Dynamics 365 Remote Assist mobile allows for easier broad-scale deployment in organizations.

Dynamics 365 Remote Assist is available on [Android phones and tablets with ARCore support](https://developers.google.com/ar/discover/supported-devices) and [iOS iPhones and iPads with ARKit support](https://developers.google.com/ar/discover/supported-devices#ios). Additionally, Dynamics 365 Remote Assist is available on mobile devices **without** ARCore or ARKit support, too! Visit our [documentation on product requirements](../requirements.md) to learn more.

## Features

- One-to-one and group video calling.
- Add mixed reality annotations in space.
- Use asset capture in offline scenarios so that users can annotate, capture, and visualize images and videos of assets and store them in Common Data Service. 
- Annotate on a 2D image capture, or snapshot, of the space during a call.
- Send and receive messages, in-call snapshots, and files through the text chat.
- Capture session history through call recordings.
- Annotate and share in-call snapshots in low-bandwidth scenarios.
- Integration with Microsoft Dynamics 365 for Field Service.
- Ability to link call history, in-call snapshots, and files shared during a Dynamics 365 Remote Assist mobile call to an associated Dynamics 365 Field Service work order.
- Ability to start a call to a remote collaborator from the Dynamics 365 Field Service mobile app to the Dynamics 365 Remote Assist mobile app.
- Availability on mobile devices without augmented reality (AR) support.

![Simulated image of a technician using Dynamics 365 Remote Assist mobile to annotate their environment on a call.](./media/ram-overview.png "Dynamics 365 Remote Assist mobile Overview")

## Microsoft Intune support

Dynamics 365 Remote Assist mobile for iOS and Android supports Microsoft Intune's app protection policies. These policies ensure that data remains safe and contained on the device through Intune policies.  

![Graphic showing Intune controls.](./media/RAM_IntuneControls.png)

For more information on Microsoft Intune's app protection policies, see [this article](/mem/intune/apps/app-protection-policy).

### Set up configuration policies for Android devices

> [!NOTE]
> At this time, you can't set up configuration policies for iOS devices.

You must be an administrator to set up configuration policies.

1. Go to [Microsoft Endpoint Manager](https://endpoint.microsoft.com/). 

2. On the left side of the screen, select **Apps**, and then select **App configuration policies**. 

3. Select **Add**, and then select **Manage Apps**. 

4. In the **Name** field, enter the name of the policy, and then in the **Target policy to** field, select **Selected apps**.  

    SCREENSHOT GOES HERE 
    
5. Under **Public apps**, choose **Select public apps**, and then select **Dynamics 365 Remote Assist Android**. 

    SCREENSHOT GOES HERE
    
6. Go to the configuration settings page, and then do the following:

    1. Set the **Name** field to "com.microsoft.ramobile.environment.instance.url". 

    2. In the **Value** field, enter the environment url. You can find this url in the [Power Platform admin center](https://admin.powerplatform.microsoft.com)  **Environment** section. Learn more: [Create and manage environments in the Power Platform admin center](https://docs.microsoft.com/power-platform/admin/create-environment)

    SCREENSHOT GOES HERE
    
7. To select the groups that will receive the configuration policy:

    1. Select **Add groups**.

       SCREENSHOT GOES HERE

    2. Select the correct group(s) for your tenant.

       SCREENSHOT GOES HERE
       
8. Confirm to create the new configuration policy. 

## Videos

- [Watch a video on a technician using Dynamics 365 Remote Assist mobile on-site](https://www.youtube.com/watch?v=J-C6GE2gFYw&t=27s).
- [Watch a live demo of Dynamics 365 Remote Assist mobile in action, from signing in to ending the call](https://www.youtube.com/watch?v=DQJWsCDNpb4&t=1s).

## See also

- [Try Dynamics 365 Remote Assist mobile for free](../try-remote-assist.md).
- [Buy Dynamics 365 Remote Assist licenses](../buy-remote-assist.md).
- [Deploy Dynamics 365 Remote Assist to your workers' devices](../deploy-remote-assist.md).
- [How-to videos for using Dynamics 365 Remote Assist on mobile](../videos.md).
- [Dynamics 365 Remote Assist mobile - FAQs](/dynamics365/mixed-reality/remote-assist/faq#using-remote-assist-on-mobile).


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
