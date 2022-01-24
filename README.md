# Cinema app
This is a prototype of a web application that works like a movie theater. In this application, user can have two roles ADMIN or USER.
## Technologies used
* Java
* Hibernate
* Spring Framework
* REST
* MySQL
* Maven
* Apache Tomcat
## The structure of the project
* Data access layer (DAO).
* Application layer (service).
* Presentation layer (controllers).
## Endpoints available
* POST: /register - all  
* POST: /cinema-halls - admin role required  
* POST: /movies - admin role required    
* POST: /movie-sessions - admin role required  
* PUT: /movie-sessions/{id} - admin role required  
* DELETE: /movie-sessions/{id} - admin role required  
* GET: /users/by-email - admin role required  
* GET: /cinema-halls - user/admin  
* GET: /movies - user/admin  
* GET: /movie-sessions/available - user/admin  
* GET: /movie-sessions/{id} - user/admin  
* GET: /orders - user role required  
* POST: /orders/complete - user role required  
* PUT: /shopping-carts/movie-sessions - user role required  
* GET: /shopping-carts/by-user - user role required
##Setup
1. Install and configure Apache Tomcat(v9.0.50)
2. Install MySQL with MySQL Workbench
3. Fork this project on GitHub
4. In the /resources/db.properties file, replace the stubs with your database data
5. Run the application