# Cinema-app
Complete back-end side of the Cinema application. The service that provides the following features:
- Buy a movie ticket (user)
- View all movie sessions for a specific date (user)
- Add, update, delete movie, movie session, cinema hall, etc. (admin)

## Has 2 client roles - user, admin and different permissions for each role:
- POST: /register - registration page (all roles)
 - GET: /cinema-halls - view all available Cinema Halls (all roles)
-  POST: /cinema-halls - insert new Cinema Hall (admin only)
-  GET: /movies - view all available movies (all roles)
-  POST: /movies - insert new Movie with description (admin only)
-  GET: /movie-sessions/available - view all available Movie Sessions (all roles)
-  GET: /movie-sessions/{id} - get Movie Session by Id (all roles)
-  POST: /movie-sessions - insert new Movie Session (admin only)
-  PUT: /movie-sessions/{id} - change existing Movie Session by Id (admin only)
-  DELETE: /movie-sessions/{id} - delete Movie Session by Id (admin only)
-  GET: /orders - get own orders (user only)
-  POST: /orders/complete - complete/purchase order (user only)
-  POST: /shopping-carts/movie-sessions - add a ticket for a certain Movie Session in the Shopping Cart (user only)
-  GET: /shopping-carts/by-user - get the list of own orders (user only)
-  GET: /users/by-email - get a user by email (admin only)

### Technologies used:
- Spring framework
- Spring MVC
- Spring security
- Hibernate
- SQL
- Maven
- Java
- Apache Tomcat

### The app follows the rules:
- SOLID

- REST

- N-tier architecture

### To run the project:
To run this project need to have installed
- IntelliJ IDEA Ultimate [IDEA](https://www.jetbrains.com/idea/download/#section=windows)
- ApacheTomcat [TOMCAT](https://tomcat.apache.org/download-90.cgi)
- MySQL and MySQL Workench [MySQL](https://www.mysql.com/downloads/)

- Fork the project on your IDE
- In src/main/java/resources/db.properties change URL, USERNAME and PASSWORD with your data
- jdbc.Driver is already provided, but you can change it with more suitable as well

- Configure TomCat Local server (Add New Configuration -> TomCat -> Local -> Fix -> cinema-project:war exploded -> OK
- Enjoy the project!
