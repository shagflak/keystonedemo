#Keystonedemo1

Keystone it's a CMS that runs on top of Node.js using Express for routes, jade for templates and mongoDB

#Prerequisites

* You need to be runing NodeJS > 4.4.3
* NPM (Which it comes bundled with node)
* MongoDB (if you are running windows this can help https://code.msdn.microsoft.com/Mongo-Database-setup-on-6963f46f

#Set up and install the project:

1.- Run:

<pre>npm install</pre>

2.- Once npm finish installation go to <b>keystone.js</b> and change the line <b>23</b>

<pre>
'mongo': 'mongodb://localhost:27017/keystonedemo',
</pre>

3.- You can then run:
<pre>
    node keystone
</pre>

Note: This project was created using the yeoman generator 'yo keystone' and have as default 'gulp'
to build the system although you can also use the npm scripts defined on package.json refer to
gulpfile.js and package.json for commands.

And adjust your mongo host if needed (I am running on windows and this is the default host when
running <mongod --dbpath="C:/db">)

#KeystoneJS File Tree Structure
<pre>
|--lib
|  Custom libraries and other code
|--models
|  Your application's database models
|--public
|  Static files (css, js, images, etc.) that are publicly available
|--routes
|  |--api
|  |  Your application's api controllers
|  |--views
|  |  Your application's view controllers
|  |--index.js
|  |  Initialises your application's routes and views
|  |--middleware.js
|  |  Custom middleware for your routes
|--templates
|  |--includes
|  |  Common .jade includes go in here
|  |--layouts
|  |  Base .jade layouts go in here
|  |--mixins
|  |  Common .jade mixins go in here
|  |--views
|  |  Your application's view templates
|--updates
|  Data population and migration scripts
|--package.json
|  Project configuration for npm
|--web.js
|  Main script that starts your application
</pre>

<a href="http://keystonejs.com/getting-started/">http://keystonejs.com/getting-started/</a>
<a href="http://keystonejs.com/docs/getting-started/">http://keystonejs.com/docs/getting-started/</a>
