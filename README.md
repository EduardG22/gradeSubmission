# Grade Submission 
## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#tech)
- [Usage](#usage)
## <a name="overview"></a> Overview
The Grade Submission System is a Spring Boot application designed to facilitate the management of grades for courses and students. It provides functionalities for creating, updating, deleting, and retrieving grades, as well as managing courses, students, It also provides APIs for user registration, login, and authentication using JWT (JSON Web Tokens).
## <a name="features"></a> Features
- User Registration: Users can register with the system by providing a username and password.
- User Login: Registered users can log in to the system using their credentials.
- Authentication: Upon successful login, users receive a JWT token, which they can use to authenticate subsequent requests to protected endpoints.
- Course Management: Admin users can create, update, delete, and retrieve information about courses.
- Grade Submission: Users can submit grades for students enrolled in courses.
- Student Management: Admin users can manage student information, including name, birth date, and enrollment status.
#### Class Diagram
![Diagram for Grade Submission](https://github.com/EduardG22/gradeSubmission/assets/121970200/03758ac4-e79d-434a-a222-7d17e351b579)
## <a name="tech"></a> Technologies Used
- Java
- Spring Boot 3
- Spring Security 6
- JWT Token Authentication
- Spring Data JPA
- OpenAPI and Swagger UI Documentation
## <a name="usage"></a>Usage
#### Register User:
- Use the localhost:8080/user/register endpoint to register a new user. Provide a username and password in the request body.
#### Login User:
- Use the localhost:8080/authenticate endpoint to log in to the system. Provide your username and password in the request body. Upon successful authentication, you will receive a JWT token in the response header.
#### Authentication:
- Include the JWT token in the Authorization header of subsequent requests to protected endpoints. The token should be prefixed with "Bearer". Example: Authorization: Bearer <your_token>.
#### Course Management:
- Admin users can perform CRUD operations on courses.
#### Grade Submision:
- Authenticated users can submit grades for students enrolled in courses.
#### Student Management:
- Admin users can manage student information.
## Getting Started:
- Clone the repository: git clone https://github.com/EduardG22/gradeSubmission.git
- Set up your database and configure the application.properties file with your database credentials.
- Build and run the application using Maven: mvn spring-boot:run
## Contact
- For any inquiries or feedback, please contact popaeduard22@gmail.com
