# User Authentication with Node JS app & save data in PostgreSQL

- It is a simple authentication system where a user will register using his name, email addrees and password.
- His credentials will be saved in PostgreSQL and password will be saved in hashed form.
- Later he may log in using his email and password.

## Setting up the application in your device

1. Install Node.js in your device.
2. Install PostgreSQL in your device.
3. Set up PostgreSQL initially.
4. Then create a user with an access to create a database.
5. Create a database and a table with these column names: id, name, email & password.
6. Create an npm project with this command line: *npm init -y*

## Required libraries and command lines to install them:
We will need to serve the application, connect database with our app, hash user passwords, store session details, display flash messages to the user, authenticate them and implement a local authentication for the application. For all these purposes the libraries below are needed. To install these run the commands below in the VSCode terminal of your project directory:

- *npm i express*
- *npm i -D nodemon*
- *npm i ejs*
- *npm i dotenv pg*
- *npm i bcrypt*
- *npm i express-session express-flash*
- *npm i passport passport-local*

## Check database for user info
You can check the user info stored in your database except the password as it is hashed. To check the user info in db, first log in as the user created at the beginning of the project after installing and setting up Postgres initially. Then use the command *\C Your_Database_name*. In this case the name of the database is "nodelogin". Then use this command line: *SELECT * FROM users;* to see all the user information in your table.

## Run the App
To run the app, in the terminal you need to type in the command: *npm run dev* and the application will start running at port 3000.

