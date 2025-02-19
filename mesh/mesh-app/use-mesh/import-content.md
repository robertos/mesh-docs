---
title: Import content
description: You can import your own content to the MyContent folder
ms.prod: mixed-reality
author: qianw211
ms.author: v-qianwen
ms.date: 11/11/2021
ms.topic: article
keywords: mixed reality, microsoft mesh, documentation, guides, features, holograms, spaces
---

# Import content

You can add 3D objects and 2D images to any space. You can then pinch an object to grab, move, rotate, and scale it. In a collaborative space, all users who are a member of the space can add, manipulate, annotate, and delete any objects.  

Here you will learn about how to:

* [Sync the MyContent folder on OneDrive.](#accessing-the-mycontent-folder)
* [Import user content.](#import-user-content)
* [Upload files from HoloLens or OneDrive.](#enable-local-file-picker)
* [Share content to a collaborative space.](#share-content-to-a-collaborative-space)

To work with contents, open the Taskbar from the Hand Menu, and choose the Content icon.

<img src="media\content-pane.png" alt="The content tab." width=500px>

In the Content pane, there are 3 places from which you can pull content into a space:

- **Samples**: This sample content is included in the app build.
- **OneDrive**: This is content that's inside of the Apps > Microsoft Mesh app (Preview) > MyContent folder on your OneDrive. Other users can't see this content. When you share it in a collaborative space, a copy is made for that space.
- **Space**: This is shared content that either you or another member added to the current space.

## Accessing the MyContent folder

The MyContent folder is created automatically when you select the **OneDrive** tab inside the Mesh app.  

<img src="media\mesh-onedrive.png" alt="Screenshot of the Microsoft Mesh Models - OneDrive." width=500px>

Once this folder is created, you'll need to take the following steps on your desktop to sync the folder:

1. Right click on the OneDrive icon on the Windows Taskbar.
1. Click **Help & Settings -> Settings**.
1. Go to the **Account** tab.
1. Click the **Choose folders** link.

    ![Screenshot of the Microsoft OneDrive Account tab dialogue box](media\onedrive-choose-folders.png)

1. In the folder view, expand the **Apps** folder and then make sure the box next to **Mesh app (Preview)** is checked.

    ![Screenshot of the Choose folders dialogue box](media\mesh-app-folder.png)

1. Click **OK** and close dialog boxes.

Now you can access the Apps > Microsoft Mesh app (Preview) > MyContent folder on your desktop and start adding your content for the Mesh app.  Desktop synchronization is beneficial for handling large file sizes and complex 3D models.  Alternatively if your content is small and not complex, you can also use OneDrive web.

## Import user content

You can add your own custom 3D content or images to OneDrive to make them available in the OneDrive folder in the app.

To add content to the User folder:

1. Go to OneDrive for Business on your PC and log in with the same Azure AD account that you used to log in to the Microsoft Mesh app.
1. In OneDrive, go to Apps > Microsoft Mesh app (Preview) > MyContent and copy files to this directory.
1. Once your files are copied to OneDrive, open the Content > OneDrive pane again to access them.

>[!Warning]
>For 3D content, only .glb files are supported at this time. We currently have a file size limit of 75MB, or maximum 300,000 vertex count for 3D models. If these limits are exceeded, you will fail to load your content, and get a warning: "This model is too complex". To resolve this, you can use [Azure Remote Rendering (ARR)](/mesh/mesh-app/arr-content), where more complex models can be loaded in your space.

The following 2D image file formats are supported: .png, .gif, .ico, .bmp, .tiff, .tif, .jpeg, .jpe, and .jpg.  For a .gif file, only the first frame will be loaded.

## Enable local file picker

You can upload a file from your Hololens or OneDrive folder into your space.  To do this, you will need to enable the **Local File Picker** option in **Experimental Features** by going through the following steps:  

1. Look at your hand to [bring up the menu](use-mesh.md#the-hand-menu), and press the **Main menu** button at the top.
1. Go to **Settings**, select **Experimental Features**.
1. Select **Local File Picker**.

    <img src="media\experimental-features-local-files.png" alt="Screenshot of the **Experiments** option under **Settings** tab." width=500px>

1. You can now see **+ Upload file** on the upper right corner of your **Content** pane.

    <img src="media\content-upload-files.png" alt="Screenshot of the Mesh app **Content** menu." width=500px>

## Share content to a collaborative space

You can share any content from the Samples or OneDrive folders to a collaborative space. This copies over the model file into your current space and shares the copy with all members of the space. Shared content for a space is stored in each users OneDrive under Apps > Microsoft Mesh app (Preview) > _spaceGUID_.space.

![Share content](media\share-content.png)

To add content to a space:

1. Open the Content pane.
1. Go to the Samples folder or OneDrive folder. In the OneDrive folder, the Mesh app displays a list of all the files you added to OneDrive.
1. Select a model.
1. The model is added to the current space.

## Additional resources

For other questions, see [Microsoft Mesh app troubleshooting and frequently asked questions](../faq.md).

- [Microsoft Mesh overview](../../overview.md)
- [Set up Microsoft Mesh for your organization](../../provisioning.md)
- [HoloLens](/hololens/)
- [Get started with Mixed Reality](/windows/mixed-reality/discover/get-started-with-mr)
- [Use the Mesh app](use-mesh.md)
- [Working with Azure Remote Rendering 3D models](arr-content.md)
