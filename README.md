# Blogs-Posts-Web-Application

Blogs-Posts-Web-Application 

 

Node.js website performing CRUD operations with a Lite SQL database (creating, reading, updating, and deleting data), following technologies used:  

Node.js 

Express.js - Web framework in the Node.js 

Pug (view – just like html) 

Okta’s OIDC-middleware and Node SDK 

Sequelize.js (ORM for working with databases in Node.js) 

To install express-generator run: 

npm install -g express-generator 

To initialize the project: 

express --view pug blog 

cd blog 

npm install 

npm start 

These comands will initialize a new project called blog, move you into the new project folder, install all project dependencies, and start up a web server. 

Go to http://localhost:3000 and you should see your application running 

To get started, create an OpenID Connect application in Okta. :  https://developer.okta.com/signup/  

Leave all the other settings as their default values, then click Done. On the following page, copy down the values for both Client ID and Client secret, you will need these in a moment. 

Next, click the Dashboard tab at the top of the page, then copy the Org URL value from the top-right of the page. 

 

 

Then click the API tab at the top of the page as well as the Create Token button. Enter a name for your token (just give it the same name as your project) then click Create Token. Copy the token value down as you will need it in a moment. 

Name: blog  

Base URIs: http://localhost:3000 

Login redirect URIs: http://localhost:3000/users/callback 

Defining Dependencies:  

npm install express@4.16.3 

npm install @okta/oidc-middleware@0.1.2 

npm install @okta/okta-sdk-nodejs@1.1.0 
npm install sqlite3@4.0.1 

npm install sequelize@4.38.0 
npm install async@2.6.1 
npm install slugify@1.3.0 
npm install express-session@1.15.6 

Finally, create a file that holds environment variables. This application relies on environment variables to specify credentials so that you don't need to hard-code secrets into your application. 

Now that everything is ready, you can start up the app. Please run the following command - npm start 

This will start the webserver on port 3000: 

Now open your browser and go visit http://localhost:3000 to view the website. If you click the Log In on top of the page, log into the blog using. Once you're logged in, you can create posts, edit posts, delete posts(all CRUD operations). 

Enjoy blogging posts ... 

 
