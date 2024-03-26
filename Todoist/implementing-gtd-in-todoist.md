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
  recipes or books I would like to read.

- The `Single Actions` project, which is a project for tasks that are
  self-contained and only require one step.

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
  created more clutter than was necessary. Plus, I'm trying to reduce my reliance
  on my phone for non-communication-based tasks.
- `Anywhere` - For tasks that can be completed anywhere, most likely using my
  phone. This is based on the context that I'm using a cloud-based system, if I
  can access the system, I can access the internet. This is mostly for tasks
  that I could complete using those awkward amounts of time, such as waiting for
  a bus.
- `Calls` - For tasks that require a phone call. Similar to the `Anywhere`
  context, but has been separated out as it's not always possible to make a
  phone call, for example, in busy places.
- `Waiting-For` - For tasks that are waiting for an external factor before they
  can be completed. This is not for tasks that are waiting for me to complete
  another task. Future tasks should simply be given no label.
- `Errands` - For tasks that require me to leave the house, this allows me to
  group errands together, and complete them all at once, to save time.

I was considering adding a `9to5` context, for tasks that can only be completed
during working hours. I found that this was only really applicable to calls, and
errands, which are already covered, so adding this label would just create more
clutter.
