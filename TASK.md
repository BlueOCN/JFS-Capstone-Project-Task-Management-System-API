# JFS-Capstone-Project-Task-Management-System-API
Spring Boot-based Task Management System with JWT-secured REST APIs, role-based access (Admin/User), and full CRUD for tasks. Built with Spring Data JPA, supports logging, monitoring, and optional features like search, pagination, and email alerts.

## Objective:

Build a Task Management System using Spring Boot that allows users to create, manage, and track tasks. The system should implement RESTful APIs for performing CRUD (Create, Read, Update, Delete) operations, secure endpoints using Spring Security and JWT, and integrate with an SQL database using Spring Data JPA.

## Evaluation Criteria:

Code quality and adherence to best practices
Proper use of Spring Boot features (Security, JPA, Actuator)
Database design and optimization
API design and documentation
Testing coverage and code reliability

## Deliverables:

1. A working Spring Boot application with all core features implemented.
2. API documentation (using Swagger/OpenAPI).
3. A README file explaining project setup, usage, and dependencies.
4. A presentation/demo video explaining your architecture, challenges, and key features (5–10 minutes).

## Project Requirements: 

### Core Features

#### User Authentication and Authorization:
- Implement registration and login functionality.
- Secure endpoints with Spring Security and issue JWT tokens.
- Role-based access (Admin, User).

#### Task Management API:
- Create, view, update, and delete tasks.
- Each task should include:
- Task ID (auto-generated)
- Title
- Description
- Status (e.g., Pending, In Progress, Completed)
- Priority (e.g., Low, Medium, High)
- Due Date
- Only the user who created a task can modify or delete it.

#### Admin Controls:
- Admin users can view and delete any task.
- Admin dashboard endpoint to list users and their task counts.

---

### Database Integration
- Use Spring Data JPA with a relational database (MySQL, PostgreSQL, or H2 for testing).
- Implement relationships where necessary (e.g., One-to-Many between users and tasks).

---

### Logging and Monitoring
- Implement logging using Spring Boot Logging to track API requests.
- Integrate Spring Boot Actuator for monitoring and exposing metrics (e.g., health checks, metrics endpoints).

---

### Advanced Features (Optional for Extra Credit)
- Add pagination and sorting for listing tasks.
- Implement search functionality based on task status, priority, or due date.
- Add email notifications for tasks nearing their due date (using Spring Boot Mail).

---

### Technical Requirements
- Follow RESTful principles for endpoint design.
- Use DTOs (Data Transfer Objects) for sending data between the client and server.
- Exception handling using Spring’s @ControllerAdvice.
- Write unit and integration tests using JUnit and Mockito.

