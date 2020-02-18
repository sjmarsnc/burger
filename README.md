# Burger 

This app illustrates the use of node, express, mySQL, orm, and handlebars to manage data in a mySQL database and generate pages using templates, and is deployed on heroku.     

See the app at https://damp-fortress-00647.herokuapp.com/ 


## Usage 

The general idea is that the user can enter hamburgers they would like to eat.   Hamburgers are shown in the left-hand column on the page with a button that says "Devour it!". 
Once the user has clicked on the button to "devour" the hamburger, it appears in the "Burgers already eaten" column on the right-hand side.  

## Structure  

The application uses the default directory structure for an express-handlebars application: 

#### Directory structure

All the recommended files and directories from the steps above should look like the following structure:

```
.
├── config
│   ├── connection.js
│   └── orm.js
│ 
├── controllers
│   └── burgers_controller.js - handles the routes for the application 
│
├── db
│   ├── schema.sql
│   └── seeds.sql
│
├── models
│   └── burger.js
│ 
├── node_modules
│ 
├── package.json
│
├── public - files used on the client / browser side  
│   └── assets
│       ├── css
│       │   └── burger_style.css
│       └── img
│           └── burger.png
│   
├── server.js
│
└── views - html fragments used by express-handlebars
    ├── index.handlebars
    └── layouts
        └── main.handlebars