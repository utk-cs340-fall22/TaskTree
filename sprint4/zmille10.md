# Sprint 4

* Name: Zavier Miller
* NetId: zmille10
* Group Name: TaskTree

### Files you worked on
- frontend/src/App.tsx
- frontend/src/components/ProjectList/index.tsx
- frontend/src/components/TaskItem/index.tsx
- frontend/src/pages/home.tsx
- frontend/src/pages/landing.tsx
- frontend/src/pages/project.tsx
- frontend/src/pages/signup.tsx
- frontend/src/pages/projects.tsx
- frontend/src/store/index.ts
- frontend/src/store/snackbar.ts
- frontend/src/store/types.ts

### What you accomplished
This sprint was focused on polishing the app, and for my part of this, I added a global service to call a snackbar. This snackbar is used to notify a user of a successful action or an error.
I also went and cleaned up some of the page components, as we had components that acted as the page and the page would just call that component. I simply put the content of these components into the pages themselves.
Next, I fixed an issue where dialog click events would cause their parent elements to be clicked as well.
I also fixed a bug that caused a skeleton loader to always show on the projects and home page if a user had no projects.
Finally, I made it so that the button options on `TaskListItem` and `ProjectListItems` would only appear on hover.
