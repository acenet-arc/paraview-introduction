---
title: "Saving your work"
teaching: 5
exercises: 5
questions:
- "How do I save my work?"
objectives:
- Saving your progress
keypoints:
- Paraview can save its entire state for later
---

## Saving your work

At this point, we have made a scene with a degree of complexity, that would
take a considerable amount of time to recreate. Fortunately, Paraview has
a way of preserving this for later - you could say, its saving grace - so
that we can quit Paraview, do something else, and pick up where we left off
later.

Paraview keeps a record of everything it has done in a session, so it records
its **State**. We are going to use the **Save State** feature to save the
state to disk.

You need to find the **File** menu and click on the **Save State** item. On
Windows or Linux, this will be at the top of the application window, whereas
on MacOS this will be at the top of the screen in the application menu:

![File menu with save state selected]({{ page.root }}/fig/file-menu-save-state.jpg){: width="45%" }

Paraview will show the save state dialogue. Here, the state file
*workforlater.pvsm* will be saved to *Desktop/acenet-paraview-examples/*, but
you can save the state file anywhere you like.

![Save state dialogue window]({{ page.root }}/fig/save-state-dialogue.jpg){: width="65%" }

Unless you get an error message, your Paraview state should now be saved.
If you're feeling brave, you can now close Paraview.

(*Suggested break: 15-20 minutes*)

{% include links.md %}
