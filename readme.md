Spring Boot Book Management System
-Overview
This project is a RESTful API developed with Spring Boot for managing a library's book collection. It demonstrates the ability to create scalable and well-structured backend systems using Spring Boot, Spring Data JPA, and H2 Database. The API allows for basic CRUD (Create, Read, Update, Delete) operations on books.

-Features
*List all books
*Retrieve a single book by ID
*Add a new book
*Update an existing book
*Delete a book

-Technologies Used
*Spring Boot
*Spring Data JPA
*H2 Database
*Maven


-Repository
git https://github.com/omerkolsuz/library-management-system.git
cd library-management-system
mvn install
-Running
mvn spring-boot:run

-Server
localhost:8080

-Usage
*List all books
GET /api/books

*Get a single book by ID
GET /api/books/{id}

*Add a new book
POST /api/books
{
  "title": "Book Title",
  "author": "Author Name",
  "isbn": "ISBN"
}

*Update an existing book
PUT /api/books/{id}
{
  "title": "New Book Title",
  "author": "New Author Name",
  "isbn": "New ISBN"
}

*Delete a book
DELETE /api/books/{id}

*Example 
curl -X POST -H "Content-Type: application/json" -d '{"title":"Exempel","author":"Ömer Kolsuz","publicationYear":2023}' http://localhost:8080/api/books



