# Cinema app
This is a prototype of a web application that works like a movie theater. In this application, user can have two roles ADMIN or USER.
## Technologies used
* Java
* Hibernate
* Spring (Core, Web, Security)
* MySQL
* Maven
* Apache Tomcat
## The structure of the project
* Data access layer (DAO).
* Application layer (service).
* Presentation layer (controllers).
## Available endpoints, depending on what roles the user has
* POST: /register - all  
* POST: /cinema-halls - admin 
* POST: /movies - admin     
* POST: /movie-sessions - admin  
* PUT: /movie-sessions/{id} - admin  
* DELETE: /movie-sessions/{id} - admin  
* GET: /users/by-email - admin   
* GET: /cinema-halls - user/admin  
* GET: /movies - user/admin  
* GET: /movie-sessions/available - user/admin  
* GET: /movie-sessions/{id} - user/admin  
* GET: /orders - user  
* POST: /orders/complete - user   
* PUT: /shopping-carts/movie-sessions - user  
* GET: /shopping-carts/by-user - user 

##Setup
1. Install and configure Apache Tomcat(v9.0.50)
2. Install MySQL with MySQL Workbench
3. Fork this project on GitHub
4. In the /resources/db.properties file, replace the stubs with your database data
5. Run the application