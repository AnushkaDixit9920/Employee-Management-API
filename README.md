📚 Employee Management API
---

A simple Spring Boot REST API for managing employee data.
This project demonstrates CRUD operations, Swagger documentation, input validations, and global exception handling .

---
🔧 Features
✅ Create, Read, Update, and Delete (CRUD) operations on Employees
✅ API Documentation with Swagger UI
✅ Field-level validations (e.g., name, email, department, salary)
✅ Exception handling with clean and meaningful JSON error responses
✅ Clean architecture with Controller Layer, Service Layer, Repository Layer, and Exception Handler Layer

🚀 Tech Stack

Java 17+

Spring Boot 3+

Spring Web

Spring Data JPA (Hibernate)

Hibernate Validator

MySQL Database

Swagger UI (springdoc-openapi)

Maven

📂 Project Structure
src/main/java/com/example/employeemanagement
├── controller      --> REST Controllers
├── model           --> JPA Entity (Employee)
├── exception       --> Custom Exceptions & Global Handler
├── repository      --> JPA Repository Interface
├── service         --> Service Layer with business logic


🔗 Swagger UI

Access your API documentation at:
http://localhost:8080/swagger-ui/index.html

⚙️ API Endpoints
| **Method** | **Endpoint**          | **Description**             |
| ---------- | --------------------- | --------------------------- |
| GET        | `/api/employees`      | Get all employees           |
| GET        | `/api/employees/{id}` | Get an employee by ID       |
| POST       | `/api/employees`      | Add a new employee          |
| PUT        | `/api/employees/{id}` | Update an existing employee |
| DELETE     | `/api/employees/{id}` | Delete an employee          |

🛡️ Exception Handling

The API includes robust exception handling with clear and meaningful error messages.

Handled exceptions:

Resource Not Found (404): Returned when an employee with the given ID does not exist.

Validation Errors (400): Triggered when fields like name, email, department, or salary fail validation.

Database Errors: Any database-related issue such as constraint violations or connection failures.

Generic Server Errors (500): Catches unexpected exceptions to prevent raw stack traces and return clean JSON responses.


▶️ Running the Application

1)Set up MySQL and update your
  application.properties
  with your database name, username, and password.

2)Run the project using IntelliJ IDEA
  or run it from the terminal with:
  mvn spring-boot:run

3)Once the application starts, open Swagger UI at:
  http://localhost:8080/swagger-ui/index.html

  to explore and test all Employee APIs.

🤝 Contributing
  Feel free to fork and contribute! Improvements like JWT Authentication, pagination, or Docker support are welcome.
  Let me know if you'd like to add:

  Setup instructions for MySQL

  API request/response examples

Author:
Anushka Dixit



