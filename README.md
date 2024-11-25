# Restful API for Online eCommerce Application using SpringBoot and Reactjs for frontEnd with Spring Security with JWT Implementation

An eCommerce Application backend with Java Spring Boot with frontend using the Reactjs

- Welcome to the documentation for the Ecommerce API, a powerful RESTful API for an Online eCommerce Application developed using Spring Boot, Spring Security with JWT implementation, and React for the frontend. This API provides comprehensive endpoints to support various features of an Ecommerce Application.

## Tech Stack and Technology Used

- Java
- Spring Framework
- Spring Boot
- JavaScript
- React
- Spring Data JPA
- Hibernate
- MySQL (DataBase)
- Swagger
- Spring Security
- JSON Web Tokens (JWT)
- BCrypt
- Maven
- Axios

## Schema Table
![ER_diagram](https://github.com/supratiktechandanalytics/Sukart/blob/main/ER_diagram.png)

## Features

- User registration and login with JWT authentication
- Password encryption using BCrypt
- Role-based authorization with Spring Security for user and admin
- Customized access denied handling
- User Module
- Admin Module

## Getting Started

To get started with this project, you will need to have the following installed on your local machine:

- JDK 17+
- Maven 3+

## Installation & Run
To install this application, run the following commands:

### Clone the project repository:
```bash
git clone https://github.com/Vivekgupta96/eCommerce-Application.git
```
### Navigate to the project directory:
```
cd eCommerce-Application

```

This will get a copy of the project installed locally. To configure all of its dependencies and start each app, follow the instructions below.

### Configure Database

Once MySQL is installed you must configure a username and password. By default the user and password should be `root` . If not, you must configure in the file `application.configure` located in the path `src/main/resources/`.

In the file `application.configure` you must edit the parameters `spring.datasource.username` and `spring.datasource.password` with the values you defined.

```
    server.port=8080

    spring.datasource.url=jdbc:mysql://localhost:3306/Ecomdb
    spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
    spring.datasource.username=SQLUsername(i.e=root)
    spring.datasource.password=SQLUserPassword(i.e=root)

```

## Build and run the Spring Boot application using CMD
```
mvnw spring-boot:run
```
```


## API Root Endpoint with Swagger Documentation

```
### https://localhost:8080/

###  Railway Deployed Apis
https://api-ecom.up.railway.app/swagger-ui/index.html#/
### http://localhost:8080/swagger-ui/index.html
```

- To Get Access as admin , you have to use below query for register the admin for the first time in MySQL databse folling are details below

```
step:1
use ecomdb;

step:2

INSERT INTO users (email, password, first_name, last_name, phone_number,user_role,user_account_status)
VALUES ('admin@gmail.com', 'admin@1234', 'Admin', 'Admin', '9999999999',ROLE_ADMIN,ACTIVE);

step:3
Admin Login using credetials ,now you are ready to do all aldmin operation

```

## Admin Access point :- On Footer section rightSide (Admin Access) at Landing / Home PAge

## For Running frontend in Local Machine

- Getting Started

* Before you can run the React frontend, make sure you have the following prerequisites installed on your machine:

* Node.js: Ensure you have Node.js installed.

### Installation

- Once you have the prerequisites in place, follow these steps to install the required packages for the React frontend:

- Open your terminal and navigate to the root directory of the React frontend project. This is the directory where you find the package.json file.

- Run the following command to install all the necessary packages:

```
npm install
```

- This command will download and install all the dependencies listed in the package.json file.

### Running the Application

- To run the React frontend locally, follow these steps:

- Open your terminal and navigate to the root directory of the React frontend project.

- Run the following command to start the development server:

```
npm start
```

