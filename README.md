# Hospital Management System

A backend application built using **Java, Spring Boot, and PostgreSQL** to manage hospital-related patient data.

## Tech Stack

- **Backend:** Java, Spring Boot
- **Database:** PostgreSQL
- **ORM:** Spring Data JPA, Hibernate
- **Build Tool:** Maven
- **Testing:** JUnit

## Project Structure

```text
hospitalManagement/
│
├── src/
│   ├── main/
│   │   ├── java/com/rutvika/project/hospitalManagement/
│   │   │   ├── entity/
│   │   │   │   └── Patient.java
│   │   │   ├── repository/
│   │   │   │   └── PatientRepository.java
│   │   │   ├── service/
│   │   │   │   └── PatientService.java
│   │   │   └── HospitalManagementApplication.java
│   │   │
│   │   └── resources/
│   │       ├── application.properties
│   │       └── data.sql
│   │
│   └── test/
│       └── java/
│
├── pom.xml
└── README.md
```

## Architecture

The application follows a layered architecture:

- **Entity Layer:** Defines the Patient data model.
- **Repository Layer:** Handles database operations using Spring Data JPA.
- **Service Layer:** Contains business logic.
- **Configuration:** Manages application and database configuration.

## Prerequisites

- Java JDK
- Maven
- PostgreSQL
- IntelliJ IDEA (recommended)

## Database Configuration

1. Create a PostgreSQL database named `hospitalDB`.
2. Configure the following environment variables:

```text
DB_URL=jdbc:postgresql://localhost:5432/hospitalDB
DB_USERNAME=postgres
DB_PASSWORD=your_password
```

## Run the Application

Clone the repository:

```bash
git clone https://github.com/rutvika09/hospitalManagement.git
```

Navigate to the project directory:

```bash
cd hospitalManagement
```

Run the application using Maven Wrapper on Windows:

```bash
.\mvnw.cmd spring-boot:run
```

## Run Tests

```bash
.\mvnw.cmd test
```

## Author

**Rutvika Lavangade**

GitHub: https://github.com/rutvika09