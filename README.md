# Library Management System API

This project is a **Library Management System API** that allows users to manage a collection of books. It provides CRUD operations (Create, Read, Update, Delete) and a detailed view for individual books. The API is designed for testing with **Insomnia**.

---

## Features

- **Create**: Add a new book to the library.
- **Read**: Retrieve all books or a specific book by ID.
- **Update**: Edit details of an existing book.
- **Delete**: Remove a book from the library.
- **Detail View**: Get detailed information about a specific book.

---

## Technology Stack

- **Backend**: Node.js
- **Database**: SQL (using a relational database)
- **API Testing Tool**: Insomnia

---

## API Endpoints

### Base URL
`http://localhost:<PORT>` (Replace `<PORT>` with your server's port)

### Endpoints

#### 1. **Get All Books**
- **Method**: `GET`
- **Endpoint**: `/books`
- **Description**: Retrieves a list of all books in the library.
- **Response Example**:
  ```json
  [
    {
      "id": 1,
      "title": "To Kill a Mockingbird",
      "author": "Harper Lee",
      "year": 1960,
      "genre": "Fiction"
    },
  ]
#### 2. **Get Book Detail**
- **Method**: `GET`
- **Endpoint**: `/books/{id}`
- **Description**: Retrieves the details of a specific book by its ID.
- **Response Example**:
  ```json
  [
    {
      "id": 1,
      "title": "To Kill a Mockingbird",
      "author": "Harper Lee",
      "year": 1960,
      "genre": "Fiction"
    },
  ]
#### 3. **Create a New Book**
- **Method**: `POST`
- **Endpoint**: `/books`
- **Description**: Adds a new book to the library.
- **Request Example**:
  ```json
  {
    "title": "1984",
    "author": "George Orwell",
    "year": 1949,
    "genre": "Dystopian"
  }
#### 4. Update Book
- **Method**: `PUT`
- **Endpoint**: `/books/{id}`
- **Description**: Updates the details of an existing book.
- **Request Example**:
  ```json
  {
     "title": "1984",
  "author": "George Orwell",
  "year": 1959,
  "genre": "Dystopian"
  }

#### 5. Delete Book
- **Method**: `DELETE`
- **Endpoint**: `/books/{id}`

## Testing the API with Insomnia  
Once the server is running, you can use Insomnia to test the following API endpoints:

- **GET /book**: Retrieve a list of all books.
- **GET /book/:id**: Retrieve a specific book by its ID.
- **POST /book**: Create a new book by sending a JSON body.
- **PUT /book/:id**: Update an existing book by sending a JSON body.
- **DELETE /book/:id**: Delete a specific book.





