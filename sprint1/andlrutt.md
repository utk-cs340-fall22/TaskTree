# Sprint 1

* Name: Andrew Rutter
* NetId: andlrutt
* Group Name: TaskTree
 
### What you planned to do
(Give a short bulleted list of the items you planned to do for this sprint. Include the github issue number and link to the issue)
* Establish a basic frontend project [Issue #6](https://github.com/scrumzone/tasktree/issues/6)
* Set up routing for the page [Issue #16](https://github.com/scrumzone/tasktree/issues/16)
* Create an API to authenticate a user [Issue #8](https://github.com/scrumzone/tasktree/issues/8)
* Create a sign up page [Issue #41](https://github.com/scrumzone/tasktree/issues/41)

### What you did not do
* Create a sign up page [Issue #41](https://github.com/scrumzone/tasktree/issues/41)

### What problems you encountered
There was a lot of depencencies early on. Since a lot of the issues in this sprint were setting up core functionality of the website, there
was a lotof issues that were dependent on other issues. This made it difficult for everyone to get started at once.

### Issues you worked on
(List the specific github issues that you worked on with a link to the issue
* [#6](https://github.com/scrumzone/tasktree/issues/6)
* [#16](https://github.com/scrumzone/tasktree/issues/16)
* [#8](https://github.com/scrumzone/tasktree/issues/8)

### Files you worked on
* frontend/src/App.css
* frontend/src/App.tsx
* backend/TaskTree/Controllers/UsersController.cs
* backend/TaskTree/Models/AppConfig.cs
* backend/TaskTree/Models/Requests/AuthenticateUserRequest.cs
* backend/TaskTree/Program.cs
* backend/TaskTree/appsettings.Development.json

### What you accomplished
I established the basic frontend project that could be run with `npm start`. I then set up routing for that page so that a user can navigate between all of our different pages.
In the backend, I established an API route to authenticate a user. It takes a username and password in the body, and then does a lookup in our database to see if it
can find a match. If it does, it returns a JWT to the frontend. Also configured was an [Authorize] decorator which configures any endpoint with it to take a JWT as a
header to authorize the action.
It's not under my name, but I also made the `docs/intro-to-apis.md` documentation to make sure that all of our team members are up to speed on how apis work
and how to play around with them.
