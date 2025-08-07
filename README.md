# 🏥 Patient Management System (Microservices Architecture)

This is a modular Patient Management Application built using Java Spring Boot and microservices architecture. It features core services such as authentication, patient management, and analytics, and uses Spring Cloud Gateway for routing, gRPC for inter-service communication, and Kafka for asynchronous messaging.

---

## 🧩 Microservices

### 1. **auth-service**
- Handles user authentication (JWT-based)
- Spring Security integrated
- Generates and validates JWT tokens

### 2. **patient-service**
- Manages patient data (CRUD)
- Exposes REST & gRPC APIs
- Publishes Kafka events on patient updates

### 3. **analytics-service**
- Listens to Kafka topics for patient events
- Performs analytics & aggregates data

### 4. **api-gateway**
- Entry point to all services
- Handles routing via Spring Cloud Gateway
- Includes `StripPrefix`, `Path` routing, etc.

---

## 🚀 Tech Stack

| Component            | Tech                                 |
|----------------------|--------------------------------------|
| Core Framework       | Spring Boot                          |
| Service Communication| gRPC                                 |
| Asynchronous Events  | Apache Kafka                         |
| API Gateway          | Spring Cloud Gateway                 |
| Security             | Spring Security + JWT                |
| Build Tool           | Maven                      |
| Containerization     | Docker                    |

---



