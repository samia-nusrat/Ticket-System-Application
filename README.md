Ticket Management System
Project Overview
The Ticket Management System is a simple yet effective application built using Spring Boot. It allows users to efficiently manage tickets through a RESTful API, enabling CRUD (Create, Read, Update, Delete) operations.

Purpose
This project aims to provide a foundational ticket management system that can be expanded and integrated into larger applications. It is an excellent starting point for understanding Spring Boot and RESTful API development.

Components and Their Roles
1. Main Application (TicketSystemApplication.java)
Description: The entry point of the Spring Boot application, responsible for launching the application.
Role: Initializes the application by running the main method.
2. Model (Ticket.java)
Description: Defines the Ticket entity, representing a ticket in the system.
Role: Contains fields such as id, title, and description, and maps these fields to a database table.
3. Repository (TicketRepository.java)
Description: Provides data access methods for the Ticket entity.
Role: Extends JpaRepository, inheriting methods for saving, finding, and deleting tickets.
4. Service (TicketService.java)
Description: Contains the business logic for managing tickets.
Role: Interacts with the repository to perform operations such as:
Fetching all tickets
Finding a ticket by ID
Creating a new ticket
Deleting a ticket
5. Controller (TicketController.java)
Description: Exposes REST API endpoints for interacting with tickets.
Role: Handles HTTP requests (GET, POST, DELETE) and processes these requests using the service layer. Key endpoints include:
GET /api/tickets: Retrieve all tickets
GET /api/tickets/{id}: Retrieve a specific ticket by its ID
POST /api/tickets: Create a new ticket
DELETE /api/tickets/{id}: Delete a ticket by its ID
6. Configuration (application.properties)
Description: Contains configuration settings for the application.
Role: Configures the data source for connecting to an H2 in-memory database, setting up the database URL, username, password, and Hibernate dialect.
7. Tests (TicketSystemApplicationTests.java)
Description: Includes basic tests to ensure the application context loads correctly.
Role: Validates that the application is set up properly without errors.
