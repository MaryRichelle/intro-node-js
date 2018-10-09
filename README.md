# Intro to Nodejs
> Scott Moss & Frontend Masters
- [Resources](#resources)
- [Course](#course)
- [Excercises](#excercises)
  - [Installing Node](#installing-node)
  - [Modules (node vs browser)](#modules-node-vs-browser)
  - [CLI (npm)](#cli-npm)
  - [API (async code)](#api-async-code)
  - [Debugging & Testing](#debugging--testing)
  - [Sharing and Deploying](#sharing-and-deploying)

## Resources
* [Slides](https://slides.com/scotups/deck/fullscreen)
* [Nodejs](https://nodejs.org/en/)
* [NVM](https://github.com/creationix/nvm)

## Course
This course has two parts, slides and excercises. The slides describe the excerices in detail. Each excercise has a folder
## Excercises
### Installing Node
Install node with [node version manager (NVM)](https://github.com/creationix/nvm). NVM was created by the community and not the Nodejs foundation. However, it is the recommended approach. After installing nvm, use nvm to install the lates version of Nodejs, which at the time is `10` and set it to the default version
```bash
nvm install node # node is an alias for the latest version
nvm alias default node
```
If this fails, or you want to install nodejs from nodejs source, [then go here](https://nodejs.org/en/)
### Modules (node vs browser)
* location - `exercises/modules`
* commands
  * test - `npx jest`

This exercise will have you convert some JavaScript written for the browser, so that it works with node.
- [ ] check out to start branch
- [ ] check the README on how to run test (will talk later about that command)
- [ ] fix and convert the 3 js files in the exercises/modules/browser to Nodejs JavaScript and place them in exercises/modules/node
- [ ] ensure all tests pass by running test command again
### CLI (npm)
* location - `exercises/cli`
* commands
  * new - `node exercises/cli/index.js new`
  * list - `node exercises/cli/index.js list`

You'll be creating a CLI program that saves and retrieves contacts from and address book. The program is partially there, however, you must install some remote modules, and use the fileSystem to get some things to work.

- [ ] install all remote modules (hint: use npm)
- [ ] Check the README on how to run your CLI
- [ ] Fix the CLI so that the "new" command works by saving contacts to contacts.json
- [ ] Fix the CLI so that the "list" command works by listing all contacts and allowing you to select one, the prints out the selected contact
### API (async code)
* location - `exercises/api`
* commands
  * start the server - `node exercises/api/server.js`

You'll be refacoring and fixing a simple static asset server. The server uses blocking sync code and crashes whenever a request comes in that is asking for an asset that is not found. Neither of those are desirable. You'll also have to teach the server how to server the assets it has in the `assets` folder.

- [ ] install all remote modules (hint: use npm)
- [ ] Check the README on how to run your CLI
- [ ] refactor the sync file reading code to be async with a callback, promise, or async await
- [ ] prevent the server from crashing when an assets is not found. Instead, respond with a 404 status code
- [ ] create some sort of router logic to handle incoming requests for assets

### Debugging & Testing
### Sharing and Deploying


