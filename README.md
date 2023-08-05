# Employee-Management-System
Employee Management System Web App
Project Description:

Implemented the following features in this project:

    List Employee Feature

    Add Employee Feature

    Update Employee Feature

    Delete Employee Feature

    Pagination Feature

    Sorting Feature

    Login Feature

    Registration Feature

    Logout Feature

Tools and technologies used:

    Java 8+
    Spring Boot
    Spring Data JPA ( Hibernate)
    Spring Security
    MySQL
    Eclipse STS
    Maven
    Tomcat
    Thymeleaf

    Create Spring Boot Project

Project Name: employee-management-webapp

Project Type: Maven

dependencies: Spring Web, Spring Data JPA, MySQL Driver, Spring Security, Thymeleaf, Dev Tools

    Maven Dependencies

    Configure MySQL Database

Spring Boot tries to auto-configure a DataSource if spring-data-jpa dependency is in the classpath by reading the database configuration from the application.properties file.

So, we just have to add the configuration, and Spring Boot will take care of the rest.

Open the application.properties file and add the following properties to it.

    Create Models

Created models or entities for the Employee Management System application.

    Create Repository or DAO Layer

Created JPA repositories to access data from the database.

    Create Service Layer

    Create DTO - UserRegistrationDto

    Spring Security Configuration

If Spring Security is on the classpath, Spring Boot automatically secures all HTTP endpoints with “basic” authentication but we need form-based authentication so we have configured the same in the above code.

The SecurityConfiguration class is annotated with @EnableWebSecurity to enable Spring Security’s web security support and provide the Spring MVC integration. It also extends WebSecurityConfigurerAdapter and overrides a couple of its methods to set some specifics of the web security configuration.

The configure(HttpSecurity) method defines which URL paths should be secured and which should not. Specifically, the / and /home paths are configured to not require any authentication. All other paths must be authenticated.

9.Create Controller Layer

Implemented a controller layer, for that created a package called controller inside base package.

    View Layer

Implemented this using various HTML resources and templates.

    Run application
