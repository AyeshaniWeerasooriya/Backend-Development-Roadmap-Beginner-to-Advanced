# 🚀 HTTP & HTTPS Requests

## ✍️ What is HTTP and HTTPS

HTTP stands for **HyperText Transfer Protocol**

- This protocol used to structure and transfer data across the web. It defines how messages are formatted and transmitted between clients (like web browsers) and servers.

HTTPS stands for **HyperText Transfer Protocol Secure**

- It performs the same role as HTTP but adds a layer of security through SSL/TLS encryption, protecting sensitive data from being read or altered during transmission.

---

## ✍️ How HTTP Works

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
   The browser asks the Domain Name System (DNS) to find the IP address associated with the domain.
   
   <pre>
     www.udemy.com → 104.18.199.63
   </pre>

   </br>

### 4. TCP Connection Setup
   A TCP (Transmission Control Protocol) connection is established between the browser and the server. TCP ensures that all parts of the communication are delivered safely, in the correct order, and without corruption.

</br>

### 5. HTTP GET Request


  
