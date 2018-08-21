# Installation guide to use RNRF with Redux 

# How to use

First , Edit your  Package.json required to use for this library which is also compatible with Redux  make sure to use below versions
just copy paste below dependencies in your package.json

# Package.json


```js
{
  "name": "Example",
  "version": "0.0.1",
  "private": true,
  "scripts": {
    "start": "node node_modules/react-native/local-cli/cli.js start",
    "test": "jest"
  },
  "resolutions": {
    "*/@babel/cli": "7.0.0-beta.54",
    "*/@babel/core": "7.0.0-beta.54",
    "*/@babel/code-frame": "7.0.0-beta.54"
  },
  "dependencies": {
    "eslint": "^5.2.0",
    "prop-types": "^15.6.2",
    "react": "16.3.1",
    "react-native": "0.55.4",
    "react-native-router-flux": "^4.0.1",
    "react-navigation": "^2.11.2",
    "react-redux": "^5.0.7",
    "redux": "^4.0.0",
    "redux-logger": "^3.0.6",
    "redux-thunk": "^2.3.0"
  },
  "devDependencies": {
    "babel-jest": "23.4.2",
    "babel-preset-react-native": "4.0.0",
    "jest": "23.5.0",
    "react-test-renderer": "16.4.1"
  },
  "jest": {
    "preset": "react-native"
  }
}

```


first delete your existing node modules folder and hit following command. than run below commands


# Terminal command
```bash

# Install dependencies
npm install --save

# Run it for android
react-native run-android 

# Run it for Ios
react-native run-ios
```



___

* [Example](#try-the-example-app)


Define all your routes in one React component...

```js
const App = () => (
  <Router>
    <Stack key="root">
      <Scene key="login" component={Login} title="Login"/>
      <Scene key="register" component={Register} title="Register"/>
      <Scene key="home" component={Home}/>
    </Stack>
  </Router>
);
```

...and navigate from scene to scene with a simple, powerful API

```js
// Login.js

// navigate to 'home' as defined in your top-level router
Actions.home(PARAMS)

// go back (i.e. pop the current screen off the nav stack)
Actions.pop()

// refresh the current Scene with the specified props
Actions.refresh({param1: 'hello', param2: 'world'})
```

## API

For a full listing of the API, [view the API docs](https://github.com/aksonov/react-native-router-flux/blob/master/docs/API.md).

## Try the [example app](https://github.com/aksonov/react-native-router-flux/tree/master/Example)

![rnrf](https://user-images.githubusercontent.com/3681859/27937441-ef61d932-626b-11e7-885f-1db7dc74b32e.gif)





