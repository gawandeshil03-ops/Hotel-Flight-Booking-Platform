# SkyStay

A full-stack hotel and flight booking platform built with **Java Spring Boot**, **React**, **TypeScript**, and **PostgreSQL**.

SkyStay enables users to search, book, and manage hotels and flights through a secure, role-based system. The project focuses on clean architecture, secure authentication, RESTful API design, and real-world booking workflows.

---

## Features

- User registration & authentication (JWT)
- Role-based authorization (Admin & Customer)
- User profile management
- Hotel & room management
- Flight management
- Hotel & flight search
- Hotel & flight bookings
- Booking history
- Mock payment processing
- Admin dashboard
- OpenAPI / Swagger documentation

---

## Tech Stack

### Frontend
- React
- TypeScript
- React Router
- React Context
- Axios
- Tailwind CSS
- React Hook Form

### Backend
- Java 21
- Spring Boot 3
- Spring Security
- Spring Data JPA (Hibernate)
- JWT Authentication
- Bean Validation

### Database
- PostgreSQL

### DevOps
- Docker
- Docker Compose
- GitHub Actions

---

## Project Structure

```text
skystay/
├── frontend/
│   ├── src/
│   └── public/
│
├── backend/
│   ├── src/main/java/io/skystay/
│   │   ├── auth/
│   │   ├── user/
│   │   ├── hotel/
│   │   ├── flight/
│   │   ├── booking/
│   │   ├── admin/
│   │   ├── config/
│   │   └── common/
│   │
│   └── src/main/resources/
│       ├── application.yml
│       └── db/migration/
│
└── docs/
```

---

## Getting Started

### Prerequisites

- Java 21+
- Node.js 20+
- PostgreSQL
- Docker (optional)

### Clone the repository

```bash
git clone https://github.com/your-username/skystay.git
cd skystay
```

### Start the backend

```bash
cd backend
docker compose up -d
./mvnw spring-boot:run
```

### Start the frontend

```bash
cd frontend
npm install
npm run dev
```

The API will be available at:

```
http://localhost:8080/api
```

Swagger documentation:

```
http://localhost:8080/swagger-ui.html
```

---

## API Overview

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Authenticate user |
| GET | `/api/users/me` | Get current user |
| PUT | `/api/users/me` | Update profile |
| GET | `/api/hotels` | Search hotels |
| GET | `/api/hotels/{id}` | Hotel details |
| POST | `/api/hotels` | Create hotel *(Admin)* |
| POST | `/api/hotels/{id}/rooms` | Add room *(Admin)* |
| GET | `/api/flights` | Search flights |
| POST | `/api/flights` | Create flight *(Admin)* |
| GET | `/api/bookings` | User bookings |
| POST | `/api/bookings/hotel` | Book hotel room |
| POST | `/api/bookings/flight` | Book flight |
| DELETE | `/api/bookings/{id}` | Cancel booking |
| GET | `/api/admin/stats` | Dashboard statistics *(Admin)* |

---

## Security

- BCrypt password hashing
- JWT authentication
- Spring Security
- Role-based authorization
- Bean Validation
- Global exception handling
- Transactional booking logic to prevent double bookings

---

## Architecture

SkyStay follows a layered architecture:

- Presentation Layer (Controllers)
- Business Layer (Services)
- Persistence Layer (Repositories)
- PostgreSQL Database

The application follows RESTful design principles with clear separation of concerns, DTOs for API communication, and secure authentication using JWT.

---

## Future Enhancements

- Online payment gateway (Stripe)
- Email notifications
- Hotel reviews & ratings
- Redis caching
- Elasticsearch
- Cloud deployment
- Microservices architecture

---


## Features

- User registration & authentication (JWT)
- Role-based authorization (Admin & Customer)
- User profile management
- Hotel & room management
- Flight management
- Hotel & flight search
- Hotel & flight bookings
- Booking history
- Mock payment processing
- Admin dashboard
- OpenAPI / Swagger documentation

---

## Tech Stack

### Frontend
- React
- TypeScript
- React Router
- React Context
- Axios
- Tailwind CSS
- React Hook Form

### Backend
- Java 21
- Spring Boot 3
- Spring Security
- Spring Data JPA (Hibernate)
- JWT Authentication
- Bean Validation

### Database
- PostgreSQL

### DevOps
- Docker
- Docker Compose
- GitHub Actions

---

## Project Structure

```text
skystay/
├── frontend/
│   ├── src/
│   └── public/
│
├── backend/
│   ├── src/main/java/io/skystay/
│   │   ├── auth/
│   │   ├── user/
│   │   ├── hotel/
│   │   ├── flight/
│   │   ├── booking/
│   │   ├── admin/
│   │   ├── config/
│   │   └── common/
│   │
│   └── src/main/resources/
│       ├── application.yml
│       └── db/migration/
│
└── docs/
```

---

## Getting Started

### Prerequisites

- Java 21+
- Node.js 20+
- PostgreSQL
- Docker (optional)

### Clone the repository

```bash
git clone https://github.com/your-username/skystay.git
cd skystay
```

### Start the backend

```bash
cd backend
docker compose up -d
./mvnw spring-boot:run
```

### Start the frontend

```bash
cd frontend
npm install
npm run dev
```

The API will be available at:

```
http://localhost:8080/api
```

Swagger documentation:

```
http://localhost:8080/swagger-ui.html
```

---

## API Overview

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Authenticate user |
| GET | `/api/users/me` | Get current user |
| PUT | `/api/users/me` | Update profile |
| GET | `/api/hotels` | Search hotels |
| GET | `/api/hotels/{id}` | Hotel details |
| POST | `/api/hotels` | Create hotel *(Admin)* |
| POST | `/api/hotels/{id}/rooms` | Add room *(Admin)* |
| GET | `/api/flights` | Search flights |
| POST | `/api/flights` | Create flight *(Admin)* |
| GET | `/api/bookings` | User bookings |
| POST | `/api/bookings/hotel` | Book hotel room |
| POST | `/api/bookings/flight` | Book flight |
| DELETE | `/api/bookings/{id}` | Cancel booking |
| GET | `/api/admin/stats` | Dashboard statistics *(Admin)* |

---

## Security

- BCrypt password hashing
- JWT authentication
- Spring Security
- Role-based authorization
- Bean Validation
- Global exception handling
- Transactional booking logic to prevent double bookings

---

## Architecture

SkyStay follows a layered architecture:

- Presentation Layer (Controllers)
- Business Layer (Services)
- Persistence Layer (Repositories)
- PostgreSQL Database

The application follows RESTful design principles with clear separation of concerns, DTOs for API communication, and secure authentication using JWT.

---

## Future Enhancements

- Online payment gateway (Stripe)
- Email notifications
- Hotel reviews & ratings
- Redis caching
- Elasticsearch
- Cloud deployment
- Microservices architecture

---

