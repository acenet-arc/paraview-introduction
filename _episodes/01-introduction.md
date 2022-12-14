---
title: "Introduction to Paraview"
teaching: 5
exercises: 0
questions:
- "What is Paraview?"
objectives:
- Understand what Paraview is and where it can be used.
keypoints:
- "Paraview is open-source visualization software"
- "It loads in structured and unstructured 3D datasets of scalar and vector data."
- "It is available for Windows, MacOS and Linux"
---

## In one sentence

Paraview is an open-source science/data visualization and data analysis
package developed by <a href="https://www.kitware.com">Kitware</a>, that
is designed for interactive and batch use within many domains and
disciplines, such as engineering, computational fluid dynamics, medical
science, material science and sensor data.

## What Paraview does

Paraview can be run straight from a desktop, reading data in directly from
storage:

![Visualization process overview]({{ page.root }}/fig/visualisation-process-overview.jpg){: width="45%" }

Alternatively, for very large datasets, Paraview can be run in client-server
mode, with processing done remotely on a cluster or more powerful server
computer, but rendered on a local desktop:

![Visualization process with processing server]({{ page.root }}/fig/visualisation-with-server.jpg){: width="65%" }

{% include links.md %}
