# User-Authentication-system-
The Project suggest a complete system for user registration, login, logout, and accessing a secure dashboard area.
Here are the general steps to get your project running on your computer:

Step 1: Set up a Local Server Environment
You need a web server (like Apache) and a database (like MySQL) to run this project. The easiest way to get both is to install a software package like XAMPP or WAMP.

Download and install XAMPP from apachefriends.org.

Once installed, open the XAMPP Control Panel and start the Apache and MySQL services.

Step 2: Place Your Project Files
The web server needs to know where your project files are located.

Navigate to the XAMPP installation folder (usually C:\xampp).

Find the htdocs directory within the XAMPP folder.

Place your user_auth project folder (the one containing the PHP files) inside the htdocs directory.

Step 3: Set up the Database
Your project uses a database to store user information. You need to create this database and import the provided SQL file.

Open your web browser and go to http://localhost/phpmyadmin. This is the database management tool that comes with XAMPP.

In the left-hand menu, click on New to create a new database.

Name the database user_auth (this is the name used in your user_auth.sql file) and click Create.

With the user_auth database selected, go to the Import tab at the top.

Click Choose file and select the user_auth.sql file from your project folder (C:\xampp\htdocs\user_auth\user_auth.sql).

Scroll to the bottom and click Go to import the file.

Step 4: Configure the Database Connection
Your db.php file needs to have the correct settings to connect to the database.

Open the db.php file in a code editor.

Check the database connection details. For a standard XAMPP setup, the details are usually:

Servername: localhost

Username: root

Password: (leave blank)

Database Name: user_auth

If the file already has these details, you do not need to change anything.

Step 5: Test the Project
With the server running, files in place, and the database set up, you can now test the project.

Open your web browser.

Go to http://localhost/user_auth/register.php to access the registration page and create a new user.

Go to http://localhost/user_auth/login.php to log in with the new user you created.
