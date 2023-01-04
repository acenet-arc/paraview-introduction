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


## Processing data with filters

One of the most powerful features in Paraview, is that it can chain together
a series of operations known as *filters* to operate on data. Filters can be
connected in series, taking input from the previous filter's output, operate
on it, and pass it to the next filter.

![Paraview filter chain]({{ page.root }}/fig/paraview-filter-chain.jpg){: width="55%" }

You can also `branch off' the chain, with seperate filters to create multiple
visualizations.

![Paraview multiple visualizations]({{ page.root }}/fig/paraview-multiple-visualisations.jpg){: width="55%" }

Each visualization appears in a seperate window frame within Paraview. What
is particularly powerful, is that data from each can also be operated on, or
saved individually to disc for further processing, eg. by a seperate
application such as MatLab or a Python program.


## Sources

Sources in Paraview are sources of data, which can be operated on using
using filters. This can be a file, or any item in the *Sources* menu, such as
text, shapes, point or line sources.

Some filters can combine sources together. This can be particularly useful in
when restructuring data, for example.


## Where to use Paraview

Paraview can be used in many different scenarios. There are covered in 
ACENET's presentation *High Performance Computing and Visualization: An
Overview*, which we will briefly recap here.

Paraview can be used in a variety of scientific, engineering and medical
scenarios.


{% include links.md %}
