---
author: Mamaylya
description: Learn how to fix a corrupted guide in Dynamics 365 Guides
ms.author: mamaylya
ms.date: 06/09/2022
ms.topic: article
title: Fix a corrupted guide in Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# Fix a corrupted guide in Dynamics 365 Guides

In very rare cases, you may find that a guide created in Microsoft Dynamics 365 Guides has become corrupted. This is most commonly associated with guides that were [shared with authors](admin-share-guide.md) in the time period from September 2021 to December 2021. When sharing a guide with an author, you must select the **Read**, **Write**, and **Append to** permissions. 

![Screenshot of Share records dialog box with privileges selected.](media/corrupted-guide-share-records.jpg "Screenshot of Share records dialog box with privileges selected")

For guides shared with an author between September 2021 and December 2021, however, due to a bug in Dynamics 365 Guides, the **Append to** permission could not be set. If an author added one or more steps to a shared guide, and then saved the guide, the guide would become corrupted. If you open a corrupted guide in the PC app, you'll see the following message. 

![Screenshot of message that appears when a guide is corrupted.](media/corrupted-guide-message.jpg "Screenshot of message that appears when a guide is corrupted")

> [!NOTE]
> A guide can also become corrupted if you use the [model-driven app](open-model-driven-app.md) to delete a step (instead of deleting the step in the PC app). 

## Run a flow to fix a corrupted guide

You can fix a corrupted guide by running a flow in the model-driven app. 

1. [Open the model-driven app](open-model-driven-app.md).

2. Open the corrupted guide. 

3. On the **Flow** menu, select **Repair corrupted guide**.

    ![Screenshot of Repair corrupted guide flow command.](media/repair-corrupted-guide-flow.jpg "Screenshot of Repair corrupted guide flow command")

4. In the **Confirmation Application of Workflow** dialog box, select **OK**.
    
    ![Screenshot of Workflow confirmation dialog box.](media/workflow-confirmation.jpg "Screenshot of Workflow confirmation dialog box")
    
5. Wait a few minutes for the flow to complete.

## Make fixes in the PC app

The flow that you run from the model-driven app recreates steps in the correct places in the PC app for any steps that:

- Weren't saved correctly due to the **Append to** issue described above.

- You deleted in the model-driven app.

Other guide steps might appear in random positions, however, after running the flow. For example, if your guide has three steps, and the issue is with step 2, when you open the PC app, the steps might look like this. 

![Screenshot of steps in the PC app after running the flow.](media/corrupted-guide-pc-app-steps.jpg "Screenshot of steps in the PC app after running the flow")

At this point, you need to:

1. Add content to any recreated steps.

2. Drag steps to place them in the right order.
