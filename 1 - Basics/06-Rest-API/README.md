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
    <td>GET /users (Get all users)</td> 
  </tr>
   <tr>
    <td>POST</td>
    <td>Create new data</td>
    <td>	POST /users (Create a new user)</td> 
  </tr>
   <tr>
    <td>PUT</td>
    <td>Update existing data</td>
    <td>PUT /users/1 (Update user with ID 1)</td> 
  </tr>
   <tr>
    <td>DELETE</td>
    <td>Remove data</td>
    <td>DELETE /users/1 (Delete user with ID 1)</td> 
  </tr>
</table>

---

