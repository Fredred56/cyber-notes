# Web Basics (HTTP / HTTPS)

## Core concepts
- HTTP = protocol for web communication
- HTTPS = HTTP + TLS encryption
- Client (browser) ↔ Server (web app)
- URL structure:
  - scheme: https
  - host: example.com
  - path: /admin
  - query: ?id=1
  - fragment: #section

---

## HTTP Request anatomy
**Request line**
- Method + Path + Version

**Headers**
- Host, User-Agent, Cookie, Authorization, Content-Type

**Body**
- Used mainly in POST/PUT requests

Example:
```http
GET /login HTTP/1.1
Host: example.com
User-Agent: Firefox
Cookie: session=abc123
```
## 2) HTTP Response anatomy
* Status code + headers + body
Common status codes:
* 200 OK
* 301/302 Redirect
* 401 Unauthorized
* 403 Forbidden
* 404 Not Found
* 500 Server Error
## Example:
```Http
HTTP/1.1 200 OK
Content-Type: text/html
Set-Cookie: session=xyz
```
## 3) HTTP Methods
* GET = request data
* POST = send data (forms, login)
* PUT/PATCH = UPDATE
* DELETE = delete resource
* OPTIONS = check allowed methods
## 4) Cookies & Sessions
* Cookies are stored in browser and sent with each request
* Sessions identify the user
* Important cookies flags:
  - HttpOnly (protects from JS access)
  - Secure (only sent over HTTPS)
  - SameSite (helps protect from CSRF)
## 5) Authentication vs Authorization
* Authentication = who you are (login)
* Authorization = what you can access (permissions/roles)
## 6) Useful recon checklist
* Check website manually (click everything)
* View source code
* robots.txt
* sitemap.xml
* Response headers
* Cookies
* Hidden parameters (URLs, forms)
## 7) Bassic Tools
* Browser DevTools (Networks tab)
* Burp Suite (proxy, intercept)
* curl
## Curl examples:
```bash
curl -l http://<ip>
curl http://<ip>/robots.txt
curl -X POST -d "username=admin&password=admin"
http://<ip>/login
```
## 8) Mini checklist (daily)
* [] Read one web concept (HTTP, cookies, auth)
* [] Practice Burp basics (intercept + repeater)
* [] Save notes in GitHub
