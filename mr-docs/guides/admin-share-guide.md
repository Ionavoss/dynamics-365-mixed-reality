---
title: Share a guide in Dynamics 365 Guides
description: Learn how to share a guide in Microsoft Dynamics 365 Guides by using an access team.
author:  Mamaylya
manager: tfehr
ms.topic: conceptual
ms.date: 04/05/2022
ms.author: mamaylya
ms.reviewer: v-wendysmith
---

# Share a guide in Dynamics 365 Guides

In Microsoft Dynamics 365 Guides, you can share a guide with other users if you're an administrator or if you have the Share privilege. You can do this by sharing a guide with a specific user or an [access team](admin-access-teams.md).

> [!IMPORTANT]
> [Assigning ownership of a guide](admin-access-assign.md) to a user or team is the preferred method for controlling who can use specific guides. Sharing a guide does not change ownership of the guide. [Learn how to change guide ownership](admin-access-assign.md)

## Share a guide

1. In the PC authoring app, sign in to the Dynamics 365 instance that includes the guide.

2. Select the **Analyze** tab, and then under **Instance URL**, select **Copy**, and then paste the value into the address bar of a web browser.

    ![Instance URL value highlighted.](media/copy-instance-url.jpg "Instance URL value highlighted")

3. Sign in, and then in the left pane of the Power Apps screen, select **Guides** to open the model-driven app.

    ![Screen shot of Power Apps screen showing Guides model-driven app.](media/guides-hub-1.PNG "Screen shot of Power Apps screen showing Guides model-driven app")
    
4. Find the guide that you want to share, select the check box next to the guide name, and then select **Share**.

    ![Check box for specific guide selected.](media/access-teams-19.PNG "Check box for specific guide selected")

5. In the **Share records** page, use the search box to search for and select the appropriate team or user name.

     ![Screen shot of Share records page.](media/share-records.jpg "Screen shot of Share records page")
    
6. Under **Manage share access**, select the team, and then select specific permissions:

   - For operators, select **Read** permissions (and **Append to** if you want to [collect operations data](analytics-overview.md)).
   - For authors, select **Read**, **Write**, and **Append to** permissions.

    ![Screen shot of Manage share section.](media/manage-share-access.jpg "Screen shot of Manage share section")
    
7. Select **Share**. 

> [!TIP]
> When you share a guide, the content (images, videos, and 3D objects) associated with the guide is not automatically shared. You can use the **All Content** tab in the Guides model-driven app to do bulk operations, such as sharing content. 
>
> ![Screenshot of All Content tab in the Guides model-driven app.](media/mda-all-content-tab.PNG "Screenshot of All Content tab in the Guides model-driven app") 

## See also

- [Create an access team](admin-access-teams.md)
- [Assign an Operator or Author role to an individual user](assign-role.md)
- [Assign roles in bulk by using Active Directory groups](admin-assign-role-groups.md)
- [Restrict access to an environment by using security groups](admin-security.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]







