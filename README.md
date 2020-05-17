# Development Setup

## Prerquisites

* [Git](https://git-scm.com/)
* [Node.JS](https://nodejs.org/en/) x64, version `>= 12.x` 

To install dependencies and run it locally:

``` 
npm install 

npm start
```

Now you should have development mode running on http://localhost:3000

We have ESLint enabled on this project. You can install ESLint extension in VS Code [`dbaeumer.vscode-eslint`](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) and enable it such that on save it takes care of all spacing and other good things (there is workspace (`.vscode`) with this repo so it should take care of that as it has settings all set for that, you just need to install ESLint). You can learn more about ESLint [here](https://eslint.org).



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