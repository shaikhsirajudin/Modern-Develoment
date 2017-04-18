##Required software NodeJS and NPM [NodeJS Environment Setup](https://www.tutorialspoint.com/nodejs/nodejs_environment_setup.htm)
==================================================================
## Instructions to create react package from scratch
1. Navigate to folder */1-basic-react*
2. *npm install*
3. *npm run dev*
4. Navigate to localhost:8080

## Instructions to install create-react-app globally and create application from it.

1. Navigate to some folder */1-basic-react*
2. *Install create-react-app
 	> npm install -g create-react-app
3. *Once the installation complete re
peat following step when you create new applications
  	> create-react-app my-app
        
	> cd my-app
        
	> npm start

## Setting Up Your React Dev Environment manually.

1. Install Global Packages
	````
	C:\path>npm install -g babel
	C:\path>npm install -g babel-cli
	````
2. Create Root Folder */1-basic-react*

	Follow the instruction	
	```
	 C:\path\1-basic-react>npm init
	```

3. Add Dependencies and plugins

	 webpack bundler
	```
	C:\path\1-basic-react>npm install webpack --save
	```
	webpack dev server
	
	```
	C:\path\1-basic-react>npm install webpack-dev-server --save
	```
	Since we want to use React
	
	 ```
	 C:\path\1-basic-react>npm install react --save
	 C:\path\1-basic-react>npm install react-dom --save
	 ````
	 Add some babel plugins
	 
	 ```
	 C:\path\1-basic-react>npm install babel-core
	 C:\path\1-basic-react>npm install babel-loader
	 C:\path\1-basic-react>npm install babel-preset-react
	 C:\path\1-basic-react>npm install babel-preset-es2015
	 
	 ````
	 Or All together you can use following command with space as a separator
	 
	 ```
	 C:\path\1-basic-react>npm install --save-dev react react-dom webpack webpack-dev-server babel-loader babel-core babel-preset-es2015 babel-preset-react 
	 
	 ```
4. Create some files
	```
	C:\path\1-basic-react>type nul > index.html
	C:\path\1-basic-react>type nul >App.jsx
	C:\path\1-basic-react>type nul >main.js
	C:\path\1-basic-react>type nul >webpack.config.js
	```
	
	
5. Edit the  webpack.config.js and add following contents
 
 webpack.config.js
```
var path = require('path');
var config = {
   entry: './main.js',
	
   output: {
      path:path.resolve(__dirname, './'),
      filename: 'index.js',
   },
	
   devServer: {
      inline: true,
      port: 8181
   },
	
   module: {
      loaders: [
         {
            test: /\.jsx?$/,
            exclude: /node_modules/,
            loader: 'babel-loader',
				
            query: {
               presets: ['es2015', 'react']
            }
         }
      ]
   }
}

module.exports = config;
```
Add the following in package.json in place of test

	```
 	"start": "webpack-dev-server --hot"
	
 	```
6. Run the application 

	```
	C:\path\1-basic-react>npm start
	```
7. Commonly used Redux middleware components.

	=> Formatted layout for logging.
	
	. redux-logger
	
	=> Redux Thunk middleware allows you to write action creators that return a function instead of an action
	. redux-thunk
	
	=> Ajax call for restful API
	
	. axios
	
	=>Default dispatch implementation for restful api
	
	. redux-promise-middleware
	
	syntanx for applying
	```
	//const middleware = applyMiddleware(thunk, createLogger())
	const middleware = applyMiddleware(promise(),thunk, logger)
	// take out the constant.
	const store = createStore(reducer, middleware);
	```

	
	
	
	
	
	
	
	
	
	
