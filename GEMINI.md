# Project Overview

This project is a simplified Instagram clone built with Spring Boot. It allows users to sign up, log in, create posts, comment on posts, and like posts.

**Main Technologies:**

*   **Backend:** Spring Boot, Spring Security, Spring Data JPA
*   **Frontend:** Thymeleaf
*   **Database:** MySQL
*   **Build Tool:** Gradle

**Architecture:**

The application follows a standard Model-View-Controller (MVC) architecture.

*   **Controllers:** Handle HTTP requests and map them to specific methods.
*   **Services:** Contain the business logic of the application.
*   **Repositories:** Interact with the database using Spring Data JPA.
*   **Entities:** Represent the data model of the application.
*   **DTOs:** Transfer data between the client and the server.

# Building and Running

**Prerequisites:**

*   Java 21
*   MySQL database

**Build:**

```bash
./gradlew build
```

**Run:**

```bash
./gradlew bootRun
```

The application will be accessible at `http://localhost:8080`.

**Database Configuration:**

The database connection properties are configured in `src/main/resources/application.properties`. You need to create a MySQL database and update the following properties:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/your-database
spring.datasource.username=your-username
spring.datasource.password=your-password
```

# Development Conventions

*   **Code Style:** The project uses the standard Java code style.
*   **Testing:** The project uses JUnit 5 for testing.
*   **Authentication:** Authentication is handled by Spring Security.
*   **View Layer:** Thymeleaf is used for the view layer.
