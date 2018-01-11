Restful CRUD API for a simple Employee Management application using Spring Boot, Mysql, JPA and Hibernate.

Requirements

1. Java - 1.8.x

2. Maven - 3.x.x

3. Mysql - 5.x.x

Steps to Setup

1. Clone the application


https://github.com/haminipreetha/EmpManagement_Hamini


2. Create Mysql database

create database hamini (or change the below in Application.properties if you already have any database)

spring.datasource.url = jdbc:mysql://localhost:3306/Your_DB_Name_here_?autoReconnect=true&useUnicode=true&characterEncoding=UTF-8&allowMultiQueries=true&useSSL=false



3. Change mysql username and password as per your installation**

+ open `src/main/resources/application.properties`

+ change `spring.datasource.username` and `spring.datasource.password` as per your mysql installation


4. Build and run the app using maven

give maven clean,maven install

then go to Run -> Run as configurations -> give Goals as spring-boot:run then give run


The app will start running at <http://localhost:8080>.

The app defines following CRUD APIs.

    GET /api/employees
    
    POST /api/employees
    
    GET /api/employees/{id}
    
    PUT /api/employees/{id}
    
    DELETE /api/employees/{id}

You can test them using postman or any other rest client.

This Api is tested with POSTMAN before integrating with angular.

Screenshots added in the attachement.
