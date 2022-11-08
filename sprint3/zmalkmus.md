
# Sprint 3
* Name: Zack Malkmus
* Id: zmalkmus
* Group name: Tasktree

### What you planned to do
* Add functionality to delete button on project list component (issue #148: https://github.com/scrumzone/tasktree/issues/148)
* Add functionality to edit button on project list component (issue #116: https://github.com/scrumzone/tasktree/issues/116)
* Add Id fields to response objects (issue #115: https://github.com/scrumzone/tasktree/issues/115)
* Add sign up link to login page #57 (issue #57: https://github.com/scrumzone/tasktree/issues/57)

### What you did not do
* I got everything I planned to do completed

### What problems you encountered
This sprint went very well overall. I didn't encounter many problems and I fixed a few bugs/helped others out
with their issues. We did have trouble initially with merging because me and Tyler were both given seperate tasks that
overlapped heavily so I had to change what I was working on.

### Issues you worked on
* (#148): https://github.com/scrumzone/tasktree/issues/148
* (#116): https://github.com/scrumzone/tasktree/issues/116
* (#115): https://github.com/scrumzone/tasktree/issues/115
* (#57): https://github.com/scrumzone/tasktree/issues/57

### Files you worked on
(Give a bulleted list of the files in your github repo that you worked on. Give the full pathname.)
* backend\TaskTree\Models\Responses\TaskResponse.cs
* backend\TaskTree\Models\Responses\ProjectResponse.cs
* frontend\src\types\Task.ts
* frontend\src\types\Project.ts
* frontend\src\components\Login\login.css
* frontend\src\components\Login\LoginDesktop.tsx
* frontend\src\components\Login\LoginMobile.tsx
* frontend\src\components\DisplayProjects\display.css
* frontend\src\components\DisplayProjects\index.tsx
* frontend\src\components\EditProjectDialog\index.tsx
* frontend\src\components\ProjectItem\index.tsx

### What you accomplished
I successfully learned how the backend endpoints linked together and created the destroy, update, read, and create routes for the task-api entity using C#. This took quite a bit longer than expected due to a variety of reasons in the backend, but it all functions properly and works together with the other endpoints. After creating the routes and making requested changes, I tested their functionality using the swagger page and was able to create a tree of tasks within my local version of the database without issue.
