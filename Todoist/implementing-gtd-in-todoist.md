# Implementing GTD In Todoist

Harry Boyd - hboyd255@gmail.com - 20/03/2024

The GTD methodology is a productivity system created by David Allen, and is
described in his book "Getting Things Done". The system is based on the idea
that a person's mind is for having ideas, not for holding them. The GTD system
is platform-agnostic, and can be implemented using any tool that allows for,
there are even multiple ways in which the system can be implemented using
Todoist. This document will describe the system I have created using Todoist.

Full credit to David Allen for the
[GTD methodology](https://gettingthingsdone.com/), and to the
[Todoist](https://todoist.com/) team for creating a platform that allows for
such a system to be implemented.

This document will not describe the why, just the how, for fear of
oversimplifying the GTD methodology. For a full understanding of the GTD system,
I recommend reading "Getting Things Done" by David Allen.

In the official
[GTD Todoist Setup Guide](https://todoist.com/productivity-methods/getting-things-done)
there are two ways in which the GTD system can be implemented. The first methods
is the one recommended by David Allen, due to its simplicity. I however I have
chosen to implement the second method, as it is more aligned with the way I like
to categorize my tasks.

## Definition Clarification

There are several key terms, that have different meanings in GTD than they do in
todoist. This can be confusing, so I will define them here.

In GTD a "Project" is defined as "Any multistep outcome that can be completed
withing one year." , whereas in Todoist a "Project" is more like a folder. The
main difference is that in todoist, a task must be assigned to a project,
whereas in GTD, tasks that are self contained and only require one step, can
exist outside of a project.

## The Structure of method 2

The GTD system I have implemented in Todoist is based on the second method,
outlined on page 20 of the GTD Todoist Setup Guide.

This system appears to be more todoistic, Projects are stored in projects, the
the use of labels feels more natural.

## Use of the Inbox

The inbox is used for capturing tasks, with tasks being processed and moved to
the appropriate project or list as soon as possible.

## Use of Projects

For the most part, Todoist projects are used to represent GTD projects. There
are a few exceptions, such as:

- The "Someday/Maybe" list is a project, as it is a list of projects that are
  not currently active, but I want to revisit in the future.

- The "Lists" project and its sub-projects. This is to store lists, such as
  recipes or books I want to read.

- The "GTD Weekly Review" project, which is a list of tasks that need to be
  completed during the weekly review. This kind of is a project, but i've chosen
  to separate it from the other projects, due to it's importance to this system.

## Use of Labels

Like the outlined system, I use labels to represent context and actionability.

If a task is immediately actionable, and thus has a `next action`, it will be
given a context label. If it cannot be completed, aside from specific
`Waiting-For` tasks, it is simply not given a label.

### Context Labels:

- `Home` - For tasks that can only be completed at home.
- `Computer` For tasks that can only be completed on a computer, previously this
  was split into `Computer` and `has_internet`, But I found that this just
  created more clutter than was necessary, plus I'm trying to reduce my reliance
  on my phone for not communication based tasks.
- `Anywhere` - For tasks that can be completed anywhere, most likely using my
  phone. This is based on the context that I'm using a cloud based system, if I
  can access the system, I can access the internet. This is mostly for tasks
  that I could complete using those awkward amounts of time, such as waiting for
  a bus.
- `Calls` - For tasks that require a phone call. Similar to the `Anywhere`
  context, but has been separated out as I find that its not always possible to
  make a phone call, for example if I'm in a busy place.
- `Waiting-For` - For tasks that are waiting for an external factor before they
  can be completed. This is not for task that are waiting for me to complete
  another task. "Future tasks" should simply be given no label.
- `Errands` - For tasks that require me to leave the house, this allows me to
  group errands together, and complete them all at once, to save time.

I was considering adding a `9to5` context, for tasks that can only be completed
during working hours, but I found that this was only really applicable to calls,
and errands, which are already covered amd adding this label
would just create more clutter.
