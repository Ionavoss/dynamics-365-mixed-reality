---
author: RobertButterworthMS
description: Overview of converting and optimizing 3D models to use with Dynamics 365 Guides and Microsoft Power Apps
ms.author: robutter
ms.date: 01/08/2020
ms.topic: overview
title: Overview of preparing 3D models for Dynamics 365 Guides and Power Apps
ms.reviewer: v-bholmes
---

# Overview of preparing 3D models for Dynamics 365 Guides or for mixed-reality components included in apps created with Power Apps

If you're using Microsoft Dynamics 365 Guides, or creating apps with mixed-reality components in Power Apps, you might want to import your own 3D models for use as holograms. This article shows you how to prepare your 3D models by using a combination of third-party tools.

## glTF and GLB file formats
Dynamics 365 Guides and Power Apps uses the Khronos Group glTF file format for mixed reality. This royalty-free specification minimizes both the size of 3D models and the run-time processing needed to unpack and use those models. The GLB format is the binary version of glTF version 2.0, which can include textures.

> [!TIP]
> The Khronos Group provides a robust overview of best practices: [Art Pipeline for glTF](https://aka.ms/glTFbestpractices).

## Parametric geometry vs. polygonal geometry

Modeling tools in most CAD applications use sets of adjustable mathematical parameters to define parametric solids. Parametric solids and surfaces provide highly accurate detail that can be used to carry out engineering simulations and manufacturing processes. Both glTF and real-time rendering applications require models to be represented as a triangulated polygon surface.

The following illustration shows a model visualized in Autodesk Inventor and Microsoft 3D Viewer.
> [!div class="mx-imgBorder"]
> ![Parametric versus polygonal geometry.](media/compare-geometry.PNG "Parametric versus polygonal geometry")

**A.**	Parametric 3D model ready for simulation and manufacturing<br>
**B.**	Polygonal surface 3D model ready for real-time rendering

## Overall process for preparing 3D models

Preparing CAD content for Dynamics 365 mixed-reality apps involves two steps: 

1.	[**Convert 3D models**](convert-models.md) from their original geometric definition into one that supports real-time rasterization. This converts the models from parametric geometry into polygonal geometry.

2.	[**Optimize the converted 3D models**](optimize-models.md) to ensure the best possible performance in real-time applications.

### See also
- [Convert 3D models](convert-models.md)
- [Optimize 3D models](optimize-models.md)
- [Best practices for converting and optimizing 3D models](best-practices.md)
- [Review a 3D model](review-3d-model.md)
- [Tutorials for converting and optimizing 3D models](tutorials-overview.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
