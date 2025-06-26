# 🚀 04 – Requests & Responses

## ✍️ What Are Requests and Responses?

Every interaction between a client (like a browser or mobile app) and a server is built around a cycle called the **request-response model**.

- The **client sends a request** asking for something (a page, data, or an action).
- The **server processes it** and sends back a response, usually with the requested data or a message.

This cycle is the **foundation of backend communication** on the web.

---

## Ordering in a Restaurant

Imagine we're at a restaurant:

- we (the **client**) place an order (a **request**) through a waiter.
- The waiter (like the **HTTP/HTTPS protocol**) delivers it to the kitchen (the **server**).
- The kitchen prepares the dish and sends it back via the waiter (a **response**).



---

## 📨 The Request – What the Client Sends

A typical HTTP request contains:

| Part        | Description                                                 |
|-------------|-------------------------------------------------------------|
| **Method**  | The action being requested (`GET`, `POST`, `PUT`, `DELETE`) |
| **URL**     | The resource being requested (e.g., `/login`, `/products`)  |
| **Headers** | Extra info like content type, auth tokens, etc.             |
| **Body**    | Data sent with the request (used with `POST`, `PUT`)        |

### 🧪 Example of a POST Request

