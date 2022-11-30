# Sprint 4

Ethan Maness
emaness
Task Tree

### Files you worked on
frontend/src/components/ProjectItem/index.tsx
frontend/src/components/ProjectList/index.tsx
frontend/src/components/TaskItem/index.tsx
frontend/src/pages/projects.tsx
frontend/src/pages/login.tsx
frontend/src/pages/signup.tsx

### What you accomplished
I modified our login and signup pages to render loading indicators when the website is busy communicating with the backend to validate the form submission and fetch user data.  I added form validation to the login page which detects when the fields are empty and notifies the user.  I added form validation to the create project dialog and edit project dialog which detects when the name field is missing, preventing submission and notifying the user.  I added form validation to the create task dialog and edit task dialog which detects when the name field is missing, or the weight field contains a negative or zero value, preventing submission and notifying the user.
