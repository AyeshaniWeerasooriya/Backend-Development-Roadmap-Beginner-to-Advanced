# 🚀 05 - HTTP Status Codes

## ✍️ What is a Status Code?

Every time a server responds to a client’s request, it sends back a status code. It's a 3-digit number. That tells the client what happened with the request.
It’s part of the status line in an HTTP response.

<p align="center">
  <img src="https://github.com/user-attachments/assets/afbc8293-3d86-417a-8a44-f495505995af" alt="status code" style="width:450px;"/>
</p>


---

## ✍️ Why Status Codes Matter

- Help developers debug requests and responses

- Let the client know what to expect (success, error, redirect, etc.)

- Critical for frontend-backend coordination and API development

- Used in tools like Postman, browser dev tools, and backend logs


---

## ✍️ Categories of HTTP Status Codes

Status codes are grouped by their first digit.

<table >
  <tr>
    <td width="20%" align="center"><b>Code Range</b></td>
    <td width="20%" align="center"><b>Category</b></td>
    <td width="60%" align="center"><b>Meaning</b></td>
    
  </tr>
  <tr>
    <td align="center">1xx</td>
    <td>
      Informational
    </td>
    <td>The request was received, and the server is still processing it</td>
  </tr>
  <tr>
    <td align="center">2xx</td>
    <td>Success</td>
    <td>The request was successful — the server processed it correctly and is sending a proper response</td>
  </tr>
  <tr>
    <td align="center">3xx</td>
    <td>Redirection</td>
    <td>The resource has moved, and the client may need to look elsewhere or follow a redirect to get it</td>
  </tr>
  <tr>
    <td align="center">4xx</td>
    <td>Client Errors</td>
    <td>The request has a problem — usually because something is wrong on the client’s side (bad data, missing permissions, wrong URL, etc.).</td>
  </tr>
   <tr>
    <td align="center">5xx</td>
    <td>Server Errors</td>
    <td>The server itself failed to handle a valid request. It’s not client's fault — something broke on the backend.</td>
  </tr>
</table>

</br>

---

## ✍️ Common HTTP Status Codes With Examples

These are the most frequently used status codes we'll encounter when building or testing web applications.

### 🔹 200 OK

The request was successful. The server returns the requested data.

_Example Response_

<pre>
    HTTP/1.1 200 OK
    Content-Type: application/json

    {
      "message": "User profile loaded successfully"
    }
</pre>

<br>

### 🔹 201 Created

Used when a new resource is successfully created, often after a POST request.

_Example Response_

<pre>
  HTTP/1.1 201 Created
  Content-Type: application/json

  {
    "message": "New product added",
    "productId": 101
  }

</pre>

<br>

### 🔹 204 No Content

Request was successful, but there’s no data to return. Common in DELETE or PUT.

_Example Response_

<pre>
  HTTP/1.1 204 No Content
</pre>

<br>

### 🔹 301 Moved Permanently

The requested resource has been permanently moved to a new URL.

_Example Response_

<pre>
  HTTP/1.1 301 Moved Permanently
  Location: https://new-site.com/page
</pre>

<br>

### 🔹 302 Found

Temporary redirect. The resource is at a different URL, but just for now.

_Example Response_

<pre>
  HTTP/1.1 302 Found
  Location: https://example.com/login
</pre>

<br>

### 🔹 304 Not Modified

Used with caching. It means the resource hasn’t changed since last time. It use our cached version.

_Example Response_

<pre>
  HTTP/1.1 304 Not Modified
</pre>

<br>

### 🔹 400 Bad Request

The request is invalid or badly formed. The server doesn’t understand it.

_Example Response_

<pre>
  
  HTTP/1.1 400 Bad Request
  Content-Type: application/json

  {
    "error": "Missing required field: email"
  }
  
</pre>

<br>

### 🔹 401 Unauthorized

The client is not authenticated. Usually means a login token or credentials are missing/invalid.

_Example Response_

<pre>
  HTTP/1.1 401 Unauthorized
  Content-Type: application/json

  {
    "error": "Access denied. Please log in."
  }

</pre>

<br>

### 🔹 403 Forbidden

The client is authenticated but not allowed to access the requested resource.

_Example Response_

<pre>
  HTTP/1.1 403 Forbidden
  Content-Type: application/json

  {
    "error": "You do not have permission to access this resource"
  }

</pre>

<br>

### 🔹 404 Not Found

The requested URL or resource doesn’t exist on the server.

_Example Response_

<pre>
  HTTP/1.1 404 Not Found
  Content-Type: application/json

  {
    "error": "User not found"
  }

</pre>

<br>

### 🔹 405 Method Not Allowed

The server supports the resource but not with the method used (e.g., sending POST to a read-only endpoint).

_Example Response_

<pre>
  HTTP/1.1 405 Method Not Allowed
  Allow: GET, PUT
</pre>

<br>

### 🔹 500 Internal Server Error

Something went wrong on the server.

_Example Response_

<pre>
  HTTP/1.1 500 Internal Server Error
  Content-Type: application/json

  {
    "error": "Oops! Something broke on our end"
  }

</pre>

<dr>

### 🔹 502 Bad Gateway

Server received an invalid response from another server it was trying to access.

_Example Response_

<pre>
  HTTP/1.1 502 Bad Gateway
</pre>

<br>

### 🔹 503 Service Unavailable

Server is down. It's maybe for maintenance or overload. Try again later.

_Example Response_

<pre>
  HTTP/1.1 503 Service Unavailable
  Retry-After: 120
</pre>

<br>

### 🔹 504 Gateway Timeout

A server acting as a gateway didn’t get a response in time from the upstream server.

_Example Response_

<pre>
  HTTP/1.1 504 Gateway Timeout
</pre>

<br>


---
## ✍️ Final Thoughts

- Status codes are like traffic lights for web communication.

- Every response carries a code that informs success, failure, or next steps.

- Understanding them helps in debugging, logging, and writing cleaner APIs.

---
</br>

**UP NEXT**: Rest API
