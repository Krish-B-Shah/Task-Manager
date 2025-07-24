# Task Manager Prototype

A Java Spring Boot REST API for secure task management with JWT authentication. This project demonstrates backend API design and security best practices, making it an ideal starter project for learning or extending task management systems.

## Features

- **JWT Authentication:** Secure endpoints with JSON Web Tokens for stateless authentication.
- **Full CRUD Operations:** Create, Read, Update, and Delete tasks via RESTful endpoints.
- **MySQL Persistence:** Store tasks and user data in a MySQL database.
- **Input Validation:** Robust validation for all incoming data to ensure data integrity.
- **Exception Handling:** Centralized error handling for clean and informative API responses.

## Tech Stack

- Java 17+
- Spring Boot
- Spring Security (JWT)
- Spring Data JPA
- MySQL
- Maven

## Getting Started

### Prerequisites
- Java 17 or higher
- Maven
- MySQL Server

### Setup
1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd Task-Manager
   ```
2. **Configure MySQL:**
   - Create a database (e.g., `task_manager`).
   - Update `src/main/resources/application.properties` with your MySQL credentials.
3. **Build and run the application:**
   ```bash
   mvn spring-boot:run
   ```
4. **API Endpoints:**
   - Authentication: `/api/auth/*`
   - Task management: `/api/tasks/*`

## Usage
- Register and log in to receive a JWT token.
- Use the token in the `Authorization: Bearer <token>` header for all protected endpoints.

## Example Requests

```
POST /api/auth/register
POST /api/auth/login
GET /api/tasks
POST /api/tasks
PUT /api/tasks/{id}
DELETE /api/tasks/{id}
```

## License

This project is open source and available under the [MIT License](LICENSE). 
