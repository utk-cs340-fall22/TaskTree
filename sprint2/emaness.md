
# Sprint 2

Ethan Maness
emaness-utk
TaskTree

### What you planned to do
* [Create route for Project entity in API](https://github.com/scrumzone/tasktree/issues/65) (65)
* [Read route for Project entity in API](https://github.com/scrumzone/tasktree/issues/66) (66)
* [Update route for Project entity in API](https://github.com/scrumzone/tasktree/issues/67) (67)
* [Destroy route for Project entity in API](https://github.com/scrumzone/tasktree/issues/69) (69)
* [List all route for Project entity in API](https://github.com/scrumzone/tasktree/issues/70) (70)

### What you did not do
None--I completed everything I planned to do during this sprint.

### What problems you encountered
* Required some editing of our response objects

### Issues you worked on
* [Create route for Project entity in API](https://github.com/scrumzone/tasktree/issues/65) (65)
* [Read route for Project entity in API](https://github.com/scrumzone/tasktree/issues/66) (66)
* [Update route for Project entity in API](https://github.com/scrumzone/tasktree/issues/67) (67)
* [Destroy route for Project entity in API](https://github.com/scrumzone/tasktree/issues/69) (69)
* [List all route for Project entity in API](https://github.com/scrumzone/tasktree/issues/70) (70)

### Files you worked on
* tasktree/backend/TaskTree/TaskTree.csproj
* tasktree/backend/TaskTree/Controllers/ProjectController.cs
* tasktree/backend/TaskTree/Controllers/TaskTreeControllerBase.cs
* tasktree/backend/TaskTree/Models/MappingProfiles/MappingProfile.cs
* tasktree/backend/TaskTree/Models/Requests/CreateProjectRequest.cs
* tasktree/backend/TaskTree/Models/UpdateProjectRequest.cs
* tasktree/backend/TaskTree/Models/Responses/ProjectResponse.cs
* tasktree/backend/TaskTree/Models/Responses/TaskResponse.cs
* tasktree/backend/TaskTree/Models/Project.cs
* tasktree/backend/TaskTree/Models/TaskTreeContext.cs

### What you accomplished

I created the necessary logic for creating, reading, editing, and destroying Projects in our database via API calls from the frontend including authorizing requests and linking projects with the appropriate user and autogenerating and linking root tasks. This will allow us to begin actually building the meat of the project (i.e. the task tree page and logic).
