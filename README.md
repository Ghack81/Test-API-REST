# Create and use a REST API in PHP

REST (Representational State Transfer) is one way to access web services. The REST API is used to make a client-side HTTP GET, POST, PUT or DELETE request to the server to retrieve or modify certain information on the server.

REST-based web services can produce output in any format, such as CSV, JSON, RSS, etc. So it depends on the format you want to easily parse with your language. In this tutorial, we will create a simple REST API using the PHP language.
Let's start by creating an example rest API, we will create an 'api/' directory. This directory contains all the files needed for this tutorial. We will create rest api for product module which will have HTTP Get, Post, Put and Delete request to fetch, add, update and delete records from mysql. The rest API details are as follows:
Road            Method        Kind                                                                                  Description
http://127.0.0.1/api/products GET JSON                                       Retrieve all products.
http://127.0.0.1/api/products/{id} GET JSON                                  Retrieve single product data
http://127.0.0.1/api/products POST JSON                                 Insert a new product into the database.
http://127.0.0.1/api/products/{id} PUT JSON                                  Update a product in the database.
http://127.0.0.1/api/products/{id} DELETE JSON                              Delete a product from the database.

We will be using the following files for this tutorial:

- index.php: This file is an input file. This file prevents directory file browsing.
- db_connect.php: This file will use the mysql connection string.
- products.php: This file contains all REST API methods.
- post.php: This file allows you to send a POST request to our REST API to test the addition of a new product.
- put.php: This file allows you to send a PUT request to our REST API to test the update of a new product.
- delete.php: This file allows you to send a DELETE request to our REST API to test the deletion of a new product.
-.htaccess: This file is used for routing.

Let's go !

Conclusion
There is another solution, to test the GET/POST/PUT/DELETE methods that we have seen in this tutorial by using Postman, which is an open-source tool for testing RESTful APIs that you have created yourself. It offers a user interface with which to make HTML requests, without having to write a bunch of code just to test the functionality of an API.