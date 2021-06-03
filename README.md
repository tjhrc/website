# website
 
Source for TJHRC's website built with Sanity and React.

# Setup
When setting this project up for the first time, first download Node.js if you haven't already from here: https://nodejs.org/en/download/, and install yarn:

```
npm install -g yarn
```

Then clone the project and run:
```
cd website
npm install
yarn install
```

# Running
After you've set up the project for the first time, simply run:
```
yarn start
```
And you should see the website load and show up in your browser, at the address https://http://localhost:3000/. 

# Creating new branches
Make sure to replace 
```
"start": "serve -s build/"
```
 with these four lines:     
```
"start": "react-scripts start",
"build": "react-scripts build",
"test": "react-scripts test",
"eject": "react-scripts eject"
``` 
when creating a branch. This in the scripts section of package.json

# Committing to master
Run ```yarn run build``` in the console

Also replace 
```
"start": "react-scripts start",
"build": "react-scripts build",
"test": "react-scripts test",
"eject": "react-scripts eject"
``` 
with 
```
"start": "serve -s build/"
``` 
This is in the scripts section of package.json

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

# Troubleshooting

If you are developing the project, make sure to replace

```
"start": "serve -s build/"
```
 with these four lines:     
```
"start": "react-scripts start",
"build": "react-scripts build",
"test": "react-scripts test",
"eject": "react-scripts eject"
``` 
This is the only way to open up localhost and have it reload with your changes.
