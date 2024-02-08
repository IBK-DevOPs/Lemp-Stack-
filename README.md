# Lemp-Stack-
## Lemp-Stack implementation
### WEB STACK IMPLEMENTATION

### 1.What is Web stack
### 2.	Introduction to web stack
### 3.	Importance of web stack
### 4.	Targeted Audience
### 5.	Prerequisite
### 6.	Goal to be accomplished by the end of web stack implementation

## What is Web stack

###  A web stack is a type of solution stack, which is a collection of software for performing specific tasks. Web stacks are critical components for web applications as well as websites development.

### A web stack, also known as a web application stack, is a compilation of software applications specifically designed for web development. It plays a crucial role in creating web applications and implementing websites.

## Introduction to Web stack

### A web stack is the same but for web development specifically. This is everything needed to implement your website, software as a service product, etc. It can be regarded as tool box needed for web site implementation.

### The top element is the application the user interacts with. The bottom element is the operating system running the application. Then you have all the stuff in between, which acts like interpreters between the two, helping them understand what the other wants.

## Components of a typical web stack: 

### 1.	Operating System
### 2.	Database Application
### 3.	Programming Language
### 4.	Web Server

### 1.	Operating system – this act as an interface between software and hardware components and it provides the essential services and manages resources for the web application.

### 2.	Database Application – This are essential for permanently storing large volume of data required by web project. They allow efficient retrieval and management of information.

### 3.	Programming Language - or Script interpreter operate on the client side and enables the creations of the dynamic’s web applications and websites. It is responsible for processing users request and generate responses.

### 4.Web Server- The web server delivers necessary documents (such as HTML, CSS, and JavaScript files) to clients who request them. It handles incoming requests and serves the appropriate content.


### Importance Of Web stack: 

### 1.	Forms foundation for Web application –
### a. A typical web application comprises of different layers like data base, web server operating system and development environment. 

### b.It also provides foundational platform for building and deploying of web application.

### 2.Front end frame work-Front end development focuses of creating the users interface UI in which user interact with Java script frame work are essential for front-end development. Some notable one includes

### (I)	Vue.js: A progressive JavaScript framework for building user interfaces. It’s user-friendly and scalable.

### (II)	Angular: Developed by Google, Angular is extensible and interfaces seamlessly with other libraries.

### (III)	React: Maintained by Facebook, react is used for UI components and single-page websites.
### 3.Back end frame work- 

### (IV)Back-end frameworks handle server-side logic, data processing, and communication with databases. Some widely used back-end includes

### (V)	Django: A Python-based framework that encourages clean design and rapid development. It covers features like forms, user authentication, caching, and data serialization.

### (VI)	Other popular back-end frameworks exist, each with its own strengths and community support 

### (VII) Full-Stack Development- 

### (VIII) Full-stack developers work on both front-end and back-end components.

### (IX) Understanding full-stack development allows developers to create end-to-end solutions and ensures seamless integration between different layers.

### Clients engaging web development companies should understand the tech stacks used by their developers. This engagement makes informed decision on their projects.

## Targeted Audience

### Web developer
### BtB marketers
### Student
### Project manager
### Designers etc
### Web site builder
### Web site manager

## Prerequisite
### Understanding How the Internet Works

### • Familiarize yourself with the basics of how the internet functions. Learn about the concepts like IP addresses, HTTP requests, and data transmission. For example, when we enter www.google on Url, a lot of steps take place.

### • An internet connection is established via a router or modem.

### • Your system queries your ISP (Internet Service Provider), which connects to servers storing and processing data.

### • The browser indexes the URL and fetches the IP address.

### •HTTP requests are sent to the server, retrieving the website content.

### • The server sends small data packets to your system, which the browser arranges into the visible website content. 

### Understanding Websites and Webpages

### • A website is a collection of interlinked pages accessible via the internet. Each webpage within a website serves a specific purpose. Web site contains information and detail about requested information typed on url while web page can contain text, images, audio, animations and videos

### Web Browsers

### •understanding how to use web browsers is essential. Familiarize ourself with features like bookmarks, tabs, and search functionality. Some Modern browsers allow you to navigate the web, access websites, and interact with web content

### Basic Knowledge of HTML, CSS, and JavaScript.

### • There are 3 languages that are fundamental in web development:

### • HTML (Hypertext Markup Language): Used for structuring web content.

### • CSS (Cascading Style Sheets): Used for styling and layout.

