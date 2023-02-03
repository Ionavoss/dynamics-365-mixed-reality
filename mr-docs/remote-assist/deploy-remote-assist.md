---
title: Deploy Dynamics 365 Remote Assist
author: amaraanigbo
description: Dynamics 365 Remote Assist users can deploy and set up Dynamics 365 Remote Assist on their devices. 
ms.author: soanigbo
ms.date: 06/17/2022
ms.topic: article
ms.reviewer: v-wendysmith
---

# Deploy Dynamics 365 Remote Assist

After you get your [free trial](try-remote-assist.md) or [purchase](buy-remote-assist.md) Dynamics 365 Remote Assist, you can assign licenses to users. Once assigned, users can deploy Dynamics 365 Remote Assist on their individual devices.

> [!Note]
> There are two types of users for Dynamics 365 Remote Assist and Dynamics 365 Remote Assist Attach: remote experts and field service technicians. Field service technicians require a Dynamics 365 Remote Assist license **and** a Microsoft Teams license. When you buy a Dynamics 365 Remote Assist license, a Microsoft Teams license is included. However, remote experts (who aren't in the field) require only a Microsoft Teams license. 

In this article, we’ll walk through how to deploy Dynamics 365 Remote Assist or Dynamics 365 Remote Assist Attach (for Field Service customers). This includes:

-	Assigning licenses to users in your organization (for IT Admins)

-	Deploying Dynamics 365 Remote Assist on a device (for individuals in your organization) 

You can also learn how to [deploy to multiple tenants](multi-tenant-deployment.md) or [enable vendors and contractors to use Dynamics 365 Remote Assist](vendor-use-RA.md).

## Add and assign licenses

### Prerequisites

Your organization must have:

- A Microsoft 365 or Microsoft 365 [administrator account](https://www.microsoft.com/microsoft-365/business/office-365-administration). [Learn more about admin permissions](/office365/admin/admin-overview/admin-overview). 

- A [free trial](try-remote-assist.md) of Dynamics 365 Remote Assist, or a [purchased license](buy-remote-assist.md). 

- An Azure Active Directory account for each licensed user. They'll use Azure Active Directory to sign into the app.

Make sure that users in your organization have the required licensing and devices. For more information, see [licensing and product requirements](./requirements.md).

### Adding and assigning licenses

Once prerequisites are met, you can now add and assign licenses to *individual users* or a *group of users* in your organization through the Microsoft 365 or Microsoft 365 administrator portal. 

1.	Log into the [Microsoft 365 or Microsoft 365 administrator portal](https://www.microsoft.com/microsoft-365/business/office-365-administration ) using your organization’s admin account.

    ![Screenshot of the admin portal.](./media/buy_1.png "Admin Portal")

2.	Make sure the **Try the new admin center** toggle is turned off.

3.	In the left navigation bar, select **Billing** > **Subscriptions**. 

    ![Screenshot showing billing subscriptions.](./media/deploy_3.png "Billing subscriptions")

4.	Select **Assign to users**. 

    ![Screenshot showing assigning users.](./media/deploy_4.png "Assign users")

5. Select **Add a user**. For more information, see [Add users and assign licenses at the same time](/office365/admin/add-users/add-users).

6.	Find the users in your organization that you want to add. In the **Product licenses** section, make sure to provide them with Dynamics 365 Remote Assist and Microsoft Teams licenses. 

    ![Screenshot of product licenses.](./media/deploy_6.png "Product licenses")

7. To add multiple users, go to **More** > **Import multiple users**. Fill out the CSV file, set user options, and view your results. 

    ![Screenshot of adding multiple users.](./media/deploy_7.png "Add multiple users")

8.	After you have added a user or users, you can assign licenses to them through the Microsoft 365 or Microsoft 365 administrator portal. See [Assing licenses to users](/office365/admin/manage/assign-licenses-to-users).

At this point, users in your organization can set up Dynamics 365 Remote Assist on their devices, as described below. 

> [!NOTE]
> [Learn about the platforms that Dynamics 365 Remote Assist is dependent on and how those dependencies can affect the app](faq-deploy.md)

## Download and install the app

After assigning licenses, users can set up and use the app on their HoloLens, HoloLens 2, or mobile devices. 

### Prerequisites

- The organization's IT admin must add the user and assign a Dynamics 365 Remote Assist license **and** Microsoft Teams license in the Microsoft 365 or Microsoft 365 administrator portal, as described above. 

- A [Microsoft Teams account](https://teams.microsoft.com/start). See [Using Teams with Dynamics 365 Remote Assist](/dynamics365/mixed-reality/remote-assist/set-up-teams) for more information.

- Azure Active Directory [Premium trial](https://azure.microsoft.com/trial/get-started-active-directory/) (for HoloLens users only).

- A HoloLens, HoloLens 2, or mobile device. See [Licensing and product requirements](./requirements.md).

### Steps for HoloLens and HoloLens 2

1.	Go to the **Start** menu select **Dynamics 365 Remote Assist** to update or launch the app. If you don't find the app installed by default, go to the Microsoft Store and get it there. 

3.	Sign into Dynamics 365 Remote Assist with your Microsoft Teams account. 

4.	You'll be taken to your **Contacts** page. If you're using a free trial, you'll be prompted to start your **Free Trial of Dynamics 365 Remote Assist**. 

5.	You can now use Dynamics 365 Remote Assist on your HoloLens or HoloLens 2. Next up, [Learn how to make calls](making-taking-calls-hololens.md). 

### Steps for mobile devices

1.	Go to the appropriate iOS or Android app store.

2.	Search for and download **Dynamics 365 Remote Assist** and launch the app.

3.	Sign into Dynamics 365 Remote Assist with your Microsoft Teams account. 

4.	You'll be taken to your **Contacts** page. If you're using a free trial, you'll be prompted to start your **Free Trial of Dynamics 365 Remote Assist**.

5.	You can now use Dynamics 365 Remote Assist on your mobile device. Next up, [Learn how to make calls](mobile-app/making-calls-with-ar.md). 

>[!Note]
> For Enterprise environments that manage application deployments using an MDM provider, contact d365rafb@microsoft.com for assistance obtaining the Dynamics 365 Remote Assist mobile application binary.

## Next steps
- [Set up Microsoft Teams on a PC or mobile for various scenarios](set-up-teams.md)
- [Install the Dynamics 365 Remote Assist model-driven app](ra-webapp-install.md)
- [Learn about the platforms that Dynamics 365 Remote Assist is dependent on](faq-deploy.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
