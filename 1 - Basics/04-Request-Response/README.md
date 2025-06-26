# 🚀 04 – Requests & Responses

## ✍️ What Are Requests and Responses?

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


### 🧪 Example of a JSON Response





