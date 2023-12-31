[![Typing SVG](https://readme-typing-svg.herokuapp.com?size=30&pause=1000&color=F7F7F7&width=435&lines=Cinema-app)](https://git.io/typing-svg)
![CINEMA!](src/images/imagesCinema.png)


**CinemaApp is a user-friendly RESTful web application designed for convenient ticket booking. It empowers users to explore and reserve seats for available movie sessions effortlessly. The application is equipped with essential features, including user authentication and authorization, enabling secure access for registered users and administrators. Regular users can easily register, log in, and book tickets for their preferred movies, while administrators enjoy extra privileges, such as managing cinema halls, 
movies, and movie sessions to ensure smooth operation.**

## Table of Contents

- [Functionality](#functionality)
- [Endpoints](#endpoints)
- [Project Structure](#project-structure-)
- [Entities relations diagram](#entities-relations-diagram-)
- [Technologies Used](#technologies-used-)
- [Instructions for Launching the Project](#instructions-for-launching-the-project)

## Functionality

The Cinema-app offers a range of essential functionalities catering to both users and administrators:
#### User Functionality:

- Registration, login, and logout.
- Viewing cinema halls, movies, and available movie sessions.
- Adding tickets to the shopping cart and creating an order based on the added tickets.
- Viewing and completing orders.
- Buying tickets.
- Viewing and updating the shopping cart.

#### Admin Functionality:

- Adding and managing cinema halls, movies, and movie sessions.
- Finding users by their email address.

## Endpoints

The Cinema-app provides the following endpoints:

#### User and Admin Endpoints:

- POST: /register - User registration.
- GET: /cinema-halls - View cinema halls.
- GET: /movies - View movies.
- GET: /movie-sessions/available - View available movie sessions.

#### Admin Endpoints:

- POST: /cinema-halls - Add a new cinema hall.
- POST: /movies - Add a new movie.
- POST: /movie-sessions - Add a new movie session.
- PUT: /movie-sessions/{id} - Update a movie session.
- DELETE: /movie-sessions/{id} - Delete a movie session.
- GET: /users/by-email - Find a user by their email address.

#### User Endpoints:

- GET: /orders - View user's orders.
- POST: /orders/complete - Complete an order.
- PUT: /shopping-carts/movie-sessions - Update the shopping cart with movie sessions.
- GET: /shopping-carts/by-user - View the shopping cart for a specific user.

## Project structure:

- src/main/java - contains the entire source code of the program
- src/main/resources - contains properties for connecting to the database

## Entities relations diagram:

![DIAGRAM!](src/images/schema.png)

## Technologies used:

- Java 17
- Tomcat 9.0.75
- MySQL 8.0.22
- Maven 3.1.1
- Java Servlet 4.0.1
- Hibernate 5.6.14.Final
- JDBC
- Spring 5.3.20
- Spring-Web 5.3.20
- Spring-Security 5.6.10


## Instructions for launching the project
1. Clone the project from GitHub;
2. Install Apache Tomcat version 9.x.x.;
3. Install MySql;
4. Install Postman for sending requests;
5. Congigure db.properties with correct data;
6. Add TomCat configuration;
7. Run the project.