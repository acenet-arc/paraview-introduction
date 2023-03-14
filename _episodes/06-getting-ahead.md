---
title: "Working with real data: getting ahead"
teaching: 10
exercises: 15
questions:
- "How do I extract data from real data"
objectives:
- 
- 
---

## Introduction

In this section, we will look at loading in data from an MRI scan of a human
head. 

## Opening and viewing the file

* Click on **File** then **Open**.
* Navigation to the **acenet-paraview-examples/** directory.
* Select the file **mri-scan.pvd**, then click **OK**.
* Click **Apply** in the Properties tab.

You should see a wireframe box. We'll need to change the rendering to
**Volume**. In the toolbar, you'll see a drop-down menu that currently says
**Outline**. Select **Volume** from this menu.

![MRI scan volume selected]({{ page.root }}/fig/mri-volume-selected.jpg){: width="85%" }

Zooming in a bit, you should have a view of the head clearly. Changing the
colormap to **Rainbow Desaturated** (See the 'Introducing filters' episode,
under *Changing the colormap*), and turning on the colormap legend, you
should see something similar to this.

![MRI with rainbow desaturated colormap]({{ page.root }}/fig/mri-colormap-legend.jpg){: width="85%" }

As the render type *Volume* suggests, this is a full volumetric render of
3D data. DICOM, incidentally, stands for *Digital Imaging and Communications
in Medicine*, and is a standard for storing and tranmitting medical images.
More can be found on DICOM at the
<a href="https://www.dicomlibrary.com/">DICOM Library</a>. For now though,
we'll treat the *DICOMImage* field in Paraview as a measure of object density.


## Measuring dimensions

Paraview is not designed by default to deal with MRI scans, although it does
support DICOM image sets. That said, we can still get useful information out
of them. This we will do now.

Let's suppose we want to get the horizontal dimensions of the head above the
eyebrow. Firstly, we create a **Slice** filter, select **Y Normal**, then click
**Apply**. 

![MRI first slice]({{ page.root }}/fig/mri-first-slice.jpg){: width="85%" }

By clicking and dragging the red horizontal edge of the slice, we can move
this to above the eyebrows of the head. Do this, and then:

* Hide the original full 3D MRI image, by clicking on the eye icon next
to **mri-scan.pvd**.
* Reorient the view to look down on the slice by clicking on the -Z axis
icon in the toolbar.

![Paraview minus Z axis]({{ page.root }}/fig/paraview-toolbar-minuszaxis.jpg){: width="65%" }

Zooming in a bit gives a clearer view in the main window.

![MRI slice main view top down]({{ page.root }}/fig/mri-main-window-slice.jpg){: width="65%" }

We are going to assume that green shell represents the skull,
with the light blue being the outer layers of skin and tissue. We want
to measure the cranium.

Firstly, we make the view 2D. We do this by click on the *3D* button at
the top of the main viewer window. 

![Main viewer 3D button]({{ page.root }}/fig/mri-3D-button.jpg){: width="45%" }

This will change the view to 2D, which makes our next tasks easier. You want
to zoom in again at this point.

{% include links.md %}
