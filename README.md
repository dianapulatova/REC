# REC
Reverse Engineering Code






  ![GitHub license](https://img.shields.io/badge/license-Creative%20Commons%20Zero%20v1.0%20Universal-blue.svg)

  ## Description
 Reverse engineer the starter code provided and create a tutorial for the code.
 
Develop
A software development folder or file is a physical or virtual container for software project artifacts, including: requirements, plans, designs, source code, test plans and results, problem reports, reviews, notes, and other artifacts of the development process.

Config -
Config stands for configuration where all the configuration files would go: 
In computing, configuration files (commonly known simply as config files) are files used to configure the parameters and initial settings for some computer programs. They are used for user applications, server processes and operating system settings.

Middleware - are functions that have access to the request object, the response object and the next object. So they are in the middle of the request-response cycle
Config.json - is a configuration file
Passport.js - is a middleware application for authenticating users in Node.


Models -
Model folder is to create models(table) for the app where you can store data.

Index.js - is a file which gathers all models file, it is a kind of a boilerplate you add whenever you create models in your app.
User.js - file is where you store user information whatever user add on the app. (in our app its storing our email and password - and storing the password in an encrypted mode)

User.addHook("beforeCreate", function(user) {
   user.password = bcrypt.hashSync(user.password, bcrypt.genSaltSync(10), null);
 });
 return User;
};

For example, addHook - is used to perform before or after a specified database operation. Hooks plays a major role in keeping your codebase DRY and easy to reason about For example: Hashing the user password before saving it to the database.


Node_modules -
The node_modules directory is only for build tools, where NPM would make copies of external packages/libraries that Node would import as you need to use the files.

Public - 
In this case the public folder is storing the js folder and the css folder. 
Js - Javascript folders
	Login.js - it is used to get user inputs and if the form is submitted it validates email and password entered. When loginUser  does a post to api/login route and if successful, redirects the user to the members page.
Members.js - this file is to GET request to figure out which user is logged in and updates the HTML page.
Signup.js - it allows user to signup if not already then it redirects them to signup page. 
Stylesheets - CSS folder
	Style.css - Reasons to Use CSS External Style Sheet File for HTML Programming. Cascading Style Sheet (CSS) is a style sheet language that manages the website's visual representation. Commonly used with markup languages like HTML, CSS allows you to style each HTML element and give your overall site a more appealing look.

HTML -
 HTML is a HyperText Markup Language file format used as the basis of a web page. ... The HTML tags can be used to define headings, paragraphs, lists, links, quotes, and interactive forms.

Login.html - creates the following look for the Passport Authentication page

Members.html - welcomes the member and shows member name.
Signup.html - sign up form page


Routes -
 Routing refers to how an application’s endpoints (URIs) respond to client requests

Api-routes.js - in this app api-routes.js uses the passport.authentication middleware with local strategy and if the user has the valid login credentials sends them to the member page otherwise error page. And it stores users credentials securely with Sequelize User Model. So it provides route for signing up a user, logging out the user, and some data about the user to be used client side. 
Html-routes.js - it provides a path to html files, first checks if the user is logged in and if user has an account send them to the members page or redirects to login page. 

Package-lock.json -
package-lock.json: records the exact version of each installed package which allows you to re-install them. Future installs will be able to build an identical dependency tree.
Package.json -
package.json: records the minimum version you app needs. If you update the versions of a particular package, the change is not going to be reflected here.

Server.js-
 server.js makes the app available to serve HTTP requests. It provides the interaction between users and the  application. 

.gitignore
 gitignore file is a plain text file where each line contains a pattern for files/directories to ignore. Generally, this is placed in the root folder of the repository.

LICENSE
It permits users to do anything with a given project as long as they credit the developer and don't hold him or her liable for the project's use. The Apache License, which is similar to the MIT License, but also explicitly grants patent rights to users.

README.md 
README (as the name suggests: “read me”) is the first file one should read when starting a new project. It's a set of useful information about a project and a kind of manual. 



References:

https://en.wikipedia.org/wiki/Configuration_file#:~:text=In%20computing%2C%20configuration%20files%20(commonly,processes%20and%20operating%20system%20settings.

https://stackoverflow.com/questions/45052520/do-i-need-both-package-lock-json-and-package-json/56683169#56683169









 


  ## Table of Contents

  * [Installation](#installation)

  * [Usage](#usage)

  * [License](#license)
 
  * [Contributing](#contributing)
   
  * [Tests](#tests)

  * [Questions](#questions)
   
 
  ### Installation

  To install, run the following command:

  ```
  $ git clone <git url>
  ```

  ### Usage
  Walk-through of the codebase
  
  
  ### License
  Creative Commons Zero v1.0 Universal


  ### Contributing
  Clone it, fork it but don't push any changes to master.
  
  ### Tests
     
      
      `  

        node server`
      
      

        
  ### Questions
   
  
  If you have any questions about the repo, feel free to contact me through gitHub [dianapulatova](https://github.com/dianapulatova)
  or directly at <dianapulatovaa@gmail.com>


