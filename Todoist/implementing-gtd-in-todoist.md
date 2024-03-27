# Implementing GTD In Todoist

Harry Boyd - hboyd255@gmail.com - 20/03/2024

The GTD methodology is a productivity system created by David Allen, and is
described in his book
[Getting Things Done](https://www.amazon.co.uk/Getting-Things-Done-Stress-Free-Productivity/dp/B01B6WSGGA).
The system is based on the idea that a person's mind is for having ideas, not
for holding them.

The GTD system is platform-agnostic, and can be implemented using any tool that
allows for it. I have chosen to implement this system in Todoist, and this
document will describe how I have done so.

Full credit to David Allen for the
[GTD methodology](https://gettingthingsdone.com/), and to the
[Todoist](https://todoist.com/) team for creating a platform that allows for
such a system to be implemented.

This document will not describe the why, just the how, as I do not want to risk
oversimplifying the GTD methodology. For a full understanding of the GTD system,
I recommend reading Allen's book.

In the official
[GTD Todoist Setup Guide](https://todoist.com/productivity-methods/getting-things-done),
there are two ways in which the GTD system can be implemented. The first method
is the one recommended by David Allen, due to its simplicity. I, however, have
decided to implement the second method, as it is more aligned with the way I
like to categorize my tasks.

## Definition of a Project

The term "Project" is used differently in GTD than it is in Todoist. In GTD, a
"Project" is defined as "Any multistep outcome that can be completed within one
year." whereas in Todoist, a Project is more like a folder. The main difference
is that in Todoist, a task must be assigned to a project, whereas in GTD, tasks
that are self-contained and only require one step, can exist outside a project.
To overcome this, any single-action task, can be assigned to the
`Single Actions` project.

## The Structure of method 2

The GTD system I have implemented in Todoist is based on the second method,
outlined on page 20 of the GTD Todoist Setup Guide. I've made a few changes to
the system, to better fit my needs.

## Use of the Inbox

The inbox is used for capturing tasks, with tasks being processed and moved to
the appropriate project or list as soon as possible.

## Use of Projects

For the most part, Todoist projects are used to represent GTD projects. There
are a few exceptions, such as:

- The `Someday/Maybe` list is a project, as it is a list of projects that are
  not currently active, but I want to revisit in the future.

- The `Lists` project and its subprojects. This is to store lists, such as
  recipes or books I would like to read. Items in lists should not be actionable
  tasks, and thus, should not be completable, this can be achieved by adding an
  asterisk to the start of the task's title.

- The `Things to Buy` List, is a list of things I need to buy. The things on the
  list may not need to be purchased immediately, especially when budgeting is
  factored in. As part of the weekly review, I will review this list, and
  consider adding items to the `Single Actions` project, as an `Errand` task.

- The `Single Actions` project, which is a project for tasks that are
  self-contained and only require one step.

- The `Quick Reads` project. This is a list of articles or blog posts that will
  typically take less than 10 minutes to read. To populate this list, I will, in
  part, use the "Email tasks to this project" feature. This is separate from the
  `Lists` project, as these are actionable tasks, but is secluded from other
  lists, due to the informality of this list. The reason for this informality,
  is because I'm prioritizing ease of access, by bypassing the inbox system. All
  items in this list should be treated as having the `Anywhere` context. This
  list should be reviewed during the weekly review, and tasks should be moved to
  the `Single Actions` project, if they have been hanging around for too long.
  This list is a prototype, and if it becomes too cluttered, I will scrap it and
  go back to the traditional method of adding articles to the inbox, then
  processing them.

- The `GTD Weekly Review` project, which is a list of tasks that need to be
  completed during the weekly review. This kind of is a project, but I've chosen
  to separate it from the other projects, due to its importance to this system.

## Use of Labels

Labels are used to represent context and actionability.

If a task is immediately actionable, and thus has a `next action`, it will be
given a context label. If it cannot be completed, aside from specific
`Waiting-For` tasks, it is simply not given a label.

### Context Labels:

- `Home` - For tasks that can only be completed at home.
- `Computer` For tasks that can only be completed on a computer. Previously,
  this was split into `Computer` and `has_internet`, But I found that this just
  created more clutter than was necessary. Plus, I'm trying to reduce my
  reliance on my phone for non-communication-based tasks.
- `Anywhere` - For tasks that can be completed anywhere, most likely using my
  phone. This is based on the context that I'm using a cloud-based system, if I
  can access the system, I can access the internet. This is mostly for tasks
  that I could complete using those awkward amounts of time, such as waiting for
  a bus.
- `Phone` - For tasks that require my phone. Similar to the `Anywhere` context,
  but has been separated out as it's not always possible to make a phone call,
  for example, in busy places. It's also the case that my phone is often
  switched off, so I would rather not be reminded of these tasks when I can't
  complete them.
- `Waiting-For` - For tasks that are waiting for an external factor before they
  can be completed. This is not for tasks that are waiting for me to complete
  another task. Future tasks should simply be given no label.
- `Errands` - For tasks that require me to leave the house, this allows me to
  group errands together, and complete them all at once, to save time.

I was considering adding a `9to5` context, for tasks that can only be completed
during working hours. I found that this was only really applicable to calls and
errands, which are already covered, so adding this label would just create more
clutter.

## Agendas

I'm still on the fence about how to implement the `Agendas` section, There are
two ways I could do this:

### Agendas as Labels

In the Guide, for method 2, it suggests creating a single label titled
`Agendas`, This would then be used to store tasks that need to be discussed with
others. This, however, does not do anything to separate the tasks by person. I
could address this by creating a label for each person, for example,
`Agendas_Will`, but this would clutter up the labels section.

### Agendas as Projects

Alternatively, I could store a project titled `Agendas`, and then create a
subproject for each person I need to discuss tasks with. This would allow me to
separate the tasks by person. The downside to this is that it pulls the task out
of the main project. This could lead to tasks being forgotten about, but it
shouldn't be an issue if the weekly review is done correctly.

For now, I'm going to go store Agendas as labels, but if it becomes too
cluttered, I will switch to projects.
