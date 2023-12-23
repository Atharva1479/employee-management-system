# Employee Management System

The Employee Management System is a web application built with Spring Boot, Spring Data JPA, Thymeleaf, and Bootstrap. It provides a user-friendly interface for managing employee records with features such as adding, editing, and deleting employees. The application supports paginated display for easy navigation through employee records.

## Features

- **Add Employee:** Add new employees to the system with their details such as name, address, email, phone number, and salary.

- **Edit Employee:** Modify existing employee details, including name, address, email, phone number, and salary.

- **Delete Employee:** Remove employee records from the system.

- **Paginated Display:** View employee records in a paginated format for better organization.

## Technologies Used

- **Spring Boot:** Framework for building Java-based enterprise applications.

- **Spring Data JPA:** Simplifies data access using the Java Persistence API (JPA).

- **Thymeleaf:** Server-side Java template engine for web and standalone environments.

- **Bootstrap:** Front-end framework for designing responsive and visually appealing web pages.

- **MySQL:** Relational database management system.

## Setup

1. **Clone the Repository:**

## Database Configuration

The Employee Management System uses MySQL as its database. Follow these steps to configure the database:

1. **Create MySQL Database:**

   - Open your MySQL database management tool (e.g., MySQL Workbench).
   - Create a new database named `emp`.

2. **Update Application Properties:**

   - Open the `src/main/resources/application.properties` file.
   - Update the following properties with your MySQL database credentials:

     ```properties
     spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
     spring.datasource.url=jdbc:mysql://localhost:3306/emp
     spring.datasource.username=your-mysql-username
     spring.datasource.password=your-mysql-password
     ```

     Replace `your-mysql-username` and `your-mysql-password` with your MySQL username and password.

3. **Run the Application:**

   - After configuring the database, run the application using the following command:
     ./mvnw spring-boot:run

   - The application will connect to the MySQL database based on the provided configuration.

4. **Access the Application:**

   - Open a web browser and navigate to `http://localhost:8080` to access the Employee Management System.

Now, your application is configured to use the MySQL database for storing and retrieving employee records.

