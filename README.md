# Healthcare Patient Support & Appointment Management System

A full-stack healthcare management application designed to simplify patient support, appointment management, and healthcare staff operations through a centralized web platform.

The project demonstrates modern **Full Stack Development**, **REST API development**, **database management**, **authentication**, **role-based authorization**, and **enterprise application architecture**.

---

## 📌 Project Overview

Healthcare organizations often need a centralized system to manage patient information, appointments, support requests, and administrative activities.

This project provides a web-based platform with separate functionality for:

* Patients
* Healthcare staff
* Administrators

The application is designed with a frontend-backend architecture where the React frontend communicates with Java Spring Boot REST APIs and the backend manages application data through a relational database.

---

## 🎯 Objectives

The main objectives of this project are:

* Provide a centralized healthcare support platform
* Allow patients to manage appointments
* Provide healthcare staff with an operational dashboard
* Manage patient support requests
* Implement secure authentication and authorization
* Expose reusable REST APIs
* Validate user input
* Maintain structured healthcare-related data
* Demonstrate enterprise-style application development

---

## 🏗️ Technology Stack

### Frontend

* React.js
* JavaScript
* HTML5
* CSS3
* Vite

### Backend

* Java
* Spring Boot
* Spring Web
* REST APIs
* Spring Data JPA
* Bean Validation

### Database

* MySQL / relational database architecture
* H2 for local development/testing

### Security

* JWT Authentication
* Role-Based Access Control
* Input Validation

### DevOps & Tools

* Docker
* Git
* GitHub
* Maven
* Postman

---

## 🏛️ System Architecture

```text
                    ┌─────────────────────┐
                    │      Patient        │
                    │   Staff / Admin     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    React Frontend   │
                    │      Web UI          │
                    └──────────┬──────────┘
                               │
                         REST / JSON
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Spring Boot API   │
                    │                     │
                    │ Business Logic      │
                    │ Authentication      │
                    │ Validation          │
                    │ Authorization       │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   SQL Database      │
                    │                     │
                    │ Users               │
                    │ Patients            │
                    │ Appointments         │
                    │ Support Requests     │
                    └─────────────────────┘
```

---

## 👥 User Roles

### Patient

Patients can:

* Create an account
* Log in securely
* Manage their profile
* Book appointments
* View appointment history
* Submit healthcare support requests
* Track request status

### Healthcare Staff

Healthcare staff can:

* View appointments
* Manage patient requests
* Update appointment/request status
* Review patient-related information
* Use the staff dashboard

### Administrator

Administrators can:

* Manage users
* Manage staff accounts
* Monitor application activity
* View system information
* Manage administrative operations

---

## 🚀 Main Features

### Authentication

* User registration
* Secure login
* Password protection
* JWT-based authentication
* Session/token validation

### Appointment Management

* Book appointments
* View appointments
* Appointment history
* Appointment status management
* Staff-side appointment management

### Patient Support

* Create support requests
* Track request status
* Staff response/update workflow
* Request categorization

### Administration

* User management
* Staff management
* Dashboard
* Application monitoring

### API

REST APIs are used for communication between the frontend and backend.

Example endpoints:

```text
GET    /api/health
GET    /api/appointments
POST   /api/auth/register
POST   /api/auth/login
GET    /api/patients
POST   /api/appointments
PUT    /api/appointments/{id}
GET    /api/support-requests
POST   /api/support-requests
```

---

## 🔐 Security Features

The project demonstrates common application-security practices:

* JWT authentication
* Role-based authorization
* Password hashing
* Server-side input validation
* Protected API endpoints
* Error handling
* Secure authentication workflow

> This is an educational portfolio project and should not be used to store real patient/medical information.

---

## 📂 Project Structure

```text
Healthcare-Full-Stack-Management-System/
│
├── backend/
│   ├── src/
│   │   └── main/
│   │       ├── java/
│   │       │   └── com/
│   │       │       └── omkar/
│   │       │           └── healthcare/
│   │       │               ├── HealthcareApplication.java
│   │       │               └── HealthController.java
│   │       │
│   │       └── resources/
│   │           └── application.properties
│   │
│   └── pom.xml
│
├── frontend/
│   ├── src/
│   │   ├── main.jsx
│   │   └── style.css
│   │
│   ├── index.html
│   └── package.json
│
├── docker-compose.yml
├── .gitignore
└── README.md
```

---

## ⚙️ Backend Setup

### 1. Navigate to backend

```bash
cd backend
```

### 2. Run the application

```bash
mvn spring-boot:run
```

The backend will start at:

```text
http://localhost:8080
```

### 3. Test the API

Open:

```text
http://localhost:8080/api/health
```

Expected response:

```json
{
  "status": "UP",
  "service": "healthcare-api"
}
```

---

## 💻 Frontend Setup

### 1. Navigate to frontend

```bash
cd frontend
```

### 2. Install dependencies

```bash
npm install
```

### 3. Start the development server

```bash
npm run dev
```

The frontend will be available through the Vite development server.

---

## 🐳 Docker

The project includes Docker configuration for running the backend in a containerized environment.

Start the backend using:

```bash
docker compose up
```

Stop the containers:

```bash
docker compose down
```

---

## 🧪 Testing

The project can be tested using:

### API Testing

**Postman**

Test:

* Registration
* Login
* Authentication
* Appointment APIs
* Support-request APIs
* Authorization

### Backend Testing

Recommended testing areas:

* Unit testing
* Controller testing
* Service-layer testing
* API integration testing
* Validation testing

### Functional Testing

Test workflows such as:

```text
Register
   ↓
Login
   ↓
Patient Dashboard
   ↓
Book Appointment
   ↓
View Appointment
   ↓
Staff Updates Status
   ↓
Patient Views Updated Status
```

---

## 📊 Future Enhancements

Planned improvements include:

* Complete MySQL integration
* Full JWT security implementation
* Doctor availability management
* Appointment scheduling calendar
* Email notifications
* Admin analytics dashboard
* Patient support ticket system
* Advanced search and filtering
* Audit logging
* Automated testing
* CI/CD pipeline
* Dockerized frontend and database
* Cloud deployment

---

## 📚 Skills Demonstrated

```text
Java
Spring Boot
React
REST API
SQL
MySQL
JWT
Authentication
Authorization
CRUD
Database Design
API Testing
Input Validation
Git
GitHub
Docker
Maven
Agile / SDLC
```

---

## 💼 Resume Description

**Healthcare Patient Support & Appointment Management System**
*React, Java, Spring Boot, REST API, SQL, JWT, Docker*

* Developed a full-stack healthcare management application using **React and Java Spring Boot** with RESTful APIs for patient, appointment, and support workflows.
* Implemented **authentication, role-based authorization, input validation, CRUD operations, and relational database integration**.
* Designed a modular enterprise-style architecture and containerized backend environment using **Docker**, with API testing through Postman.

---

## ⚠️ Disclaimer

This project is created for **educational and portfolio purposes**.

It does not use real patient data and should not be deployed for handling real Protected Health Information (PHI) without appropriate security, privacy, compliance, and infrastructure controls.

---

## 👨‍💻 Author

**Omkar**

Computer Science | Full Stack Development | Software Engineering

---

## ⭐ Project Goal

The goal of this project is to demonstrate practical knowledge of:

**Frontend Development → Backend Development → REST APIs → Database → Security → Testing → Docker → Enterprise Application Development**
