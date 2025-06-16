# 🚀 03 - HTTP & HTTPS Requests

## ✍️ What is HTTP & HTTPS

HTTP stands for **HyperText Transfer Protocol**

- This protocol used to structure and transfer data across the web. It defines how messages are formatted and transmitted between clients (like web browsers) and servers.

HTTPS stands for **HyperText Transfer Protocol Secure**

- It performs the same role as HTTP but adds a layer of security through SSL/TLS encryption, protecting sensitive data from being read or altered during transmission.

---

### **HTTP/ HTTPS like a waiter in a Restaurant.**

<p align="center">
  <img src="https://github.com/user-attachments/assets/9c927c3a-9458-476a-bc81-29223379d948" alt="HTTP as a waiter" style="width:60%;" />
</p>

At a restaurant, the customer sits at the table and places an order. The waiter receives the order and takes it to the kitchen. In the kitchen, the chef carefully prepares the requested meal. Once it's ready, the waiter picks it up and returns to the table with the finished dish.

On the web, the process is quite similar. A browser sends a request, much like placing an order. **The protocol, acting as the waiter → whether HTTP or HTTPS, carries that request to the server**, which works like the kitchen. The server processes the request and prepares the appropriate content. Then, **the protocol brings the final result → the webpage back to the browser** and ready to be displayed.



---


## ✍️ Importance of HTTPS

HTTPS is more than just a secure version of HTTP. It provides essential benefits like,

- Encrypts data to protect personal information like passwords and card details.
  
- Prevents attackers from tampering with data during transmission.
     
- Verifies website identity, helping users avoid fake or malicious sites.
 
- Automatically used by modern browsers when visiting known secure websites.
   
---

## ✍️ Role of TCP

TCP stands for **Transmission Control Protocol**. 
- It's the reliable transport layer between browser and the server.
- TCP ensures that all parts of the communication are delivered safely, in the correct order, and without corruption. 
- TCP handles the mechanics of sending data:
  
   🔸 Breaks data into smaller packets

   🔸 Sends them individually

   🔸 Reassembles them correctly at the destination

   🔸 Detects and resends lost or corrupted packets

It’s like mailing pages of a book in separate envelopes. TCP ensures all the pages arrive, are in the right order, and nothing is missing.

---

## ✍️ How HTTP/HTTPS Works

Imagine visiting a website like `www.udemy.com`. On the surface, it looks like a simple action. But in behind, several important steps are happening.

### 1. Typing the URL
   A user enters `www.udemy.com` in the browser’s address bar.
   
</br>

### 2. Choosing the Protocol
   The browser detects that the site supports HTTPS and adds it in the background.
    
  <pre>
     https://www.udemy.com
  </pre>

</br>

### 3. Domain to IP Conversion (DNS Lookup)
   The browser asks the **Domain Name System (DNS)** to find the IP address associated with the domain.
   
   <pre>
     www.udemy.com → 104.18.199.63
   </pre>

   </br>

### 4. TCP Connection Setup
   A **TCP (Transmission Control Protocol)** connection is established between the browser and the server. 

</br>

### 5. HTTP GET Request
   The browser sends a request to retrieve the homepage.

   <pre>
      GET / HTTP/1.1  
      Host: www.udemy.com
   </pre>

   </br>

### 6. Server Response
   The server processes the request and returns an HTTP response.

   <pre>
      HTTP/1.1 200 OK  
      Content-Type: text/html  
      <html>...</html>

   </pre>

   </br>
   
### 7. Rendering the Webpage
   The browser receives the response and renders the content for viewing.

---

## ✍️ HTTP Methods – Types of Requests

Different HTTP methods serve different purposes when interacting with a server.

</br>

<table>
  <tr>
    <td align="center"><b>Method</b></td>
    <td  align="center"><b>Description</b></td>
  </tr>
    <tr>
    <td>GET</td>
    <td>Request to retrieve a resource</td>
  </tr>
    <tr>
    <td>POST</td>
    <td>Request to create a new resource</td>
  </tr>
    <tr>
    <td>PUT</td>
    <td>Request to update or replace a resource</td>
  </tr>
    <tr>
    <td>DELETE</td>
    <td>Request to remove a resource</td>
  </tr>
</table>

</br>

These methods are the building blocks of client-server communication on the web.
  
---

## ✍️ Final Thoughts

- HTTP is the core language that enables web browsers and servers to communicate.
- TCP ensures that this conversation is delivered accurately and safely.
- HTTPS adds a much-needed layer of trust and security, making the web safer for users and developers alike.
- HTTP methods like GET, POST, PUT, and DELETE define the actions a client can request from a server. They form the foundation for web interactions, from viewing a page to submitting data and updating content and it's making them essential tools in every backend developer’s toolkit.

---
</br>

**UP NEXT**: Requests & Responses







