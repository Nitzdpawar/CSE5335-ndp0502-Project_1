	Project 1- CSE5335
	=================
	
	Name: Nitin D. Pawar		netid: ndp0502		Student id: 1001250502
	===============================================================================
	
	URL: https://cse5335-ndp0502.herokuapp.com/
	-----------------------------------------------------
	
	Project Desc:
	==========================================
	
	Project is basically Portfolio mangement system. it is single page application web page.
	On homepage of my Portfolio website, there is button "My Portfolio" in the header section.
	Click on that button.
	based on no of shares present in your portfolio (in my case 10 objects). the no. of tiles will get created on the site.
	each tile will consist of "Name of the Company" & "Share Price"
	
	If you click on any of the tile the following addtional 3 objects will be dispalyed:
	1. Details: It will consist of additonal data for that particular company.
	2. Charts: it will represnt the Company`s "Revenue/Profit" charts for last five years.
	3. Maps: Is will show the company`s headquater on google maps.
	---------------------------------------------------------------------------------------------------
	

	a.	What server framework did you choose and why?
	=======================================================================
	
	I have used Nodejs server framework. Basically Node is not a Server framework. It is kind of sever which executes JavaScript. 
	Node executes JavaScript at server side. It’s not multi-threaded. It runs in a single thread with callback concept. 
	Node`s model of concurrency is based on events. It runs single threaded event based loop, so all executions become non-blocking. 
	Node is open source, cross platform to make real time network applications.
`	Because of these amazing properties, Node is gaining more popularity and you can scale up the by streaming big files as well.
	To summarize, It is easy to use, understand and popular and its currently trending. 
	That is why I have used Nodejs which will help me to gain knowledge about new technology and help me to get job as well.
	--------------------------------------------------------------------------------------------------------------------------------------

	b.	What client framework did you choose and why?
	==========================================================
	I have used jQuery as client framework. The syntax is simple and jQuery can produce beautiful almost Flash-like animations. 
	The best thing about jQuery is that you don’t need to be a programming genius to wow clients. 
	It makes DOM manipulation painless while creating dynamic html object as well as while binding the data. 
	I used work on jQuery so I was quite familiar with all the concepts of it and it plays well with AJAX which was sort of new to me. The best part is its FREE.
	--------------------------------------------------------------------------------------------------------
	
	c.	What aspect of the implementation did you find easy, if any, and why?
	==================================================================================
	I was working as .NET developer back in India. I was familiar with CSS but never worked on HTML. 
	While working on this project, I found HTML & CSS has the same concept like asp.net & css.
	SO it was easy for me to design the page and manage its stylesheets. 
	I have learned a lot during this project from W3SCHOOL and other websites to understand the dynamic implementation of HTML page using jQuery. 
	It was easy to create dynamic <Div> (attributes) of HTML using jQuery and binding the data to it.
	I have used Google Maps API which was quite easy to implement.
