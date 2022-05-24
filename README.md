# SomewhatSecureWebAPP
secure application development - assignment 002

# Welcome fellow 3rr0rs
This is the documentation guide to successfully startup and run this simple and ready web application.


# Startup
First of all you need to install the appropriate [XAMPP](https://www.apachefriends.org/download.html) control pannel according to your OS.
After running XAMPP click on the *Start* button infront of MYSQL and APACHE.

With both APACHE and MySQL up and running the next step is to click the *Admin* button infront of MySQL to add a new database.
                                        


# Database

The following query is used to create the database from the MySQL console:

```
CREATE DATABASE LoginSystem;
```

alternatively you can use the UI.

Next open the SQL console of the new database and add the following query:

```

CREATE TABLE IF NOT EXISTS `users` ( 
 `id` int(11) NOT NULL AUTO_INCREMENT, 
 `adminauthenticator` boolean NOT NULL,
 `username` varchar(50) NOT NULL, 
 `email` varchar(50) NOT NULL, 
 `password` varchar(50) NOT NULL, 
 `create_datetime` datetime NOT NULL, 
 PRIMARY KEY (`id`)
);

```
Now the database is ready.



# Web Server

Next step is to got the C:\xampp\htdocs and delete the Dashboard directory completely, then add the directory provided in this page.

Lastly click on the *Admin* button infront of APACHE to launch the web application.


# Usage

To switch a registered user from a normal user to an administrator, simply login to the PHPmyAdmin and change the Boolean value from 0 to 1.


Thats all for now, Good Luck !!
