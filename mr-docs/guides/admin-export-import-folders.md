---
author: melissahellmund
description: Learn how to export and import Dynamics 365 Guides folders between environments
ms.author: mehellmu
ms.date: 11/08/2021
ms.topic: article
title: Export and import Dynamics 365 Guides folders between environments
ms.reviewer: v-wendysmith
---

# Export and import Dynamics 365 Guides folders between environments

You can export the folders you have created in Microsoft Dynamics 365 Guides and import them into another environment to recreate your file structure. The guides, 3D 
content, and media associated with these folders will not be included in this process. However, you can use the [Content Migration Tool](migrate.md) to migrate this content after you’ve imported your folders.  

> [!NOTE]
> If you export and import your folders first, and then migrate the content, the relationships between the folders and the content will be reconstructed.

## Prerequisites 

- You must be a system administrator to access the Power Platform admin center.  

- You must have Dynamics 365 Guides solution version 600.1.0.0 or later.  

We also highly recommend [backing up the contents](/power-platform/admin/backup-restore-environments#create-a-manual-backup) of both environments before starting the export/import process. 

## Export the folders

1. Go to [make.powerapps.com](https://make.preview.powerapps.com/), and then sign into the environment that contains the folders you want to export. 

2. In the left navigation pane, select **Solutions**. 

    ![Power Apps screen with Solutions command selected.](media/export-folders-01.PNG "Power Apps screen with Solutions command selected")

3. Create a new solution by doing the following:  

    1. In the command bar, select **New solution**.  

    2. Enter a display name. This will be the name of your solution.  

    3. Select **Default Publisher for {orgid}** from the drop-down menu.  

    4. Select **Create**.  

       ![Power Apps screen with 4 choices highlighted.](media/export-folders-02.PNG "Power Apps screen with 4 choices highlighted")

4. Add the folders as components of your solution:  

    1. Select the solution you just created.  

    2. Select **Edit**.  

       ![Power Apps screen with solution and Edit button highlighted.](media/export-folders-03.PNG "Power Apps screen with solution and Edit button highlighted")

    3. Select **Add existing** > **More** > **Other** > **Folder**.  

       ![Power Apps screen with Add existing and Folder highlighted.](media/export-folders-04.PNG "Power Apps screen with Add existing and Folder highlighted")

    4. Select the folders you want to include in your export, and then select **Add**.  

       ![Power Apps screen with Add highlighted.](media/export-folders-05.PNG "Power Apps screen with Add highlighted")
 
       > [!NOTE]
       > If you select a folder that includes subfolders, you'll need to select the parent folder and the child folder individually. However, if you select a subfolder, the parent folder will automatically be added to the list that will be exported. 

5. To export your solution:  

    1. Select **Export**, and then select **Next**. 

       ![Power Apps screen with Export and Next highlighted.](media/export-folders-06.PNG "Power Apps screen with Export and Next highlighted")

    2. Select between a managed and an unmanaged solution, and then select **Export**.  

       ![Export this solution pane with Managed option selected and Export button highlighted.](media/export-folders-07.PNG "Export this solution pane with Managed option selected and Export button highlighted")
       
       > [!NOTE]
       > Select a managed solution if you want the rows to be bundled with the solution. This means that if you delete the solution, the rows that were imported as part of the managed solution will be deleted as well (including any guides saved under the folders, since deletion of a folder includes any subfolders). On the other hand, if you delete an unmanaged solution from the environment, the rows will persist.

    3. Once the export is ready, it's automatically downloaded as a .zip file. You’ll see a green notification saying it has been exported successfully. This might take a while.   

       ![Power Apps screen with green notification.](media/export-folders-08.PNG "Power Apps screen with green notification")
      
       > [!NOTE]
       > Deactivated folders will appear on the list to be exported.
      
### Import the folders

1. Go to [make.powerapps.com](https://make.preview.powerapps.com/) and **ensure you are in the environment where you want to import the folders**. You can check this in the top right corner of the screen under **Environment**.  

    ![Power Apps screen showing where to check for the correct environment.](media/export-folders-09.PNG "Power Apps screen showing where to check for the correct environment")

2. In the left navigation pane, select **Solutions**.  

3. In the command bar, select **Import**, and then in the **Import a solution** pane, select **Browse**.  

    ![Power Apps screen with Import and Browse highlighted.](media/export-folders-10.PNG "Power Apps screen with Import and Browse highlighted")

4. In the **Open** dialog box, find the .zip file you just downloaded, select it, and then select **Open**.  

    ![Open dialog box with Zip file and Open button highlighted.](media/export-folders-11.PNG "Open dialog box with Zip file and Open button highlighted")

5. Select **Next**.  

    ![Import a solution pane with Next button highlighted.](media/export-folders-12.PNG "Import a solution pane with Next button highlighted")

6. Select **Import**.  

    ![Import a solution pane with Import button highlighted.](media/export-folders-13.PNG "Import a solution pane with Import button highlighted")

    When the import is complete, you'll see a notification stating that the solution has been successfully imported. This might take a few minutes.
 
    ![Power Apps screen with notification showing solution successfully imported.](media/export-folders-14.PNG "Power Apps screen with notification showing solution successfully imported")
    
## See also

[Create folders](admin-create-folders.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
