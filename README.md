
# Spring REST CRUD Practice Project

## Overview
This repository contains code from my learning practice with Spring REST APIs. The project demonstrates basic CRUD (Create, Read, Update, Delete) functionality for managing an Employee Directory.

### Please go through the branch or commit history for detailed working history. I made CRUD features without using Data JPA and Data Rest first. Then I have included Data JPA and then finally in the master branch you can see the CRUD features code using Data Rest.


## Features
- **Create**: Add new employees to the directory.
- **Read**: Fetch details of all employees or a specific employee.
- **Update**: Modify details of an existing employee.
- **Delete**: Remove an employee from the directory.

## Technologies Used
- **Spring Framework**: For building RESTful APIs.
- **Hibernate**: For ORM (Object Relational Mapping).
- **MySQL**: As the database.
- **Maven**: For dependency management.
- **Postman**: For testing APIs.

## Installation and Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/spring-rest-crud-practice.git
   ```
2. Navigate to the project directory:
   ```bash
   cd spring-rest-crud-practice
   ```
3. Import the project into your preferred IDE (e.g., IntelliJ IDEA or Eclipse).
4. Configure the database connection in `application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/employee_directory
   spring.datasource.username=your-username
   spring.datasource.password=your-password
   ```
5. Run the application:
   ```bash
   mvn spring-boot:run
   ```
6. Use Postman or a web browser to interact with the APIs at `http://localhost:8080`.

## API Endpoints
- **GET /employees**: Retrieve all employees.
- **GET /employees/{id}**: Retrieve a specific employee by ID.
- **POST /employees**: Add a new employee.
- **PUT /employees/{id}**: Update an existing employee.
- **DELETE /employees/{id}**: Delete an employee by ID.

## Project Structure
```
src/
├── main/
│   ├── java/
│   │   └── com.example.springboot.cruddemo/
│   │       ├── rest/       # REST controllers
│   │       ├── entity/            # Employee entity
│   │       ├── dao/       # DAO interface and implementation
│   │       └── service/          # Service layer
│   └── resources/
│       ├── application.properties # Configuration
│       └── data.sql              # Sample data (optional)
```

## Acknowledgments
This project is a part of my personal learning journey to understand Spring REST and CRUD functionalities. Special thanks to the Spring documentation and online resources for guidance.
