---
author: Mamaylya
description: Install and sign in to the Microsoft Dynamics 365 Guides HoloLens app as an operator.
ms.author: mamaylya
ms.date: 02/25/2020
ms.topic: article
title: Install the Dynamics 365 Guides HoloLens app (operators)
ms.reviewer: v-brycho
---

# Install and sign in to the Dynamics 365 Guides HoloLens app (operators)

1. Make sure that you have [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-hololens](../includes/pn-hololens.md)] build 10.0.14393.0 or later installed on your [!include[pn-hololens](../includes/pn-hololens.md)] device. We recommend that you update to newer versions when they are available. For information about how to use [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Update for Business, see [Manage updates to HoloLens](/HoloLens/hololens-updates).

2. On your [!include[pn-hololens](../includes/pn-hololens.md)] device, use the [bloom gesture](authoring-gestures.md) to open the **Home** menu. Then open the [!include[cc-microsoft](../includes/cc-microsoft.md)] Store app, and search for "[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]".

3. Select **Install** to download and install the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] application.

## Sign in to the HoloLens app

If you sign in to a brand-new [!include[pn-hololens](../includes/pn-hololens.md)] device, you will be prompted to complete the **Setup** wizard. In the **Setup** wizard, you can either sign in by using an existing account or create a new account, depending on the version of [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] that you're running. The **Setup** wizard also guides you through steps to calibrate and prepare [!include[pn-hololens](../includes/pn-hololens.md)] for use. 
 
## Open and sign in to HoloLens for the first time

1. Select **All Apps**.

    ![All Apps button.](media/hololens-apps.PNG "All Apps button")

2. Select the down arrow button.

    ![Down arrow button.](media/hololens-down-arrow.PNG "Down arrow button")

3. Open the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] app.

    ![Dynamics 365 Guides button.](media/open-guides-application.PNG "Dynamics 365 Guides button")
    
    > [!NOTE]
    > If you're using Dynamics 365 Guides version 7.0, you'll need to provide permissions to use the HoloLens eye tracker, camera, and microphone before you can sign in. [Learn more about permissions required to use the HoloLens app](hololens-permissions.md). 

4. On the **Welcome** page, select **Sign in**. 

5. On the **Email and accounts** page, select **Work or school account**, and then select **Continue**.

6. On the **Work or school account** page, enter the credentials that your admin provided. For the credentials, the user name will resemble `username@domain.com`. For example, if your user name is LauraO, and you work for the Contoso company, the user name will be `laurao@contoso.com`.

    ![Work or school account page.](media/sign-in-hololens.PNG "Work or school account page")

7. Select an instance to use, if you have more than one instance. Then select **Continue**.

> [!NOTE]
> If you're a Dynamics 365 Guides admin, you can assign the **Operator** role to operators so that they can view guides but can't edit them. If you assign the **Operator** role to a user, the user can also skip the step in the **Select Mode** dialog box and open a guide directly. For more information, see [Assign an Author or Operator role to a user](assign-role.md).

## Sign out of the HoloLens app in Dynamics 365 Guides version 7.0

If you're using Dynamics 365 Guides version 7.0, you can sign out by using touch.

1. Look at your palm to open the Main menu, and then select the **Profile** button.

    ![Screen shot of hand and Main menu.](media/main-menu.PNG "Screen shot of hand and Main menu")
    
2. Select **Sign out**. 

## What's next?


[Find a guide](find-guide.md)<br>
[Gestures for navigating the HoloLens app](operator-gestures.md)<br>
[Anchor your guide](operator-anchor.md)<br>
[Operate a guide](operator-step-card-orientation.md)
[Calibrate your HoloLens](operator-calibrate.md)<br>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