-------------------------------------------------------------------------------------------------------------

	d.	What aspect of the implementation did you find hard, if any, and why?
	=================================================================================
	The hard part during the development was when I deployed my code on “Heroku” is was not all working but it was working on “localhost:5000”.
	I tried changing the initial Index.js to my mpf_node.js(Nodejs File) and made necessary changes to app.JSON and Procfile, but it didn`t work.
	So I replace the code of index.js & index.html with my mpf_node.js & HomePortfolio.html respectively. Now its working fine.
	I have never worked on AJAX, JSON & Nodejs. For me it was bit tough to learn first this things and then implement it. 
	As compared to HTML & CSS, these new technologies took more time for implementation. But it was fun working on this new technologies. 
	During the development phase, I found out JSON is much better alternative than XML to stream the data.
	Surprisingly AJAX call was very sweet, simple and short as compared to Nodejs & JSON.
	There are too many good things about Nodejs , it is fast, robust, concurrent connections, npm (Nodejs Package manager).
	----------------------------------------------------------------------------------------------------------------------------
	
	e.	What components OTHER than your client and server framework did you install,
		if any, and if so, what is their purpose for your solution?
		=================================================================================================================
		I have used Eclipse (Java EE) for development as I was familiar with tool. Other than Eclipse I have install express for Nodejs and npm(Nodejs Package Manger) for Nodejs.
		As I was using Windows PC for development, these package needs be to install unlike Linux systems which has these packages by default.
		While installing and deploying my project using Heroku, it was giving me error that its need Express and npm so I installed it. 
		Then I read about the importance/need of packages and understand that Express is preferred because it adds dead simple routing and support for Connect middleware, 
		allowing many extensions and useful features. It adds a powerful and extensible set of features in a cohesive and well supported whole.
		I have installed Heroku Toolbelt provides me access to the Heroku Command Line Interface (CLI), which can be used for managing and scaling my applications and add-ons.
		A key part of the toolbelt is the Heroku local command, which can help in running my applications locally.
		--------------------------------------------------------------------------------------------------------------------------------------
		
	f.	What Ubuntu commands are required to deploy and run your server?
	=============================================================================================================
		As I mentioned earlier that I was using Windows system, I used windows command prompt to deploy and run my project on Heroku server.
		Please the commads and its purpose below:
		-------------------------------------------------------
		1.	Heroku Login: 
		========================================================================
		After installing Heroku Toolbelt, I have used this command to gain access to create and deploy the application on Heroku.
		--------------------------------------------------------------------------------------------------------------------------------
		
		2.	git clone https://github.com/heroku/node-js-getting-started.git
		cd node-js-getting-started: 
		===========================================================================================
		This will provide us functioning git repository that contains a simple application as well as a package.jsonfile, which is used by Node’s dependency manager.
		-------------------------------------------------------------------------------------------------------------------------------------------------------------------
		
		3.	heroku create :  
		===========================================================================================
		Helps to create an app on Heroku and When you create an app, a git remote (called heroku) is also created and associated with your local git repository.
		Heroku generates a random name for your app, or you         can pass a parameter to specify your own app name.
		-----------------------------------------------------------------------------------------------------------------------------
		
		4.	git push heroku master :
=======================================================
		helps to deploy the app
		-----------------------------------------------------
		
		5.	heroku local web : 
		====================================================================
		It will help the start and run your application locally, It checks your Procfile to determine what to run. You can goto http://localhost:5000 to see your app running.
		----------------------------------------------------------------------------------------------------------------------------------------------------------------------
		
		6.	git add .
		git commit –am “make it better”
		git push heroku master: 
		===========================================================================================
		this commands can be used to add ned udated file, then after committing it you can push the code to deploy it.
		------------------------------------------------------------------------------------------------------------------------------
		
		7.	heroku apps:rename my_new_app_name :  
		==================================================
		I have used this command to rename app name and which effectively changed my url as well.
		------------------------------------------------------------------------------------------------




	

# node-js-getting-started

A barebones Node.js app using [Express 4](http://expressjs.com/).

This application supports the [Getting Started with Node on Heroku](https://devcenter.heroku.com/articles/getting-started-with-nodejs) article - check it out.

## Running Locally

Make sure you have [Node.js](http://nodejs.org/) and the [Heroku Toolbelt](https://toolbelt.heroku.com/) installed.

```sh
$ git clone git@github.com:heroku/node-js-getting-started.git # or clone your own fork
$ cd node-js-getting-started
$ npm install
$ npm start
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

## Deploying to Heroku

```
$ heroku create
$ git push heroku master
$ heroku open
```
or

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

## Documentation

For more information about using Node.js on Heroku, see these Dev Center articles:

- [Getting Started with Node.js on Heroku](https://devcenter.heroku.com/articles/getting-started-with-nodejs)
- [Heroku Node.js Support](https://devcenter.heroku.com/articles/nodejs-support)
- [Node.js on Heroku](https://devcenter.heroku.com/categories/nodejs)
- [Best Practices for Node.js Development](https://devcenter.heroku.com/articles/node-best-practices)
- [Using WebSockets on Heroku with Node.js](https://devcenter.heroku.com/articles/node-websockets)
