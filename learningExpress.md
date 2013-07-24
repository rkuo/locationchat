# Learning Express 

## References:
[Getting started with Express js ](http://indoallcode.com/getting-started-with-express-js)

[Node-upandrunning](http://shop.oreilly.com/product/0636920015956.do)

## Install
- check npm installation `npm -version`
- check node installation `node -v`
- verify express installation `npm info express version`, if it not installed, run `npm install -g express` for global installation.

## Project Development
- create an app directory
- check express version `npm info express version`
- define dependencies in package.json, i.e. <pre><code>{
  "name": "getting-started",
  "description": "first application using express",
  "version": "0.0.1",
  "private": true,
  "dependencies": {
    "express": "3.x"
  }
} </code></pre> This step may not be necessary. It gets write over later.
- initially, we only have package.json in app directory
<code><pre>% ls                                                                                             
package.json
 % express --sessions --css stylus --ejs                                                     
destination is not empty, continue? yes
   create : .
   create : ./package.json
   create : ./app.js
   create : ./public
   create : ./public/javascripts
   create : ./public/images
   create : ./public/stylesheets
   create : ./public/stylesheets/style.styl
   create : ./routes
   create : ./routes/index.js
   create : ./routes/user.js
   create : ./views
   create : ./views/index.ejs

   install dependencies:
     $ cd . && npm install

   run the app:
     $ node app</code></pre>
- At this point, the directory structure:
<pre><code>% tree
.
├── app.js
├── package.json
├── public
│   ├── images
│   ├── javascripts
│   └── stylesheets
│       └── style.styl
├── routes
│   ├── index.js
│   └── user.js
└── views
    └── index.ejs

6 directories, 6 files</code></pre>

- modify package.json to meet the application needs`vim package.json` <pre><code>vim package.json 
{
  "name": "getting-started",
  "version": "0.0.1",
  "private": true,
  "scripts": {
    "start": "node app"
  },
  "dependencies": {
    "express": "3.0.3",
    "ejs": "*",
    "stylus": "*"
  }
}</code></pre>
- then download the dependencies `npm install`. This will add stylus and express modules to project. 
- We can run `node app.js` to verify the project setup.
- enter "localhost:3000" in browser.

### drectory structure

Express is MVC framework for Node.js

- public directory holds all (html, css, and images)
- routes directory provide control/dispatch function
- the user will choose one of template engine during the application creation `express --sessions --css stylus --ejs` Options are EJS, Hmal, Jade, CoffeeKup, or jQuery.  
- app.js defines the required modules, sets environment varibles, rountining per url, and activates server. app.js decides which routes, i.e. "/" to index.js, then index.js to index.ejs in view.  

### Use Bootstrap
- download Bootstrap, unzip it, and put css, js, img directories under public directory. 
- remove images, javascripts and styles directories.
- add bootstrap.min.css, bootstrap-responsive.css and viewport links in index.ejs, then the app should behavior as a normal Bootstrap app. 
