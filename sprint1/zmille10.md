# Sprint 1

Zavier Miller, zaviermiller, ScrumZone

### What you planned to do
- Set up MySQL database
- Set up Docker for development
- Create 'user' table
- API CRUD routes for User
- Set up MaterialUI framework for React
- Create NavBar component
- Consume backend API from frontend React project

### What you did not do
- Set up formatting

### What problems you encountered
- Docker was a pain for Windows users, some just ended up installing MySQL and other required programs directly
- The MySQL database was a bit tough to get working
- Working with MaterialUI and React is a lot different from my frontend experience (Vue and Vuetify)
- Getting relations to work with our Dotnet ORM was a bit difficult

### Issues you worked on
(List the specific github issues that you worked on with a link to the issue (ex: [#1](https://github.com/utk-cs340-fall22/ClassInfo/issues/1) Sample Issue)
[#1](https://github.com/scrumzone/tasktree/issues/1)
[#4](https://github.com/scrumzone/tasktree/issues/4)
[#5](https://github.com/scrumzone/tasktree/issues/5)
[#27](https://github.com/scrumzone/tasktree/issues/27)
[#29](https://github.com/scrumzone/tasktree/issues/29)
[#35](https://github.com/scrumzone/tasktree/issues/35)
[#36](https://github.com/scrumzone/tasktree/issues/36)
[#54](https://github.com/scrumzone/tasktree/issues/54)

### Files you worked on
- `docker-compose.yml`
- `backend/TaskTree/Dockerfile`
- `backend/TaskTree/Program.cs`
- `backend/TaskTree/Controllers/UsersController.cs`
- `backend/TaskTree/Models/BaseEntity.cs`
- `backend/TaskTree/Models/Project.cs`
- `backend/TaskTree/Models/Task.cs`
- `backend/TaskTree/Models/TaskTreeContext.cs`
- `backend/TaskTree/Models/User.cs`
- `backend/TaskTree/Models/MappingProfiles/MappingProfile.cs`
- `backend/TaskTree/Models/Requests/CreateUserRequest.cs`
- `backend/TaskTree/Models/Requests/UpdateUserRequest.cs`
- `backend/TaskTree/Models/Responses/UserResponse.cs`
- `db/init/init.sql`
- `docs/backend-structure.md`
- `frontend/.env.development`
- `frontend/.env.production`
- `frontend/src/components/TTNavBar/TTNavBarBase.ts`
- `frontend/src/components/TTNavBar/TTNavBarDesktop.tsx`
- `frontend/src/components/TTNavBar/TTNavBarMobile.tsx`
- `frontend/src/components/TTNavBar/index.ts`
- `frontend/src/pages/home.tsx`
- `frontend/src/services/UserService.ts`
- `frontend/src/types/User.ts`
- `frontend/src/util/http.ts`

### What you accomplished
(Give a description of the features you added or tasks you accomplished. Provide some detail here. This section will be a little longer than the bulleted lists above) 
This sprint has been focused on getting the project set up and creating basic use-case examples to figure out how we want to structure and build the project. 
The first thing I did was set up a docker compose project to run all our services with a single command (backend, frontend and the db).
Next, I set up the database connection for the backend API and set up the Entity Framework ORM so we wouldn't have to interact with raw SQL.
Once that was working, I moved on to creating the first entity with the ORM, the User. This was pretty simple and after defining a BaseEntity with information all rows should have like `Id, CreatedAt, UpdatedAt` I was able to define the User in `backend/Models/User.cs` and create a migration for it.
Now we needed a way to use HTTP requests to interact with the backend, so I set up the `UsersController` with basic CRUD routes. At this point, I realized we would need special objects for the request and response so I added those in at this time as well.
After that was done, I switched over to the frontend to get the UI framework set up to make styling the app easier. We went with MaterialUI as it seems to be the most popular React UI framework.
Then, I wanted to define a component structure that would allow the app to have a mobile and desktop version, so I set up the `TTNavBar` component with a structure I learned from work that defines a mobile and desktop component and switches between them based on the viewport size.
Finally, we needed a way to actually call the backend API from the frontend app, so I created a `UserService` that abstracts away the HTTP request and let's us only worry about getting the data instead of how we get the data.


