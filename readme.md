# Wordpress Theme Development

## Introduce Yourself

- Name
- What do you want to get out of this workshop?
- What (if anything) have you done with WordPress?

## Learning Objectives

- Understand the capabilities of WordPress as a blogging platform and CMS. 
- Incorporate basic HTML and CSS in a WordPress Theme
- Develop a custom WordPress Theme from scratch 
- Learn how to customize navigation 
- Understand how to leverage the WordPress plug-in library

## Schedule

- Getting started with WordPress 
- wordpress.com vs wordpress.org 
- Local WordPress development 
- WordPress Themes 
- Posts and Pages 
- Widgets and Plugins 
- Custom Posts and Pages 
- What is the WordPress Codex? 
- What is the WP Hierarchy
- Domains, Hosting, and Deployment

## Getting started with WordPress 

WordPress is a content management system. You 
get a nicely designed admin area for managing all of 
your content on the site. WordPress allows for 
plugins to extend the built in functionality of 
WordPress. About 25% of all sites on the internet 
are powered by WordPress. WordPress is an open 
source project which means you can download and 
use the files for free.

## wordpress.com vs wordpress.org 

On wordpress.org you can download and install a software script called
WordPress. To do this you need a web host who meets the minimum 
requirements and a little time. WordPress is completely customizable 
and can be used for almost anything. There is also a service called 
WordPress.com which lets you get started with a new and free 
WordPress-based blog in seconds, but varies in several ways and is 
less flexible than the WordPress you download and install yourself.

## Local WordPress Development 

- Install MAMP (Mac) or XAMPP (Windows)
- Start local server (MAMP or XAMPP) 
- Navigate to ‘htdocs’ in your MAMP or XAMPP folder 
- Create a folder named ‘wordpress’ in your ‘htdocs’ folder 
- Go to wordpress.org and download the most recent version of WordPress 
- Open the WordPress download and copy all files into the ‘wordpress’ folder in htdocs 
- Create a project folder in ‘htdocs’ and copy all files from ‘wordpress’ folder into project folder 
- Go to ‘localhost’ in a web browser while your MAMP or XAMPP server is running to view your newly created ‘wordpress’ and ‘project’ site folder projects
- Click on your newly created project folder and follow the prompt to create your wp-config.php file 
- Go to the start page for MAMP or XAMPP and go to the phpMyAdmin portal. 
- Click on the database tab and create a new database which you can name the same as your project 
- Go back to your web browser to finish setting up WordPress locally and enter in the database name you just created. Since we are working locally you can use ‘root’ for the database username and password. I would use ‘localhost’ for the database host but change the database prefix from ‘wp_’ to ‘wp_projectname_’ 
- Run the install 
- Enter a site title, username, and password and uncheck private so search engines do not index your site. This username and password is what you will use to login to localhost/projectname/wp-admin 
- Click install WordPress and login to your newly created, locally hosted WordPress site!

### You do: Wordpress Admin

- Click admin link. 
- Create at least two posts and two new pages.
- Configure your site to show posts on the home page.
- Change the site’s theme.

## WordPress Themes 

- We can search for other themes and we are searching the WordPress.org theme repository 
- Themeforest.net we can purchase themes and upload them
- Themes live in wp-content/themes in our htdocs folder

### We do:

    $ mkdir wp-content/themes/milky-way
    $ cd wp-contents/themes/milky-way
    $ touch index.php styles.css functions.php

### CSS & JS

- style.css under the meta data for the theme is where you can add your css 
- If you have additional css files, enqueue in the functions.php 
- You can create a css and js folder in the root of your theme 
- Function: wp_enqueue_style 
  - https://codex.wordpress.org/Function_Reference/wp_enqueue_style
- Function: wp_enqueue_script 
  - https://codex.wordpress.org/Function_Reference/wp_enqueue_script

### Header and Footer

- Create both files and use get_header(); and get_footer(); in index.php file 
- Function: wp_title(); in the title html tag in the header to display in the browser tab 
- Function: wp_head(); inside the header.php file

### The Loop

It checks what is available for that particular page and then displays it. 
The loop starts with an if statement, them moves into a while statement 
as long as there is content to be displayed. Inside the loop is the HTML 
and PHP markup to display what is in the loop. 

https://codex.wordpress.org/The_Loop

## Posts and Pages 

https://developer.wordpress.org/themes/basics/template-files/

- Custom Page Templates
- Global Page Templates
- Meta Data

## Plugins 

- [Advanced Custom Fields](http://www.advancedcustomfields.com/)
- [Custom Post Type UI](https://wordpress.org/plugins/custom-post-type-ui/)
- [SEO by Yoast](https://wordpress.org/plugins/wordpress-seo/)
- [Google Analytics](https://wordpress.org/plugins/google-analytics-for-wordpress/)
- [Contact Form 7](https://wordpress.org/plugins/contact-form-7/)

## Custom Posts and Pages 

## What is the WordPress Codex? 

## Domains, Hosting, and Deployment
