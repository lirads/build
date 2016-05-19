# Lirads Build
#### QuickStart Guide
If you're used to using Lirads Build and just want to install it on your server, simply run this line of code on any Ubuntu server (ideally 14.04):
```
sudo wget https://raw.githubusercontent.com/lirads/build/master/script?v=1 && sudo chmod +x script && sudo ./script
```
This will setup your Ubuntu server with all of the tools you need to begin rapid development.

#### What is Lirads?
Lirads (or _Lightweight Rapid Development System_) is a series of tools to make rapid prototyping of products simple. The entire Lirads ecosystem is built with plugin support to allow developers to modify it to fit their needs.

#### What is Build?
Lirads Build is a component of the Lirads ecosystem which allows deveolpers to setup an entire Ubuntu server for web development by simply running a single line of code. It is designed to work on all Ubuntu servers, but works best on a Ubuntu 14.04 droplet running on DigitalOcean.

#### What does it do?
Lirads can do anything you want via a number of different Lirads plugins. However, by default, all it does is setup your Ubuntu server for web development by taking the following steps:

1. Updating your OS
    - Your OS is updated via `apt-get update` and `apt-get upgrade`
2. Installing Apache
    - Apache is installed via `apt-get install apache2`
    - RewriteEngine is enabled via `a2enmod rewrite`
    - `.htaccess` files are enabled by modifying `000-default.conf`
3. Installing PHP
    - PHP is installed via `apt-get install php5`
4. Installing MySQL
    - MySQL is installed via `apt-get install mysql-server`
    - PHPMyAdmin is installed via `apt-get install phpmyadmin`
5. Configuring Development Environment
    - default `.htaccess` file created
    - default `index.php` file created to replace default `index.html` file

The entire process takes just **1-2 minutes** to execute, whereas setting this up by hand often takes **more than an hour**. This procedure should leave you completely ready to start developing a web application on your Ubuntu web server.
