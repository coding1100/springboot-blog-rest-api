# Spring Boot Blog REST API

REST API for a blog application built with Spring Boot.

## Project Details
- Spring Boot: `3.2.1`
- JWT library: `0.12.3`
- Java: `17`

## Features
- JWT-based authentication (`register` and `login`)
- Role-based authorization
- CRUD APIs for posts, categories, and comments
- Pagination and sorting support
- Request validation and centralized exception handling
- OpenAPI/Swagger UI integration

## Tech Stack
- Spring Boot (Web, Security, Data JPA, Validation)
- MySQL
- Hibernate
- Lombok
- ModelMapper
- Springdoc OpenAPI

## Run Locally
1. Build the project:
```bash
./mvnw clean package
```
2. Create the database:
```sql
CREATE DATABASE myblog;
```
3. Update database credentials in:
`src/main/resources/application.properties`
4. Start the application:
```bash
./mvnw spring-boot:run
```
5. Insert default roles:
```sql
INSERT INTO myblog.roles VALUES (1, 'ROLE_ADMIN'), (2, 'ROLE_USER');
```

## API Documentation
After starting the app, open:
`http://localhost:8080/swagger-ui/index.html`