### • JavaScript: Enables interactivity and dynamic behaviour on web pages.

### Computer Science Background-

### • Degree in computer science is important but can be optional in these days technology. Although having a degree in computer science or related fields can provide a solid foundation.

### Goal to be accomplished by the end of web stack implementation.

### Goal to be accomplished by the end of web stack implementation

### • At the end of Lemp stack Projects learner will have experience and full confidence to set up the full Lemp Stack and create a remarkable, high performance web application.

### • Learner can apply basic design principles to present ideas, information, products, and services effectively on web pages.

### • Understand front-end website architecture, Design user interactions on web pages, develop back-end website applications & Create servers and databases for functionality.

### • Learner should be able to Manage a project from conception to the finished and collaborate with graphic designers for web design features.

## STEP 0

#### Log into AWS account (free tier) and create a new EC2 instance of t2 with Ubuntu server.
![alt text](<image/EC2 CONNECTION.png>)
![alt text](<image/Start an instance.png>)

#### Remember to stop or terminate any instance you are with currently.
![alt text](<image/stop instance.png>)not working 


#### Open your git bash terminal

#### On EC2 instance copy your pem. Key and paste it on the terminal.

#### Click enter

#### Link your terminal with your EC2
![alt text](<image/Covert Pem key to .ppk on git bash.png>)

#### `ssh -i <Your-private-key.pem> ubuntu@<EC2-Public-IP-address>`


## STEP 1

### In order to display a web page to our site visitor or viewer, we have to employ Nginx, a high-performance web server. 

#### Installing the Nginx web server by running a command on our terminal.
![alt text](<image/Nginx installation.png>)

### `$ sudo apt update`
![alt text](<image/sudo apt-get update.png>)

### `$ sudo apt install nginx`
![alt text](<image/sudo nano for Nginx.png>)

#### Click enter

#### After hitting enter, you get a quarry if you really want to install on your machine, click YES.
#### To ensure Nginx installed successfully run below code

### `$ sudo systemctl status nginx`
![alt text](<image/To ensure Nginx installed successfully.png>)

#### If its green and returning smoothly, them everything is done correctly.
![alt text](<image/To ensure Nginx installed successfully.png>)

###   Hurray, my first WEB SERVER is lunched!

#### To test that our website is running, we have to run below code on the terminal.

#### $ curl http://localhost:80 by using DNS name
### or
#### $ curl http://127.0.0.1:80  by using IP address
![alt text](<image/public IP on web URL Nginx welcome.png>)

### The output is like Welcome to Nginx and thank you for using Nginx at the end of the return.

STEP 2
## INSTALLATION OF MYSQL

### MYSQL is our database management system to be able to store and manage data for our website
#### Run below code
#### `$ sudo apt install mysql-server` hit enter.
![alt text](<image/sudo apt mysql server.png>)

#### Then log into mysql console with below code.
#### `$ sudo mysql`
#### We will see below information. 
![alt text](<image/sudo apt mysql server.png>)

### Welcome to the MySQL monitor.  Commands end with ; or \g.
### Your MySQL connection id is 11
### Server version: 8.0.22-0ubuntu0.20.04.3 (Ubuntu)

### Copyright (c) 2000, 2020, Oracle and/or its affiliates. All rights reserved.

#### Oracle is a registered trademark of Oracle Corporation and/or its affiliates. Other names may be trademarks of their respective owners.

#### Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

### mysql>
![alt text](<image/Mysql admin user root.png>)

#### Run a security script

#### ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY ……………….
![alt text](<image/connect to mysql using root account.png>)

####  Run interactive scripting with below code.
####  `$ sudo mysql_secure_installation`
#### Validate root password with ………………
![alt text](<image/VALIDATE PASSWORD COMPONENT.png>)

#### It is good to leave validation disable 
#### You can exit mysql by running below code.
#### `mysql> exit`
![alt text](<image/Exit mysql.png>)

### Complete Mysql……

## STEP 3

### Installing PHP
#### We have installed Nginx to serve our content
#### We have installed MYSQL to store and manage our data.
#### We can now install PHP to process code and generate dynamics content for the web server.
#### Run php-fpm on our terminal
![alt text](<image/mysql myphp installation.png>)

#### Then run php-mysql on the terminal as well
![alt text](<image/PHP & MYSQL installation.png>)

### It came with a query ; Do you want to continue? [Y/n] Y Hit Y
### Now we have component installed 


