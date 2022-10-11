# Sprint 1
Tyler Nitzsche, PotassiumLover, The Scrum Zone

### What you planned to do
(Give a short bulleted list of the items you planned to do for this sprint. Include the github issue number and link to the issue)
-Store JWT tokens in cookies [#7](https://github.com/scrumzone/tasktree/issues/7)
-Create a logout button and put it on the home page [#15](https://github.com/scrumzone/tasktree/issues/15)
-Add the user name to the home page [#14](https://github.com/scrumzone/tasktree/issues/14)

### What you did not do
(Give a short bulleted list of the items that you planned to do, but did not accomplish)
-Add the user name to the home page, ended up getting accidentally done by Zavier

### What problems you encountered
(List the problems you encountered)
I have no experience whatsoever with web development, JWT tokens, cookies, whatever. I was totally in the dark for everything I needed to do with the exception of me having taken 1 semester of javascript like 6 years ago, so just learning everything was an ordeal. I'm also not very github saavy so working on a project in github was something I had to learn.

### Issues you worked on
(List the specific github issues that you worked on with a link to the issue (ex: [#1](https://github.com/utk-cs340-fall22/ClassInfo/issues/1) Sample Issue)
-Store JWT tokens in cookies [#7](https://github.com/scrumzone/tasktree/issues/7)
-Create a logout button and put it on the home page [#15](https://github.com/scrumzone/tasktree/issues/15)
-Get a cookie with the user info in it [#60](https://github.com/scrumzone/tasktree/issues/60)

### Files you worked on
(Give a bulleted list of the files in your github repo that you worked on. Give the full pathname.)
-frontend/src/services/authService.ts
-frontend/src/pages/home.tsx
-frontend/package-lock.json
-frontend/package.json

### What you accomplished
(Give a description of the features you added or tasks you accomplished. Provide some detail here. This section will be a little longer than the bulleted lists above)
-A way to store the user's info once they have been authenticated using JWT tokens and cookies
-A way to clear a user's cookies making it so they are no longer authenticated
-A log out button on the home page, which will call the method which clears cookies on a click
-A way to retrieve a user's information from the cookie