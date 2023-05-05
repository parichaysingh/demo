# Spring Boot Demo Application

This is a simple Spring Boot application demonstrating REST APIs, H2 in-memory database integration, Flyway migrations, Springfox documentation, global exception handling, and basic authentication using Spring Security.

## Features

1. REST APIs: The application contains a single controller for managing Person entities through RESTful APIs.
2. H2 In-memory Database: The application uses an H2 in-memory database for persistence, along with Spring Data JPA for easy data access.
3. Flyway Migrations: Database schema management is done through Flyway migrations.
4. Springdoc OpenAPI: API documentation is generated using Springfox and can be accessed through the Swagger UI.
5. Global Exception Handling: A global exception handler handles all uncaught exceptions and returns appropriate error responses.
6. Spring Security: Basic authentication is implemented using Spring Security with in-memory users.

## How to Run

1. Clone the repository.
2. Import the project into your favorite IDE.
3. Ensure that the necessary dependencies are added to your build file (Maven or Gradle).
4. Run the `DemoApplication.java` class.
5. Access the application at the following endpoints:
    - REST APIs: `/api/person`
    - H2 Console: `/h2-console`
    - Swagger UI: `/swagger-ui/`

## Authentication

The application uses basic authentication with the following in-memory users:

| Username | Password  | Role  |
|----------|-----------|-------|
| user     | userPass  | USER  |
| admin    | adminPass | ADMIN |

## Endpoints

- `GET /api/person`: Retrieve a list of all persons.
- `POST /api/person`: Create a new person.

## Technology Stack

- Spring Boot
- Spring Data JPA
- H2 Database
- Flyway
- SpringDoc OpenAPI
- Spring Security