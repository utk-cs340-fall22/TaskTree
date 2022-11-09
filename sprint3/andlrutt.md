# Sprint 3

* Name: Andrew Rutter
* NetId: andlrutt
* Group Name: TaskTree


### What you planned to do
* Add functionality to task list item edit icon [#118](https://github.com/scrumzone/tasktree/issues/118)
* Add functionality to task list item check icon [#119](https://github.com/scrumzone/tasktree/issues/119)
* Add functionality to task list item delete icon [#120](https://github.com/scrumzone/tasktree/issues/120)
* Add separate view for a completed task [#121](https://github.com/scrumzone/tasktree/issues/121)
* Improve home page [#122](https://github.com/scrumzone/tasktree/issues/122)

### What you did not do
I did everything I set out to accomplish

### What problems you encountered
In the first half of the first week of the sprint, I was blocked by other issues and could not progress. 
This was temporary, though, and as soon as that blocker was lifted there were no issues.

### Issues you worked on
* [#118](https://github.com/scrumzone/tasktree/issues/118)
* [#119](https://github.com/scrumzone/tasktree/issues/119)
* [#120](https://github.com/scrumzone/tasktree/issues/120)
* [#121](https://github.com/scrumzone/tasktree/issues/121)
* [#122](https://github.com/scrumzone/tasktree/issues/122)

### Files you worked on
* frontend/src/types/Project.ts
* frontend/src/types/Task.ts
* backend/TaskTree/Models/Responses/TaskResponse.cs
* frontend/src/components/TaskItem/index.tsx
* frontend/src/services/TaskService.ts
* frontend/src/index.tsx
* backend/TaskTree/Models/Responses/ProjectResponse.cs
* frontend/src/components/DisplayProjects/index.tsx
* frontend/src/components/ProjectItem/index.tsx
* frontend/src/components/ProjectList/index.tsx
* frontend/src/pages/home.tsx


### What you accomplished
(Give a description of the features you added or tasks you accomplished. Provide some detail here. This section will be a little longer than the bulleted lists above)
This sprint, I almost exclusively worked on frontend components. I added functionality to the delete, check, and edit icons on a task so that they execute the appropriate action.
I also updated a task to have a different, distinct view if it is complete. 
This involes a grayed out, strikethroughed task with a green progress bar and checksymbol to indicate that it has been completed.
For the edit icon, I had to configure an Edit Task dialog with a form inside of it that is displayed when the edit icon is clicked.

The last change I made was to the home page. Previously, it was just a placeholder page that had no real content on it. I made it into a mini-dashboard
that displays a greeting message, the number of active and inactive projects, and the 5 most recently worked-on projects.

