---
title: "Introducing filters"
teaching: 20
exercises: 10
questions:
- "How do I filter data?"
- "How do I chain filters together?"
objectives:
- Attaching a filter to an opened file
- Chaining filters together
- Changing the order of filters
keypoints:
- "No matter how much he cries, no matter how much he begs, never, never feed
him after midnight."
- "Don't cross the streams."
- "An Englishman, an Irishman, and a Scotsman walk into a bar. This is the
start of a joke with cultural stereotypes."
---

## Overview of filters

A filter is a processing unit that takes data from a data source or other
files, and produces output. Filters can be chained together, typically
with the last in the chain shown. Filters can be branched off too, so one
data source can have multiple filters independently operating on its data.

There are a great many filters available. Paraview categorises them in the
**Filters** menu so you can find what you want easier.

![Filters menu]({{ page.root }}/fig/filters-menu.jpg){: width="25%" }

We will mostly dealing with those in the **Common** submenu.

## Adding the first filter

We will start from where we left off in the previous lesson. Here, we are
going to apply a filter to see is happening to the gas inside the chamber.
We are going to do this by applying the **Clip** filter.

First, click on **disk_out_ref.ex2** in the **Pipeline browser** and then
go into the **Common** submenu in the filters, select the **Clip** filter.

![Clip filter in submenu]({{ page.root }}/fig/submenu-clip-filter.jpg){: width="75%" }

You should now see a render view similar to this.

![Clip filter initial view]({{ page.root }}/fig/clip-filter-initial.jpg){: width="85%" }

Note that in the **Pipeline browser**, *disk_out_ref.ex2* has a greyed-out
eye icon next to it, and *Clip1* - our clip filter - has a solid black
eye icon. This is to indicate that the view of *disk_out_ref.ex2* is hidden
from view. If you show wish to see it again, you can click the faded icon
to show it - however, this will obscure the *Clip1* view.

Next, we will rotate the view so we can see the fluid velocity within the
chamber. You can do this in one of two ways:

1. Rotate the view with **Left mouse click and drag** as shown previously, or
2. Hit the **-X** rotation button in the toolbar.

![Negative X-axis rotate]({{ page.root }}/fig/toolbar-minus-x-rotate.jpg){: width="35%" }

Your view should now look similar to this.

![Chamber internal view]({{ page.root }}/fig/chamber-interal-view.jpg){: width="85%" }

You can see that fluid speeds up and moves around the sides of the piston,
which is what we would expect as it moves up and down. By looking at this
picture, the physics of the situation can be clearly understood by a
non-expert. This shows one of the many strengths of visualisation.


But what is happening to the pressure? How would we show that? Can we show
that alongside the velocity?


## Multiple filters and multiple views

Here we are going to do two things:
1. Create a second filter
2. Create a second render view to show the results of that filter

{% include links.md %}
