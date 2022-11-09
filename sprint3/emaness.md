
# Sprint 3

Ethan Maness
emaness-utk
TaskTree

### What you planned to do
* [Update DELETE task endpoint behavior](https://github.com/scrumzone/tasktree/issues/122) (122)
* [Update PUT Task endpoint](https://github.com/scrumzone/tasktree/issues/123) (123)
* [Update PUT Task to propagate progress upwards](https://github.com/scrumzone/tasktree/issues/127) (127)
* [Bound Task.Progress to 0.0 - 100.0](https://github.com/scrumzone/tasktree/issues/151) (151)
* [Set Task.CompletedAt to current time whenever Progress is set to 100](https://github.com/scrumzone/tasktree/issues/153) (156)

### What you did not do
I completed all of my designated work during this sprint. However, issue 122 ended up being unnecessary as the database structure already performed this functionality automatically. On the other hand, issue 127 turned out to be a much, much larger undertaking than expected, having to be rewritten 3 times and also done for our POST and DELETE Task endpoints.  It also ended up swallowing issue 156.  I am very happy with how it turned out in the end though.

### What problems you encountered
Given the strict visibility heirarchy of our database structure, it was hard to get the tree update code to work as each layer above and below the affected task had to be manually specified in the database request, otherwise the server would not have access to that information.  This means that currently our code isn't infinitely scalable (we have a finite limit on the number of tree layers). It is possible to fix this, but it will require a significant refactoring of multiple parts of the project.  If performance is also an issue we plan on doing it.

### Issues you worked on
* [Update DELETE task endpoint behavior](https://github.com/scrumzone/tasktree/issues/122) (122)
* [Update PUT Task endpoint](https://github.com/scrumzone/tasktree/issues/123) (123)
* [Update PUT Task to propagate progress upwards](https://github.com/scrumzone/tasktree/issues/127) (127)
* [Bound Task.Progress to 0.0 - 100.0](https://github.com/scrumzone/tasktree/issues/151) (151)
* [Set Task.CompletedAt to current time whenever Progress is set to 100](https://github.com/scrumzone/tasktree/issues/153) (156)

### Files you worked on
* tasktree/backend/TaskTree/Controllers/ProjectsController.cs
* tasktree/backend/TaskTree/Controllers/TasksController.cs
* tasktree/backend/TaskTree/Models/MappingProfiles/MappingProfile.cs
* tasktree/backend/TaskTree/Models/Task.cs

### What you accomplished

I created all of the logic for task-task and task-project interaction so that the entire project tree will update in real time to account for changes made at any level, including changes to composite progress and task completion date and time.  This means that now our Task Tree is a recursive tree structure, rather than independent non-interacting nodes, so our progress tracking app can finally track progress.
