# Online Store Backend Template
## Organize Your Store by Product, Categories and Tags

### About
This is a server api using Express.js that stores information about an online store to a MySQL database. You can add products and assign tags and categories to the products. You can add, view, update and delete all inventory and related tags and categories.

### Requirements
1. Local MySQL Server
2. Command Line Interface like Git Bash or VS Code
3. NPM Sequelize
4. NPM dotenv
5. NPM mysql2
6. NPM express
7. Insomnia app or similar


### Installation

Download or clone the app files from this link:
https://github.com/robyng/online-store-template

Go to your terminal and cd into the root of the app file. 
Write these commands one line at a time to download node modules and then install all dependencies including Sequelize, mysql2, dotenv, and express.

    npm init -y
    
    npm intall

This app requires a MySQL server on your computer. If you don't have it, follow this guide from UC Berkeley Extension Full Stack Coding Bootcamp: https://coding-boot-camp.github.io/full-stack/mysql/mysql-installation-guide

Set your MySQL password to 'password'. 
You will need a database called 'ecommerce_db'.

NOTE! If you want to use a different password or database name, just update the name and password you are using in /config/connection.js

Otherwise follow these commands one line at a time in your terminal to create the database. When prompted to enter your password enter 'password'.

    mysql -u root -p

    source db/schema.sql

    use ecommerce_db;

    quit


### Usage

To use example seeds, run once in your terminal:

    npm run seed

To start the program use this command:

    npm start

Use Insomnia app to add new products.

### Local API Routes

#### View all / Create routes
http://localhost:3001/api/products
http://localhost:3001/api/categories
http://localhost:3001/api/tags

#### View by id / Delete by id routes
Replace {id} with the primary key integer of the product, tag or category you want to work with.
Example: http://localhost:3001/api/products/2

http://localhost:3001/api/products/{id}
http://localhost:3001/api/categories/{id}
http://localhost:3001/api/tags/{id}

Watch this walkthrough showing how the program can be used:
https://watch.screencastify.com/v/bdJeEYdQTpxNwX5QFSZ3
