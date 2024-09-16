# Spring Boot CRUD REST API - Book & Account Management

This project is a Spring Boot REST API that performs CRUD (Create, Read, Update, Delete) operations on both **Book** and **Account** entities, demonstrating basic database operations. It is built using Spring Boot, Spring Data JPA, and connects to an **online database hosted on Clever Cloud**. The project follows a layered architecture with models, repositories, services, and controllers.

## Features
- **Create a Book/Account**: Add a new book or account to the database.
- **Get All Books/Accounts**: Retrieve all books or accounts from the database.
- **Get Book/Account by ID**: Retrieve a specific book or account by its ID.
- **Update a Book/Account**: Modify the details of an existing book or account.
- **Delete a Book/Account**: Remove a book or account from the database.

## Technologies Used
- **Spring Boot**: Java-based framework for building web and enterprise applications.
- **Spring Data JPA**: Abstraction over JPA to easily interact with the database.
- **Clever Cloud**: Hosting platform for the online cloud mysql database.
- **Maven-dependency**: Add JSTL dependency for run Jsp pages.

## API Endpoints
- **Book API**:
  - **POST** `/api/books` - Create a new book
  - **GET** `/api/books` - Retrieve all books
  - **GET** `/api/books/{id}` - Retrieve a book by its ID
  - **PUT** `/api/books/{id}` - Update an existing book
  - **DELETE** `/api/books/{id}` - Delete a book
- **Account API**:
  - **POST** `/api/accounts` - Create a new account
  - **GET** `/api/accounts` - Retrieve all accounts
  - **GET** `/api/accounts/{id}` - Retrieve an account by its ID
  - **PUT** `/api/accounts/{id}` - Update an existing account
  - **DELETE** `/api/accounts/{id}` - Delete an account

## Database Configuration
The project is configured to use an online database hosted on **Clever Cloud**. To set up the database connection, update the `application.properties` file with the connection details provided by Clever Cloud:

```properties
# Example Clever Cloud PostgreSQL configuration
spring.datasource.url=jdbc:postgresql://<your-clever-cloud-db-url>/<db-name>
spring.datasource.username=<your-username>
spring.datasource.password=<your-password>
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
```

## How to Run the Project

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/book-account-api-crud.git
   ```

2. **Open the project in Eclipse**:
   - In Eclipse, go to `File > Import > Maven > Existing Maven Projects`.
   - Select the project directory (`book-account-api-crud`), and click `Finish`.

3. **Run the Application**:
   - Locate `SpringRestApiApplication.java` in the `src/main/java` directory.
   - Right-click on the file and select `Run As > Java Application`.

4. **Test the API using Postman**:
   - If you have Postman installed, open it and start performing CRUD operations using the provided API endpoints.
   - **Download Postman** if you haven't yet: [Postman Download](https://www.postman.com/downloads/).

5. **Access the API**:
   - The API will be available at `http://localhost:8080/api/books` and `http://localhost:8080/api/accounts`.

I upload the images for Account entity crud operation image below
![insert](https://github.com/user-attachments/assets/f173cc62-aa84-4cc1-9ba3-ef793dd56e08)
![select](https://github.com/user-attachments/assets/8d1db528-6ba7-475e-94f5-cdadc0acc891)
![search](https://github.com/user-attachments/assets/197ae03f-e8d9-4b54-b06e-1228c17d75eb)
![update](https://github.com/user-attachments/assets/2240519c-3adb-4328-bbe7-029a17f00f20)
![delete](https://github.com/user-attachments/assets/ec117500-1328-4a96-b0bf-6ee91a8d4d8f)

