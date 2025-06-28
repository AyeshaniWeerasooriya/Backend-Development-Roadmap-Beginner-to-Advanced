# 🚀 05 - HTTP Status Codes

## ✍️ What is a Status Code?

Every time a server responds to a client’s request, it sends back a status code — a 3-digit number — that tells the client what happened with the request.
It’s part of the status line in an HTTP response.

![image](https://github.com/user-attachments/assets/afbc8293-3d86-417a-8a44-f495505995af)

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


