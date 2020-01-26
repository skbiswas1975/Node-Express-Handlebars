# Node Express Handlebars

This app is all about eating burgers, yes, that's right! You'll create a burger logger with MySQL, Node, Express, Handlebars and a homemade ORM (yum!). Be sure to follow the MVC design pattern; use Node and MySQL to query and route data in your app, and Handlebars to generate your HTML.
* Eat-Da-Burger! is a restaurant app that lets users input the names of burgers they'd like to eat.
```

* Whenever a user submits a burger's name, your app will display the burger on the
 left side of the page -- waiting to be devoured.

* Each burger in the waiting area also has a `Devour it!` button. When the user
 clicks it, the burger will move to the right side of the page.

* Your app will store every burger in a database, whether devoured or not.



#### Directory structure

All the recommended files and directories from the steps above should look like the following structure:

```
Eat-Da-Burger
│
├── config
│   ├── connection.js
│   └── orm.js
│ 
├── controllers
│   └── burgers_controller.js
│
├── db
│   ├── schema.sql
│   └── seeds.sql
│
├── models
│   └── burger.js
│ 
├── node_modules
│ 
├── package.json
│ 
├──.env
│
├── public
│   ├── assets
│   │	├── css
│   │   │   └── burger_style.css
│   │   ├── img
│   │   │   └── burger.png
│   │   └── js
│   │   	 └── burgers.js
│   │
│   └── test.html
│
├── server.js
│
└── views
    ├── index.handlebars
    │
    ├── layouts
    │   └── main.handlebars
    │
    └── partials
    	└── burgers
		└── burgers.js
```

## Instructions on setting up and running this app on your computer

#### App Setup

1. Clone Github repo to your computer.

1. Got to your Git Bash and got to into the folder called Eat-Da-Burger.

1. To get all the npm packages required to run this app type into the command line `npm install`

1. Create a server.js file.


#### Database Setup

1. On your computer, open MySQL Workbench and login to a local server you have set up. 

__One option for executing the database code required to run the app is:__

1. Open a new SQL tab for executing queries.

1. Then go back to your chosen text editor (I suggest either Visual Studio or Sublime Text) and open your `Eat-Da-Burger` folder.

1. Inside the `Eat-Da-Burger` folder you will find a folder named `db`.

1. In the `db` folder, open the file named `schema.sql`. Copy the code in the file and paste it to the new SQL tab you opened in MySQL Workbench.

1. Go back to the `db` folder in you text editor and open the `seeds.sql` file and copy the code and paste it into the open tab in MySQL Workbench and execute the code.


__The other option for running the MySQL code is to:__


1. Run the `schema.sql` and `seeds.sql` files into the mysql server from the command line

1. Now you're going to run these SQL files.

1. Make sure you're in the `db` folder of your app.

1. Start MySQL command line tool and login: `mysql -u root -p`.

1. With the `mysql>` command line tool running, enter the command `source schema.sql`. This will run your schema file and all of the queries in it -- in other words, you'll be creating your database.

1. Now insert the entries you defined in `seeds.sql` by running the file: `source seeds.sql`.

1. Close out of the MySQL command line tool: `exit`.



#### Open App in Browser

1. In the command line go into main folder of `Eat-Da-Burger`

1. Type `node server.js` end hit enter

