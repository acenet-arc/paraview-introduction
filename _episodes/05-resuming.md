---
title: "Loading a session"
teaching: 5
exercises: 5
questions:
- "How do I pick up where I left off?"
objectives:
- Learning how to resume a session
- Moving your session to another machine
keypoints:
- Session states can be loaded in.
- Take your sessions elsewhere, with caution
---

## Resuming a session

Assuming that you were brave/foolhardy enough to **Save State** and quit
Paraview, we will now reload the saved session. After starting Paraview, find
the **Load State** item in the **File** menu - it's just above the
**Save State** item. This will give you the load state dialogue window:
navigate to where the state was saved, and select the state file you want to
load, then clock **Ok**. In this case, the state file is at
**Desktop/acenet-paraview-examples/workforlater.pvsm**.

![load state dialogue window]({{ page.root }}/fig/load-state-dialogue.jpg){: width="65%" }

This will give a second dialogue, named **Load State Options**. We will return
to this later, but we can ignore it for now, as just click on **Ok**.

You should now have the original session, which you saved earlier.

![RenderView1 new colourmap]({{ page.root }}/fig/renderview1-new-colourmap.jpg){: width="85%" }

You can continue using the session as you were before.


## Potential problems

A state file is an precise record of what a Paraview session contained at the
moment it was saved. That means that locations of external data sources, such
as simulation results files, are saved too.

While this sounds convenient, if you are working on one system only, some
concerns that could arise are:

* What happens if you want to use Paraview to look at your data on a
different system?
* How do you do that, when the results files may be in a
different place?

We will deal with those questions below.


## Moving to Paraview on a different system

Let's assume that you are now on a seperate computer, and you have copied
across your data files, and your state file. We are going to start from
scratch and load in your copied session on this new system.

We will start from scratch. Go into the **Edit** menu and select the
**Reset Session** item.

![Edit menu reset session]({{ page.root }}/fig/edit-menu-reset-session.jpg){: width="25%" }

For this lesson, the state file and data file have been copied to
*Desktop/acenet-paraview-examples/somewhere-else/* to simulate the new
computer we are opening our files on. We select the **Load State** item
in the **File** menu, and select *workforlater.pvsm*, then click on **Ok**.

![Load state new computer]({{ page.root }}/fig/load-state-new-pc.jpg){: width="65%" }

{% include links.md %}
