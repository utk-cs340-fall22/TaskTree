# Sprint 2

* Name: Zavier Miller
* NetId: zmille10
* Group Name: TaskTree

### What you planned to do
* Set up formatting [#42](https://github.com/scrumzone/tasktree/issues/42)
* Validate user on authorization [#47](https://github.com/scrumzone/tasktree/issues/47)
* Set up Redux [#81](https://github.com/scrumzone/tasktree/issues/81)
* Authorized and unauthorized layouts [#82](https://github.com/scrumzone/tasktree/issues/82)
* Update README.md to be useful [#84](https://github.com/scrumzone/tasktree/issues/84)
* Create CreateTaskDialog component [#97](https://github.com/scrumzone/tasktree/issues/97)


### What you did not do

### What problems you encountered
The biggest challenge I faced was finding time to complete my tasks. I had a lot going on this week, so hopefully this won't be an issue in the future.

It was also difficult to review and approve last-minute PRs, but as our entire team was busy they likely had the same issue as me. Hopefully this won't prove to be an issue in the future.

### Issues you worked on
* [#42](https://github.com/scrumzone/tasktree/issues/42)
* [#47](https://github.com/scrumzone/tasktree/issues/47)
* [#81](https://github.com/scrumzone/tasktree/issues/81)
* [#82](https://github.com/scrumzone/tasktree/issues/82)
* [#84](https://github.com/scrumzone/tasktree/issues/84)
* [#97](https://github.com/scrumzone/tasktree/issues/97)

### Files you worked on
* backend/TaskTree/Controllers/TaskTreeControllerBase.cs
* backend/TaskTree/Controllers/UsersController.cs
* frontend/.eslintignore
* frontend/.eslintrc.js
* frontend/src/components/CreateTaskFormDialog/index.tsx
* frontend/src/components/TTNavBar/TTNavBarBase.ts
* frontend/src/components/TTNavBar/TTNavBarMobile.tsx
* frontend/src/components/TTNavBar/TTNavBarDesktop.tsx
* frontend/src/store/hooks.ts
* frontend/src/store/index.ts
* frontend/src/store/types.ts
* frontend/src/store/user.ts
* frontend/src/types/Route.ts
* frontend/src/App.tsx
* README.md


### What you accomplished
First, I finished up the formatting PR that rolled over from the last sprint. This didn't end up being the most useful, though, since there are differences to how Windows and Unix handle new lines. I ended up removing the pre-commit hook I built so now there is just formatting on save for the frontend project.
Then, I fixed a security issue where a logged in user could access and modify any data they wanted. I fixed this by adding a method to check for the requested resource's user id and the id of the signed in user.
Next, we needed a way to globally access the currently signed in user from the frontend, so I set up Redux for state management. After that was done, I created a way to show different content in the nav bar and have different accessible routes based on whether or not a user was signed in.
Then, I created the `CreateTaskDialog` component so that we can eventually create a new task in the frontend.
Finally, I updated the README to be useful for new developers to get set up and get the project running.
