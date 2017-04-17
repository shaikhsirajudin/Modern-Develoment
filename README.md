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
	For all your node touching needs. 
	```
	C:\path>npm install touch
	```
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
						
	
	
	
	
	
	
	
	
	
	
	
	
