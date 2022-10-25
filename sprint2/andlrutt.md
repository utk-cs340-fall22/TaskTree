# Sprint 2

* Name: Andrew Rutter
* NetId: andlrutt
* Group Name: TaskTree

### What you planned to do
* Create a sign up page [#41](https://github.com/scrumzone/tasktree/issues/41)
* Consume the create user api from the signup page [#76](https://github.com/scrumzone/tasktree/issues/76)
* Add auth headers to the swagger page [#77](https://github.com/scrumzone/tasktree/issues/77)
* Consume create project api from create project page [#78](https://github.com/scrumzone/tasktree/issues/78)
* Consume get projects api from the display projects page [#79](https://github.com/scrumzone/tasktree/issues/79)
* Consume get project api from the display project page [#80](https://github.com/scrumzone/tasktree/issues/80)

### What you did not do
* Consume get project api from create project page (set up code for it but could not call from create project page)
* Consume get project api from display project page (set up code for it but could not call from display project page)

### What problems you encountered
* By and large the biggest issue was issue dependencies. There were significant delays that arose because of issues that were
dependent on other issues, so developers had to wait on other developers at times. During planning for sprint 3, we paid special attention
to dependencies to make sure that if there are any dependent issues, they are also assigned to the same developer who will work on the issue
that is depended on.

### Issues you worked on
* [#41](https://github.com/scrumzone/tasktree/issues/41)
* [#76](https://github.com/scrumzone/tasktree/issues/76)
* [#77](https://github.com/scrumzone/tasktree/issues/77)
* [#78](https://github.com/scrumzone/tasktree/issues/78)
* [#79](https://github.com/scrumzone/tasktree/issues/79)
* [#80](https://github.com/scrumzone/tasktree/issues/80)

### Files you worked on
* backend/TaskTree/Controllers/UsersController.cs
* backend/TaskTree/Program.cs
* backend/TaskTree/Models/Requests/CreateUserRequest.cs
* frontend/.env.development
* frontend/src/components/SignUp/index.tsx
* frontend/src/types/User.ts
* backend/TaskTree/Controllers/UsersController.cs
* frontend/src/components/SignUp/index.tsx
* frontend/src/services/UserService.ts
* frontend/src/components/DisplayProjects/index.tsx
* frontend/src/pages/home.tsx
* frontend/src/services/ProjectService.ts
* frontend/src/services/UserService.ts
* frontend/src/types/Project.ts
* frontend/src/types/Task.ts
* backend/TaskTree/TaskTree.csproj
* package-lock.json
* .husky/pre-commit
* package.json

### What you accomplished
* Created a signup page that creates and authenticates a user in the database the following validation checks pass. Otherwise,
  displays the rule that is violated to the user. The validation checks are:
  * database is running
  * unique username
  * required fields are present (first name, username, password)
  * password is 8+ characters
  * password and confirm password match
* Addded an authorization option on the swagger page. This allows us to call/test backend api routes from our swagger page 
  without having to interact with the frontend. Once authorized, swagger automatically passes in the Bearer token when calling
  any route that requires authorization.
* Consuming project apis:
  * GET Project endpoint -- used to display all information for a single project -- not used in frontend yet
  * GET Projects endpoint -- used to display all of a user's projects -- used in the Projects page
  * POST Project endpoint -- used to create a new project -- used in the Projects page
  * PUT Project endpoint -- used to update a project -- not used in frontend yet
  * DELETE Project endpoint -- used to delete a project -- not used in frontend yet
