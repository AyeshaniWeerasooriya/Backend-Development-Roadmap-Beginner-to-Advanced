# 🚀 06 - REST APIs

## ✍️ What is REST API 

- REST stands for **Representational State Transfer.**  It’s an architecture style for designing networked applications.
  A REST API (or RESTful API) is a set of rules that allows clients and servers to communicate over HTTP.

- In simpler terms, a REST API lets different software systems talk to each other using web URLs.

---

## ✍️ Why REST APIs Matter

- Allows communication between frontend and backend

- Helps connect mobile apps, web apps, and servers

- Widely used in modern web development

- Easy to use with tools like Postman, Curl, and Fetch/Axios in JavaScript

---

## ✍️ REST Principles (Key Concepts)

<table> 
  <tr> 
    <td align="center"><b>Principle</b></td> 
    <td align="center"><b>Description</b></td> 
  </tr> 
  <tr> 
    <td>Stateless</td> 
    <td>Each request from client to server must contain all information. The server does not remember previous requests.</td> 
  </tr> 
  <tr> 
    <td>Client-Server</td> 
    <td>Frontend and backend are separated, so they can evolve independently.</td> 
  </tr> 
  <tr> 
    <td>Uniform Interface</td> 
    <td>Resources (data) are identified with URIs like <code>/users</code> or <code>/products/5</code>.</td> 
  </tr> 
  <tr> 
    <td>Cacheable</td> 
    <td>Responses can be cached to improve performance.</td> 
  </tr> 
</table>

---

## ✍️ HTTP Methods in REST

REST APIs use standard HTTP methods to perform actions.

<table>
  <tr>
    <td align="center"><b>Method</b></td>
    <td align="center"><b>Purpose</b></td>
    <td align="center"><b>Example</b></td>
  </tr>
  <tr>
    <td>GET</td>
    <td>Read data</td>
    <td><code>GET /users</code> (Get all users)</td> 
  </tr>
   <tr>
    <td>POST</td>
    <td>Create new data</td>
    <td><code>POST /users</code> (Create a new user)</td> 
  </tr>
   <tr>
    <td>PUT</td>
    <td>Update existing data</td>
    <td><code>PUT /users/1</code> (Update user with ID 1)</td> 
  </tr>
   <tr>
    <td>DELETE</td>
    <td>Remove data</td>
    <td><code>DELETE /users/1</code> (Delete user with ID 1)</td> 
  </tr>
</table>

---

## ✍️ REST API Endpoint Example

Assume we’re building an API for managing books in a library.

<table border="1">
  <thead>
    <tr>
      <th>Action</th>
      <th>HTTP Method</th>
      <th>Endpoint</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Get all books</td>
      <td>GET</td>
      <td><code>/books</code></td>
      <td>Returns a list of books</td>
    </tr>
    <tr>
      <td>Get single book</td>
      <td>GET</td>
      <td><code>/books/10</code></td>
      <td>Get book with ID 10</td>
    </tr>
    <tr>
      <td>Add a book</td>
      <td>POST</td>
      <td><code>/books</code></td>
      <td>Add new book</td>
    </tr>
    <tr>
      <td>Update a book</td>
      <td>PUT</td>
      <td><code>/books/10</code></td>
      <td>Update book with ID 10</td>
    </tr>
    <tr>
      <td>Delete a book</td>
      <td>DELETE</td>
      <td><code>/books/10</code></td>
      <td>Delete book with ID 10</td>
    </tr>
  </tbody>
</table>

---

## ✍️ Sample Request & Response

Create a New Book (POST)
<br>

  **Request**

  <pre>
      POST /books
      Content-Type: application/json
  
      {
        "title": "Atomic Habits",
        "author": "James Clear"
      }
  </pre>

---

  **Response**

  <pre>
      HTTP/1.1 201 Created
      Content-Type: application/json

      {
        "message": "Book created successfully",
        "bookId": 101
      }
  </pre>

---

## ✍️ Tools to Test REST APIs

- Postman

- Insomnia

- Curl (Terminal)

- Thunder Client (VS Code Extension)

---

## ✍️ Final Thoughts

- REST APIs help your app talk to the backend.

- They rely on HTTP methods and status codes.

- Understanding endpoints and methods is key to backend development.

---
</br>
**UP NEXT:** Server Side Frameworks