## STEP 4
### CONFIGURATION Nginx to use PHP Processor
#### Create the root web directory with below code.
### `$ sudo mkdir /var/www/projectLEMP`
![alt text](<image/Create the root web directory.png>)

#### Now assign ownership of the directory with the $USER environment, which is my system.
### `$ sudo chown -R $USER:$USER /var/www/projectLEMP` 
	![alt text](<image/assign ownership for $USER.png>)

#### We need to open Nano editor for Nginx 
### `$ sudo nano /etc/nginx/sites-available/projectLEMP
![alt text](<image/sudo nano for Nginx.png>)

#### Activate configuration by linking to the config file from Nginx with below code

### `$ sudo ln -s /etc/nginx/sites-available/projectLEMP /etc/nginx/sites-enabled/`
![alt text](<image/Activate configuration link with Nginx config.png>)

#### For Nginx to use the stored configuration next time its reloaded, we can test our configuration for syntax error.

### $ sudo nginx -t
![alt text](<image/Check Nginx for syntax error.png>)

### #We shall see the following 
### nginx: the configuration file /etc/nginx/nginx.conf syntax is ok
### nginx: configuration file /etc/nginx/nginx.conf test is successful

#### We have to disable default  Nginx host so that it can listen to port 80
#### Run below code
### sudo unlink /etc/nginx/sites-enabled/default
![alt text](<image/Diable Nginx to listen to port 80.png>)

#### We can reload Nginx and apply the changes with below code.

#### `$ sudo systemctl reload nginx`
![alt text](<image/To reload Nginx.png>)

#### Now that our website is created, but its empty we need to create an index.htlm file in that location so that we can test that new web block work as planned.

#### Run below code
### `sudo echo 'Hello LEMP from hostname' $(curl -s http://169.254.169.254/latest/meta-data/public-hostname) *'with public IP' $(curl -s http://169.254.169.254/latest/meta-data/public-ipv4) > /var/www/projectLEMP/index.html`*`

![alt text](<image/nginx new file with php code.png>)

####  We should take it to our URL and use public IP .
####  It return our Hello LEMP from host name
![alt text](<image/Hello LEMP ON URL.png>)

### Our LEMP is now working , we can leave the index.htlm file temporary landing until index.php is created to replace it.


## STAGE 5
### TESTING PHP WITH NGINX
#### Our LEMP STACK is completely setup now
#### Test to ensure that Nginx can correctly handle .PHP
#### Run below code .
### `$ nano /var/www/projectLEMP/info.php`
![alt text](<image/To validate that Nginx can hand .php.png>)

#### Enter valid PHP code inside the blank file.

![alt text](<image/php script code saved.png>)
`<?php`
`phpinfo();`
#### Follow by this code

`http://`server_domain_or_IP`/info.php`  

#### Copy yourPublic IP with PHP code and check on your web

