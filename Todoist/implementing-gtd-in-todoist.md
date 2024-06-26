# Implementing GTD In Todoist

Harry Boyd - hboyd255@gmail.com - 20/03/2024

The GTD methodology is a productivity system created by David Allen, and is
described in his book
[Getting Things Done](https://www.amazon.co.uk/Getting-Things-Done-Stress-Free-Productivity/dp/B01B6WSGGA).
The system is based on the idea that a person's mind is designed for having
ideas, not holding them.

The GTD system is platform-agnostic, and can be implemented using any tool that
allows for it. I have chosen to implement this system in Todoist, and this
document will describe how I have done so.

Full credit goes to David Allen for the
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

For the most part, Todoist projects are used to represent GTD projects. A few
Todoist projects are used to represent separate concepts, such as the following:

- `Single Actions` - A project for tasks that are self-contained and only
  require one step.

- `Lists` - A collection of lists, stored as subprojects, such as recipes or
  books I would like to read. Items in lists should not be actionable tasks, and
  thus, should not be completable, this can be achieved by adding an asterisk to
  the start of the task's title.

- `Someday/Maybe` - A list of projects that are not currently active, but I want
  to revisit in the future.

- `Quick Reads` - This is a list of articles or blog posts that will typically
  take less than 10 minutes to read. To populate this list, I will, in part, use
  the "Email tasks to this project" feature. This list is different from the
  other lists, as its items are actionable tasks, and thus should be
  completable. All items in this list should be treated as having the `Anywhere`
  context. This list should be reviewed during the weekly review, and tasks
  should be moved to the `Single Actions` project if they have been hanging
  around for too long. This list is a prototype, and if it becomes too
  cluttered, I will scrap it and go back to the traditional method of adding
  articles to the inbox, then processing them.

- `Incubator` - A list of projects that are not currently active, but have been
  scheduled to be revisited at a later date. This is the same concept as the
  tickler file. This is separate from the `Someday/Maybe` list, as these tasks
  have been scheduled for reevaluation.

- `Waiting-For, External` - A list of tasks that I am waiting for someone else
  to complete. Each task in this list should have a "Waiting Since" comment, in
  the description, to track how long I have been waiting for a task to be
  completed.

- `Waiting-For, Internal` - The Waiting-For, Internal list should be used
  sparingly. It is for projects, that cannot be started until another project
  has been completed. It is not for single actions that are waiting for another
  task of the same project to be completed, as these can just be left
  unlabelled, and will be addressed during the weekly review. Every item in this
  list should have a clear definition of what exiting projects need to be
  completed before this project can be started.

## Projects of interest

- `GTD Weekly Review` - A list of tasks that need to be completed during the
  weekly review. This kind of is a project, but I've chosen to separate it from
  the other projects, due to its importance to the system.

- `Things to Buy` - A list of things I want to buy. The things on the list may
  not require purchasing immediately, especially when budgeting is factored in.
  As part of the weekly review, I will review this list, and consider adding
  items to the `Single Actions` project, as an `Errand` task.

## Use of Labels

Labels are used to represent context. If a task is immediately actionable, and
thus has a `next action`, it will be given a context label. If it cannot be
completed, it is simply not given a label.

### Context Labels:

- `Home` - For tasks that can only be completed at home.

- `Computer` - For tasks that can only be completed on a computer. Previously,
  this was split into `Computer` and `has_internet`. However, I found that this
  just created more clutter. Plus, I'm trying to reduce my reliance on my phone
  for non-communication-based tasks.

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

- `Errands` - For tasks that require me to leave the house. This allows me to
  group errands together, and complete them all at once, to save time.

- `Brainstorm` - For tasks that require a lot of thought, and maybe a whiteboard
  or a piece of paper. This is separate from the other contexts, as it requires
  a different state of mind. It's good to review this list before going on a
  walk, to give me things to think about.

### Agenda Labels

Agendas refer to tasks that need to be discussed with others, preferably in
person. To facilitate this, I have created multiple agenda labels, one for each
person that I have tasks to discuss with. These labels can be created and
deleted as needed.

The format of these labels are `Agenda_<First initial>.<Surname>`. For example,
tasks that I need to discuss with my good friend William Betteridge, would be
assigned the label `Agenda_W.Betteridge`.
