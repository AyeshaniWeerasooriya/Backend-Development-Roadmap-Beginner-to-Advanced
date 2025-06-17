#  Requests & Responses 

✅ 2. Request & Response Headers
Headers carry metadata about the request/response. Examples:

## Request Headers:
User-Agent: Info about the browser or device

Accept: What kind of content is expected (HTML, JSON, etc.)

Authorization: Contains tokens or login credentials




## Response Headers:
Content-Type: The format of the response (e.g., text/html, application/json)

Set-Cookie: Stores data in the browser

Cache-Control: Tells the browser how to cache the response

🔹 Helpful to explain that not all communication is in the visible body — headers matter too.



🔄 Requests and Responses
This chapter can explore:

✍️ What is an HTTP Request?
Structure of a request:

Method (GET, POST, etc.)

URL

Headers (like Content-Type, Authorization)

Body (mainly for POST/PUT)

Example:

http
Copy
Edit
POST /login HTTP/1.1
Host: example.com
Content-Type: application/json

{
  "username": "john",
  "password": "12345"
}
