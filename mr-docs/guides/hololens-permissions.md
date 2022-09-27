---
author: chantiff
description: Learn about the HoloLens permissions required to use Dynamics 365 Guides 7.0.
ms.author: chantiffany
ms.date: 11/08/2021
ms.topic: article
title: HoloLens permissions required to use version 7.0 of Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# HoloLens permissions required to use Dynamics 365 Guides

To use certain features in the Microsoft Dynamics 365 Guides HoloLens app, you must provide permissions. When you open the HoloLens app for the first time, you're prompted to provide these permissions through separate dialog boxes. For example, you'll see this dialog box for the eye tracker.

![Permissions dialog box for eye tracker.](media/hololens-permissions-eye-tracker.PNG "Permissions dialog box for eye tracker")

If you don't provide permissions through any these dialog boxes, you'll see the following dialog box that prompts you to provide the necessary permissions.

![Guides permissions dialog box.](media/hololens-permissions-guides.jpg "Guides permissions dialog box")

You can't use the HoloLens app until you provide these permissions. 

|Permission|Why required|
|----------------------|----------------------------------------------------------|
|Eye tracking|Required to use the main menu and to create a great experience. Eye tracking lets HoloLens know what you’re looking at and helps validate your intentions.<br><br>Eye tracking has been designed with user privacy in mind. Microsoft doesn’t store any biometric or other identifiable information.| 
|Camera|Required to make video calls, to understand the space around you, and more.| 
|Microphone|Required to make voice calls and use voice commands.|  

You can also turn on each permission by following the steps described below.

### Give permission to use eye tracking

1. Go to **Settings** > **Privacy**. 

2. Do the following:

    1. On the left side of the screen, under **App permissions**, select **Eye tracker**.

    2. On the right side of the screen, under **Allow apps to access your eye tracker**, turn the setting to **On**.  

    3. On the right side of the screen, under **Choose which apps can access your eye tracker**, turn the **Dynamics 365 Guides** setting to **On**. 

    ![Screenshot of selected settings for eye tracker.](media/hololens-permissions-eye-tracker-settings.PNG "Screenshot of selected settings for eye tracker")

[Learn more about Windows 10 eye tracking and privacy](https://support.microsoft.com/en-us/windows/windows-10-eye-tracking-and-privacy-62623324-36cf-04a3-6992-8f329081f20b)

### Give permission to use the camera 

1. Go to **Settings** > **Privacy**.

2. Do the following:

    1. On the left side of the screen, under **App permissions**, select **Camera**.

    2. On the right side of the screen, under **Allow access to the camera on this device**, turn the setting to **On**. This also turns on the **Allow apps to access your camera** setting.

    3. On the right side of the screen, under **Choose which apps can access your camera**, turn the **Dynamics 365 Guides** setting to **On**. 

    ![Screenshot of selected settings for camera.](media/hololens-permissions-camera-settings.PNG "Screenshot of selected settings for camera")

[Learn more about Windows camera, microphone, and privacy](https://support.microsoft.com/en-us/windows/windows-camera-microphone-and-privacy-a83257bc-e990-d54a-d212-b5e41beba857#ID0EBD=Windows_10)

### Give permission to use the microphone

1. Go to **Settings** > **Privacy**.

2. Do the following:

    1. On the left side of the screen, under **App permissions**, select **Microphone**.

    2. On the right side of the screen, under **Allow access to the microphone on this device**, turn the setting to **On**. This also turns on the **Allow apps to access your microphone** setting.

    3. On the right side of the screen, under **Choose which apps can access your microphone**, turn the **Dynamics 365 Guides** setting to **On**. 

    ![Screenshot of selected settings for microphone.](media/hololens-permissions-microphone-settings.PNG "Screenshot of selected settings for microphone")

[Learn more about Windows camera, microphone, and privacy](https://support.microsoft.com/en-us/windows/windows-camera-microphone-and-privacy-a83257bc-e990-d54a-d212-b5e41beba857#ID0EBD=Windows_10)

## See also

- [Install and sign in to the HoloLens app](hololens-app-install-sign-in.md)
- [Frequently asked questions about Dynamics 365 Guides](faq.md)
