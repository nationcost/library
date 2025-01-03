# Library Management System
A Java-based library management system for efficiently managing books, members, and lending operations.
Features

Book management (add, remove, search)
Member management (registration, update, delete)
Lending operations (borrow, return, track due dates)
Fine calculation for overdue books
Search functionality by title, author, genre
Admin dashboard for system monitoring

Tech Stack

Java
MySQL Database
Hibernate ORM
Spring Boot Framework
Spring Security
Maven
JUnit for testing

Setup

Clone repository

bashCopygit clone [your-repo-url]

Configure MySQL

propertiesCopyspring.datasource.url=jdbc:mysql://localhost:3306/library_db
spring.datasource.username=root
spring.datasource.password=your_password

Run application

bashCopymvn spring-boot:run
API Endpoints
CopyPOST /api/books - Add new book
GET /api/books - List all books
POST /api/members - Register member
PUT /api/loans/{id} - Process loan
Testing
Run tests:
bashCopymvn test
Database Schema

Books (id, title, author, isbn, status)
Members (id, name, email, status)
Loans (id, book_id, member_id, due_date)

Contributors
Tanmay and Team

License
MIT License
