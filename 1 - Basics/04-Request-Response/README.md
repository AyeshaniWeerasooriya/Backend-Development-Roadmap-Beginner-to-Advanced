# 🚀 04 – Requests & Responses

## ✍️ What Are Requests and Responses

Every interaction between a client (like a browser or mobile app) and a server is built around a cycle called the **request-response model**.

- The **client sends a request** asking for something (a page, data, or an action).
- The **server processes it** and sends back a response, usually with the requested data or a message.

This cycle is the **foundation of backend communication** on the web.

---

### Ordering a meal in a Restaurant

Imagine we're at a restaurant:

- we (the **client**) place an order (a **request**) through a waiter.
- The waiter (like the **HTTP/HTTPS protocol**) delivers it to the kitchen (the **server**).
- The kitchen prepares the dish and sends it back via the waiter (a **response**).

  <p align="center">
  <img src="https://github.com/user-attachments/assets/f07a852d-fdf8-4709-8f42-466663c5e8e7" alt="HTTP as a waiter" style="width:60%;" />
</p>


---

## ✍️ The Request – What the Client Sends

A typical HTTP **request** contains below things.

</br>

<table>
  <tr>
    <td align="center"><b>Part</b></td>
    <td  align="center"><b>Description</b></td>
  </tr>
    <tr>
    <td>Method</td>
    <td>
      The action being requested ( GET, POST, PUT, DELETE ) 
    </td>
  </tr>
    <tr>
    <td>URL / Path</td>
    <td>The resource being requested (e.g., /login, /products)</td>
  </tr>
    <tr>
    <td>Headers</td>
    <td>Extra information like content type, authorization tokens, etc.</td>
  </tr>
    <tr>
    <td>Body</td>
    <td>The data sent with the request (used with POST, PUT)</td>
  </tr>
</table>

</br>

###  Example 

This request sends a user's login credentials (`username` and `password`) to the server at the `/login` path using the HTTP/1.1 protocol, asking the server to authenticate the user.

<p align="left">
  <img src="https://github.com/user-attachments/assets/ef932f8b-2172-418a-be0f-d24f19eaf17b" alt="HTTP as a waiter" style="width:60%;" />
</p>



---

## ✍️ The Response – What the Server Sends Back

The server responds with a structured message.

</br>

<table>
  <tr>
    <td align="center"><b>Part</b></td>
    <td  align="center"><b>Description</b></td>
  </tr>
    <tr>
    <td>Status Line</td>
    <td>
      Includes the HTTP version and status code
    </td>
  </tr>
    <tr>
    <td>Headers</td>
    <td>Metadata about the response</td>
  </tr>
    <tr>
    <td>Body</td>
    <td>The actual data/content being returned (HTML, JSON)</td>
  </tr>
</table>

</br>


###  Example

This response uses HTTP/1.1 to inform the client that the login was successful (status 200), and it returns a JSON body containing a success message and an authentication token.

<p align="left">
  <img src="https://github.com/user-attachments/assets/be75fd99-06a2-42ea-928a-83d55353cb8d" alt="HTTP as a waiter" style="width:60%;" />
</p>



---

## ✍️ Request & Response Headers

Headers are key-value pairs that carry **metadata** about the request or response. They’re invisible to users but crucial for functionality.

### ✅ Request Headers

| Header            | Purpose                                               |
|------------------|--------------------------------------------------------|
| `User-Agent`      | Identifies the browser or device                      |
| `Accept`          | Expected content type (`application/json`, `text/html`) |
| `Authorization`   | Credentials like tokens or API keys                   |
| `Content-Type`    | Format of request body (`application/json`, etc.)     |


<br>


### ✅ Response Headers

| Header                   | Purpose                                           |
|--------------------------|--------------------------------------------------|
| `Content-Type`           | Format of the returned data                      |
| `Set-Cookie`             | Stores small data in the browser                 |
| `Cache-Control`          | Controls how browser should cache the response   |
| `Access-Control-Allow-Origin` | Controls cross-origin access (CORS)       |

---

## ✍️ Why Headers Matter

- They enable security, formatting, and proper communication.
- Without headers, much of the web wouldn’t function correctly.

---

## ✍️ Final Thoughts

- The request-response cycle powers all web communication.

- Headers play a behind-the-scenes role in security and formatting.

- HTTP methods like GET, POST, PUT, and DELETE define the core actions in APIs.

- Mastering this cycle prepares you to build real-world backend systems and REST APIs.

---

</br>

**UP NEXT**: Status codes




