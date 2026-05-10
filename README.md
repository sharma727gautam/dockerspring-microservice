# DockerSpring Microservice

A multi-container application built using Spring Boot, MySQL, Docker, and Docker Compose.

This project demonstrates containerized backend development with persistent storage, optimized Docker images, secure runtime configuration, and service orchestration.

---

## Tech Stack

- Java 17
- Spring Boot
- MySQL 8
- Docker
- Docker Compose
- Maven

---

## Features

- Multi-container architecture
- Spring Boot backend container
- MySQL database container
- Docker networking
- Persistent database storage using volumes
- Environment variable based configuration
- Multi-stage Docker builds
- Non-root container execution
- Health checks and restart policies
- Production-oriented Docker setup

---

## Project Structure

```bash
dockerspring-microservice/
├── README.md
├── docker-compose.yml
└── backend/
    ├── Dockerfile
    ├── pom.xml
    └── src/
```

---

## Getting Started

### Clone Repository

```bash
git clone <your-repository-url>
cd dockerspring-microservice
```

---

## Run Application

Build and start all services:

```bash
docker compose up -d --build
```

Stop services:

```bash
docker compose down
```

---

## Access Application

Backend:

```text
http://localhost:8080
```

MySQL:

```text
localhost:3307
```

---

## Docker Concepts Implemented

- Container lifecycle management
- Docker networking
- Docker volumes
- Environment variables
- Docker Compose orchestration
- Multi-stage image optimization
- Health checks
- Resource management
- Secure container runtime

---

## Final Architecture

```text
Spring Boot Container
        │
        ▼
Docker Network
        │
        ▼
MySQL Container
        │
        ▼
Docker Volume (Persistent Storage)
```