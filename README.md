# Barbershop Booking Platform

A Spring Boot web application for managing client appointments in a barbershop. The project includes authentication, role-based access, appointment records, admin views, Thymeleaf templates, and PostgreSQL persistence.

## Tech Stack

- Java 17
- Spring Boot 2.6
- Spring Security
- Thymeleaf
- Spring Data JPA
- PostgreSQL
- Maven

## Features

- User registration and login
- Appointment booking flow
- User appointment history
- Admin management page
- Server-rendered UI with static assets
- Environment-based database configuration

## Run Locally

Create a PostgreSQL database and configure connection values:

```bash
cp .env.example .env
```

Run the application:

```bash
./mvnw spring-boot:run
```

On Windows:

```powershell
.\mvnw.cmd spring-boot:run
```

## Configuration

The application reads database settings from environment variables:

| Variable | Default |
| --- | --- |
| `DATABASE_URL` | `jdbc:postgresql://localhost:5432/barbershop` |
| `DATABASE_USERNAME` | `postgres` |
| `DATABASE_PASSWORD` | `postgres` |

## Portfolio Notes

This project demonstrates a classic monolithic Java web application with MVC structure, authentication, persistence, and server-side rendering.

