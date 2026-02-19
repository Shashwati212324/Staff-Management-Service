#🚀 Staff Management Service

A RESTful backend application built using Spring Boot for managing organizational staff records.

This service provides CRUD APIs to create, retrieve, update, and delete employee and department data using a layered architecture approach.

##📌 Overview

Staff Management Service is designed to demonstrate backend development best practices including:

REST API design

Layered architecture (Controller → Service → Repository)

ORM-based persistence using JPA

In-memory database integration

Clean and modular project structure

##🛠 Tech Stack

Java 21

Spring Boot

Spring Web

Spring Data JPA

Hibernate

H2 In-Memory Database

Gradle

##🏗 Architecture

The application follows a clean layered architecture:

Controller → Service → Repository → Database

##📂 Project Structure
src/main/java/
│
├── controller      # REST Controllers
├── service         # Business Logic
├── repository      # Data Access Layer
├── entity          # JPA Entities
├── dto             # Data Transfer Objects
├── config          # Configuration Classes
└── StaffManagementServiceApplication.java

##✨ Features

Add new staff member

Retrieve all staff members

Retrieve staff by ID

Update staff details

Delete staff records

Department management support

In-memory database for development/testing

##▶️ Running the Application
1️⃣ Clone the Repository
git clone https://github.com/your-username/Staff-Management-Service.git
cd Staff-Management-Service

2️⃣ Build the Project
./gradlew clean build


Windows:

.\gradlew clean build

3️⃣ Run the Application
./gradlew bootRun


Application will start at:

http://localhost:8080

##🌐 API Endpoints
Employee APIs
Method	Endpoint	Description
GET	/employees	Get all employees
GET	/employees/{id}	Get employee by ID
POST	/employees	Create new employee
PUT	/employees/{id}	Update employee
DELETE	/employees/{id}	Delete employee

##🧪 Testing the APIs

You can test the APIs using:

Postman

Browser (for GET requests)

🗄 H2 Database Console

Access H2 Console at:

http://localhost:8080/h2-console


##Default configuration:

JDBC URL: jdbc:h2:mem:testdb
Username: sa
Password: (leave blank)

📦 Sample Request (POST /employees)
{
  "name": "John Doe",
  "email": "john.doe@example.com",
  "department": "IT"
}

##🎯 Key Learnings

RESTful API development with Spring Boot

Layered architecture implementation

JPA entity mapping and repository abstraction

Gradle build configuration

Environment-based project setup

##🔮 Future Enhancements

Global exception handling

Input validation using @Valid

Swagger/OpenAPI documentation

Integration with MySQL or PostgreSQL

Authentication using Spring Security + JWT
