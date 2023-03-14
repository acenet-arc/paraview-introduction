---
title: Setup
---

## Downloading Paraview

To download Paraview to your local machine, go to [www.paraview.org/download](https://www.paraview.org/download/). It should you a web page similar to that below.

<img src="fig/paraview-download.jpg" width="75%" alt="Paraview MacOS download page">

The website should automatically select the correct operating system (OS) for
you, ie. Windows, MacOS or Linux. Each OS has a slightly different installation
procedure; we will focus upon MacOS below. 

In the example screenshot above, we would select either of the download links
highlighted:

* Ending in `x86_64.dmg` - for Intel based Macs
* Ending in `arm64.dmg` - for Apple Macs with M1 or M2 processors

Be sure you know what type of Mac you are using. 

## Installing Paraview

Once you have the correct `.dmg` file (MacOS) or `.msi` file (Windows),
click on it and follow the instructions. You should first see a end-user
agreement:

<img src="fig/paraview-agreement.jpg" width="60%" alt="Paraview agreement">

Click on 'Agree' then let the installation continue. On MacOS, you will be
prompted to drag Paraview into the Applications folder:

<img src="fig/paraview-to-applications.jpg" width="35%" alt="Paraview application folder drag">

Drag the Paraview icon into the Applications folder. Paraview should now be
installed.

## Getting the Paraview examples

We have some example visualization files required for this lesson. You can
download the ZIP file from <a href="https://github.com/acecreech/paraview-lesson/releases/download/v0.1/acenet-paraview-examples.zip">here</a> (96 MB).

Once that is downloaded, you will need to extract them. Under MacOS, this can
be done simply by clicking on the ZIP file. Doing so will create a directory
called

`acenet-paraview-examples/`

This directorycontains all the Paraview files you will need for this lesson.
The notes assume that you have extracted the ZIP file under **Desktop/**.


{% include links.md %}
