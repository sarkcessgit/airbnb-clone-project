# airbnb-clone-project
# Airbnb Clone Project

## Overview
This project is a full-stack Airbnb clone that simulates a real-world booking platform. It emphasizes backend architecture, database design, API security, CI/CD integration, and team collaboration.

## Goals
- Practice collaborative software development.
- Design scalable backend systems.
- Implement security best practices.
- Deploy using modern CI/CD pipelines.

## Tech Stack
- Django
- MySQL
- GraphQL
- Docker
- GitHub Actions

## Team Roles

### Backend Developer
Responsible for designing and building the API and backend logic using Django.

### Database Administrator
Designs the relational database schema and manages data integrity using MySQL.

### DevOps Engineer
Implements CI/CD pipelines, manages Docker containers, and handles deployment.

### Security Engineer
Ensures that all APIs are secure, implements authentication/authorization.

### Project Manager
Coordinates team activities, sets deadlines, and ensures project requirements are met.

## Database Design

### Entities and Attributes:

- **Users**
  - id
  - name
  - email
  - password

- **Properties**
  - id
  - title
  - location
  - price
  - user_id (foreign key)

- **Bookings**
  - id
  - user_id (foreign key)
  - property_id (foreign key)
  - start_date
  - end_date

- **Reviews**
  - id
  - user_id (foreign key)
  - property_id (foreign key)
  - rating
  - comment

- **Payments**
  - id
  - booking_id (foreign key)
  - amount
  - payment_date

### Relationships
- A **user** can list multiple **properties**.
- A **booking** is linked to both a **user** and a **property**.
- A **review** is created by a **user** for a **property**.
- A **payment** is tied to a specific **booking**.


