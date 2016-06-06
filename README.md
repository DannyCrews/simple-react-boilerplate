
<h1>Basic Boilerplate to use React</h1>

Install Babel CLI tool and run it in the src directory to produce bundle.js

`npm init -y` to create a package.json 

`npm install --save-dev babel-cli babel-preset-react`

Compile our files
`./node_modules/.bin/babel --presets babel-preset-react src --out-file bundle.js`

Add the following packaage.json script, then we can run it more easily using `npm run <nam>`

```
"scripts": {
  "babel": "babel --presets babel-preset-react src --out-file bundle.js --watch"
},
```

`npm run babel` will build the app

To avoid manual page refreshes install 'live-server'
`npm install --save-dev live-server`
Then add the following as a package.json script"
`"live-server": "live-server --port=3004"`

`npm run live-server` to get the app running locally and being reloaded when files change
