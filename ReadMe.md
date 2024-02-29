# Bookstore Web Application (Spring Boot)

This is a simple bookstore web application developed using Spring Boot. It provides RESTful endpoints to perform CRUD operations on a collection of books stored in a MySQL database.

## Features

- View a list of books
- Add a new book
- Get details of a book by ID
- Update an existing book
- Delete a book

## Technologies Used

- Spring Boot
- Spring Data JPA
- MySQL
- Maven
- RESTful API

## Project Structure

- `src/main/java`: Contains Java source files for controllers, models, and repositories.
- `src/main/resources`: Contains `application.properties` for configuration.
- `pom.xml`: Maven project configuration file.

## Prerequisites

Before running the application, ensure you have the following installed:

- Java Development Kit (JDK)
- MySQL Database Server
- Apache Maven

## Configuration

1. **Database Configuration**: Modify the database connection settings in `application.properties` to match your MySQL database configuration.

    ```properties
    spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
    spring.datasource.url=jdbc:mysql://localhost:3306/booksdb
    spring.datasource.username=your_username
    spring.datasource.password=your_password
    ```

   Replace `your_username` and `your_password` with your MySQL database username and password.

2. **Create Database**: Create a MySQL database named `booksdb`.

3. **Build Project**: Build the project using Maven:

    ```bash
    mvn clean install
    ```

4. **Run the Application**: Run the Spring Boot application using Maven:

    ```bash
    mvn spring-boot:run
    ```

## Usage

1. **View Book List**: Access the list of books by sending a GET request to `/books`.

2. **Add New Book**: Add a new book by sending a POST request to `/books` with JSON payload containing book details.

3. **Get Book by ID**: Get details of a book by sending a GET request to `/books/{id}` where `{id}` is the book's ID.

4. **Update Book**: Update an existing book by sending a PUT request to `/books/{id}` with JSON payload containing updated book details.

5. **Delete Book**: Delete a book by sending a DELETE request to `/books/{id}` where `{id}` is the book's ID.

## Development

To contribute to the development of this project, follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push your changes to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

Harshal Patil

## Acknowledgements

- [Spring Boot](https://spring.io/projects/spring-boot)
- [Spring Data JPA](https://spring.io/projects/spring-data-jpa)
- [MySQL](https://www.mysql.com/)
- [Apache Maven](https://maven.apache.org/)