(http://3.17.179.57/info.php)

![alt text](<image/Php URL 2.png>)

#### We can see our php page with all information we have there.

## STEP 6 
### RETREIVING DATA FRO MYQSL DATABASE WITH PHP
#### We will create data base DB with simple to do list.
#### We will configure access to the DB.
#### With this Nginx website will be able to query data from DB and display it.
#### MYSQL PHP library mysqlnd does not support catching _sha2-authentication.
#### So the default authentication method for MYSQL 8 
#### We have to create a new user the mysql_native_password authentication method
#### In order to be able to connect to MYSQL data base from PHP.
#### Now create DATA BASE NAME ` my_database`
![alt text](<image/mysql Data base name.png>)

#### Create USER NAME  my_user
![alt text](<image/mysql test_ USER.png>)

#### CREATE ibk_user

#### Connect to MYSQL console using root account
#### Run below code 

` $Sudo mysql`
![alt text](<image/sudo myqsl.png>)

####  To create new database run below command.
### `mysql> CREATE DATABASE `test_database`;`
![alt text](<image/mysql Data base name.png>)

#### It return with Query OK, 1 row affected (0.000 sec)

### `Then CREATE  USER  test_user`;`        ` mysql> `
![alt text](<image/mysql test_ USER.png>)

#### It returns with Query OK, 0 rows affected (0.004 sec)

#### We need to give the user permission test_database

#### mysql> GRANT ALL ON test_database.* TO 'test_user'@'%';`
![alt text](<image/Give new MYSQL user permission.png>)

#### It will return like this
#### Query OK, 0 rows affected (0.001 sec)
#### The above code will give the test_user  full priviledge on data base and preventing test_user to create or modify other database on your server.

### We can exit  mysql shell  this code  mysql> exit
![alt text](<image/Exit mysql  server.png>)

#### We can test to show that our new user has correct access  to log into console as a customer.
#### Enter below code 
### `$ mysql -u test_user -p`
#### -P is a flag for password to enter test_user page

#### `$ mysql -u `test_user` -p;`
![alt text](<image/mysql test_ USER.png>)

#### This return with password request, input password and click enter.
 #### You will see below message.
 #### (ubuntu@ip-172-31-2-49:~$ mysql -u test_user -p)
#### Enter password:
### Welcome to the MariaDB monitor.  Commands end with ; or \g.
### Your MariaDB connection is is 61
### Server version: 10.6.16-MariaDB-0ubuntu0.22.04.1 Ubuntu 22.04

#### Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

#### Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

#### To confirm our access, we will instruct MYSQL to SHOW DATABASES.
![alt text](<image/SHOW DATABASES.png>)

![alt text](<image/login into sql console with ibk_user.png>)

#### It returns with 
MariaDB [(none)]> SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| example_database   |
| information_schema |
| mysql              |
| performance_schema |
| sys                |
| test_name          |
+--------------------+
6 rows in set (0.000 sec)

#### Then we create a table called to do List with below code.

### CREATE TABLE example_database.todo_list (item_id INT AUTO_INCREMENT,content VARCHAR(255),PRIMARY KEY(item_id));
![alt text](<image/create table example_database.png>)


#### It return with 
#### Query OK, 0 rows affected (0.019 sec)

### Then insert into to do List with this code 
### mysql> INSERT INTO example_database.todo_list (content) VALUES ("My first important item");
![alt text](<image/insert into to do list example_databases.png>)

#### it return with 
### Q`uery OK, 1 row affected (0.003 sec)`

#### To confirm that data was successfully saved on our table  we can run below code
### `mysql>  SELECT * FROM example_database.todo_list;`
![alt text](<image/new user data base, create  to do list table.png>)

#### It returns with output

### `base.todo_list' at line 1`
### M`ariaDB [(none)]> SELECT * FROM example_database.`todo_list;`
+---------+-------------------------+`
| item_id | content                 |
+---------+-------------------------+
|       1 | My first important item |
+---------+-------------------------+
`1 row in set (0.000 sec)`

#### After creating our to do list, we can now log out with mysql exit.

#### We can now create a PHP script connect to MYSQL database and query the content of to do list by running below code.
### `$ nano /var/www/projectLEMP/todo_list.php`
![alt text](<image/php script code saved.png>)

### When its open,save below php script and exit

### `<?php`
### $user = "ibk_user"; 
### $password = "PassWord.1";
### $database = "example_database";
### $table = "todo_list";

try {
  $db = new PDO("mysql:host=localhost;dbname=$database", $user, $password);
  echo "<h2>TODO</h2><ol>";
  foreach($db->query("SELECT content FROM $table") as $row) {
    echo "<li>" . $row['content'] . "</li>";
  }
  echo "</ol>";
} catch (PDOException $e) {
    print "Error!: " . $e->getMessage() . "<br/>";
    die();
} 


#### Then visit your web with public domain by running below code.
`(http://<Public_domain_or_IP>/todo_list.php)`
#### Replace public IP with our IP number on our ec2 server.
3.147.85.198/todo_list.php
![alt text](<image/Php URL 2.png>)

#### We can see our php site with the to  do list.



$user = "ibk_user"; 
$password = "PassWord.1";
$database = "example_database";
$table = "todo_list";

`try {`
  `$db = new PDO("mysql:host=localhost;`dbname=$database", $user, $password);
  echo "<h2>TODO</h2><ol>";
  foreach($db->query("SELECT content FROM $table") as $row) {
    echo "<li>" . $row['content'] . "</li>";
  }
  echo "</ol>";
} catch (PDOException $e) {
    print "Error!: " . $e->getMessage() . "<br/>";
    die();
} 


#### Then visit your web with public domain by running below code.
``(http://<Public_domain_or_IP>/todo_list.php)
### Replace public IP with our IP number on our ec2 server.
`(3.147.85.198/todo_list.php)`
![alt text](<image/public IP todo_ list php..png>)

### We can see our php site with the to  do list on our RRL.
