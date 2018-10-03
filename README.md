# React & Webpack4 Boilerplate
-based on this article https://medium.freecodecamp.org/part-1-react-app-from-scratch-using-webpack-4-562b1d231e75

## Install Webpack as dev dependency
npm i webpack webpack-cli -D

## Install React and React-Dom
npm i react react-dom -s

## Install Babel and Presets as dev dependency
 npm i babel-loader @babel/core @babel/preset-env @babel/preset-react -D

## Create webpack.config.js in the root folder. Add the babel-loader as loader for js files.

## Create .babelrc and add the presets.
 "presets": ["@babel/preset-env", "@babel/preset-react"]

## Add the folder src/ and add your index.js file
 src/index.js

## Add in to your package.json file so when you run npm start or build, webpack will generate the bundle.

"scripts": {
    "start": "webpack --mode development",
    "build": "webpack --mode production"
}

## At this point you can run npm start to check if webpack works
 npm start

## Create your app component under src/index.js and render something.

const App = () => {
    return <div>Hello there!</div>;
}
ReactDOM.render(<App />, document.getElementById('app'));

## Create your index.html file under src and add the "app" id to check if App component works
 src/index.html

## Add the html-webpack-plugin to create a dist html file (minimized version)
 npm i html-webpack-plugin -D

## Add the webpack-dev-server to create to do realtime changes
 npm i webpack-dev-server -D

## Change the start: webpack --mode development in package.json to
 "start": "webpack-dev-server --mode development"

## At this point you can now access your app component in http://localhost:8080 - default path




