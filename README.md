# Development Setup
This is a create-react-app template that has some add-ons I like to use with my projects. Comes with workflows that you can use to deploy a site on GH-Pages. 

## Prerequisites

* [Git](https://git-scm.com/)
* [Node.JS](https://nodejs.org/en/) x64, version `>= 12.x` 

To install dependencies and run it locally:

``` 
npm install 

npm start
```

Now you should have development mode running on http://localhost:3000


## ESLint is enabled on this project

## Github Actions Workflow
* `continuous-integration`: 
  * Uses ESLint to do linting tasks
  * It will run on PR's and pushes on all branches.
  * If your commit contains "skip lint" then it will not run the action
* `deploy`:
  * To enable this you will need to move it into `workflows` from `disabled-workflows`.
  * It will run react build script and deploy the project to gh-pages
  * It runs only on pushes to master branch. (This is setup assuming that you have dev and master branches and master is used as a production branch)
  * NOTE: You will need to modify few things to make sure your deploy works:
    * `committer_name: YOUR_GITHUB_NAME`
    * `commiter_email: YOUR_GITHUB_EMAIL`
  * You will need to add a [Github Token](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line) in Secrets of your repo. Name it `deploy_access_token`

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

### `npm test`
No tests currently

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

### `npm run lint`

This should lint the project and will display and warnings and errors if they exist. 

## Helpful Resources

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

To modify GH-Page deploy action check out and modify accordingly [`ghaction-github-pages`](https://github.com/crazy-max/ghaction-github-pages)

## Credits

Eslint configurations and npm scripts are inspired from [@ShabadOS/desktop](https://github.com/ShabadOS/desktop)
