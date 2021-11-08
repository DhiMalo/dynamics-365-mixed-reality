---
author: Mamaylya
description: Learn how to opt out of storing Microsoft Dynamics 365 Guides usage data in Microsoft Dataverse, for privacy reasons.
ms.author: mamaylya
ms.date: 11/08/2021
ms.topic: article
title: Microsoft Dataverse data opt out for Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Opt out of storing Dynamics 365 Guides operations data in Microsoft Dataverse

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Dynamics 365 Guides apps enable teams to capture usage statistics and detailed time-tracking information. This data is used to 
provide metrics for operator performance and help you identify opportunities for process optimization. Administrators can turn off 
data collection for specific users if they like. 

To do this:

1. Go to powerapps.microsoft.com and sign in with your admin account.

2. In the tenant/instance drop-down, select the instance that has Dynamics 365 Guides installed.

3. Select the **Guides** app in the list. A new tab for the Guides model-driven app is opened.

    > [!NOTE]
    > The Guides model-driven app isn't intended as a replacement for authoring in the PC and HoloLens apps. If you use the model-driven app to create, update, or delete records, you might make Guides nonfunctional or prevent users from using the PC or HoloLens apps in the intended way. Currently, modification through the model-driven app isn't fully supported and should be reserved for experienced Dynamics 365 developers who are familiar with Microsoft Dataverse.

4. On the left side of the screen, select the up arrow next to **Main**, and then select **Settings**.

    ![User Settings.](media/data-opt-out-user-setting.PNG "User Settings")
 
5. Select **New**.

    ![Select New.](media/data-opt-out-new.PNG "Select New")
 
6. In the **New User Settings** screen, under **User Settings**, fill out the form as follows:

    - **Name:** Opt out for *[User name]*

    - **Record Guide Usage:** Yes

    - **Belongs To:** *[User name]*

    ![Filled-out form.](media/data-opt-out-filled-out-form.PNG "Filled-out-form")
    
7. Select **Save** at the top of the screen.
 
## See also

[Overview of analyzing and integrating Dynamics 365 Guides operations data](analytics-overview.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
