# fullstack-devloper-react-sample-001
this project only for setup the react workspace 
===================================================
1) create a project in github
2) clone the project repo to  code edditor
3) open visual studio and install material icon theme
4) npm init -y   // use this command initialized the react project. it create pacakge.json file 
5) npm install next react react-dom  // use this command to download the related library 
6) change the script in pacakge.json file to following script 
	"scripts": {
	"dev": "next dev",
	"build": "next build",
	"start": "next start",
	"lint": "next lint"
	}
7) create some following new folder & file  within the project  by terminal
   mkdir pages
		 pages / _app.js
		 pages / index.js
		 
	mkdir public
		  public / style.css
		  public / image
		  /* this is basically for store the public resources file 
		  
	mkdir components  // to store the page components . here some default components are 
	mkdir components / navbar
	mkdir components / footer
	mkdir components / auth 
	
8) write the following code in  _app.js  using the  direct command = rafce

	import React from 'react'
	import  '../public/style.css'
	const App = ({Component ,pageProps}) => {
		return (
        <>
			<Component {...pageProps} />
        </>
		)
	}
	export default App
	
9) write the following code in index.js
	import React from 'react'
	const index = () => {
    return (
        <div>
            <h1>This is my default workspace project</h1>
        </div>
		)
	}
	export default index
	
10) npm run dev  // this command run for display the page in browser

11) add a .gitignore file and add following script to ignore some file and folder to track by git 
/node_modules/
/.next/
/next.config.js/
 ============= end ==============