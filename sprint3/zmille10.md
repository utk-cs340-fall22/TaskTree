# Sprint 3

* Name: Zavier Miller
* NetId: zmille10
* Group Name: TaskTree

### What you planned to do
* Make create project form component [#71](https://github.com/scrumzone/tasktree/issues/71)
* Change JWT fields to camelCase [#124](https://github.com/scrumzone/tasktree/issues/124)
* Populate project page [#125](https://github.com/scrumzone/tasktree/issues/125)
* Add functionality to '+' icon in TaskListItem component [#126](https://github.com/scrumzone/tasktree/issues/126)
* Add edit functionality to TaskFormDialog component [#128](https://github.com/scrumzone/tasktree/issues/128)
* Create ExpandableTaskList component [#143](https://github.com/scrumzone/tasktree/issues/143)
* Create link from project list item to specific project page [#147](https://github.com/scrumzone/tasktree/issues/147)


### What you did not do

### What problems you encountered
There were definitely fewer problems this sprint than in the others. We have figured out how to work on the stories needed by other stories first, and in such a way that there were not a lot of times when people were just waiting around.

It was difficult to get a self-referential component working in React, but I was able to figure this out.

### Issues you worked on
 * [#71](https://github.com/scrumzone/tasktree/issues/71)
 * [#124](https://github.com/scrumzone/tasktree/issues/124)
 * [#125](https://github.com/scrumzone/tasktree/issues/125)
 * [#126](https://github.com/scrumzone/tasktree/issues/126)
 * [#128](https://github.com/scrumzone/tasktree/issues/128)
 * [#143](https://github.com/scrumzone/tasktree/issues/143)
 * [#147](https://github.com/scrumzone/tasktree/issues/147)

### Files you worked on
backend/TaskTree/Controllers/UsersController.cs
frontend/src/components/CreateTaskDialog/index.tsx
frontend/src/components/CreateProjectDialog/index.tsx
frontend/src/components/DisplayProjects/index.tsx
frontend/src/components/EditTaskDialog/index.tsx
frontend/src/components/ExpandableTaskList/index.tsx
frontend/src/components/Project/index.tsx
frontend/src/components/ProjectItem/index.tsx
frontend/src/components/TaskForm/index.tsx
frontend/src/components/TaskItem/index.tsx
frontend/src/router/index.ts
frontend/src/types/Task.ts


### What you accomplished
This sprint was heavy on the frontend, and I was able to get a lot done with it. First, I added a quick fix to the backend to have the data returned in a JWT camelCase as the frontend expected.
Next, I broke out the `CreateTaskFormDialog` component in to a `TaskForm` and `CreateTaskDialog` components; this allowed for the `TaskForm` to be reused in the edit task component I created called `EditTaskDialog`.
After that, I used the same pattern to create the `ProjectForm` and `CreateProjectDialog` components, whose functions are pretty self-explanatory.
Then, I made the `ProjectListItem` component a link to a specific projects page, which involved creating a new route and using router parameters -- something I hadn't done in React before.
Next up, I added functionality to the '+' button in the `ProjectListItem` component, making it show the `CreateProjectDialog` I had created earlier.
Then, I created an `ExpandableTaskList` component that is able to render tasks and sub-tasks from the task tree structure that we have from the backend. This proved to be a little tricky, but in the end, I was able to figure out a pretty clean solution (in my opinion).
Finally, I took the `ExpandableTaskList` component and the `ProjectHeader` component made by Tyler and put them in to the project page, giving us an app with all of our base functionality done!
