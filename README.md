# web-devlopment-

## INDEX
- [foundation](#Foundations)
- [HTML](#HTML)
- [CSS](#CSS)
- [JAVASCRIPT](#JavaScript)
- [React.js](#Reactjs)
- [Backend](#Backend)
- [Full Stack Projects](#Full-Stack-Projects)
- [System & Web Concepts](#System-and-Web-Concepts)
- [Interviews Internships](#Interviews-Internships)


---

# Foundations 
- [Computer basics](#Computer-basics)
- [How the web works](#How-the-web-works)
- [Internet DNS HTTP HTTPS](#Internet-DNS-HTTP-HTTPS)
- [What is frontend vs backend](#What-is-frontend-vs-backend)
- [How browsers render HTML/CSS/JS](#How-browsers-render-HTMLCSSJS)


###### Computer basics
---
## 🖥️ Computer Basics

A computer is an **electronic machine** that: Takes **input** , **Processes** data , Produces **output** , Stores data
* Input → form data
* Process → JS / backend logic
* Output → webpage

### Hardware Basics 
* CPU (Processor) -> Executes code (JS, Node, backend), Faster CPU → faster builds & servers
* RAM -> Temporary memory ; Stores running programs (VS Code, browser, server) ; Web dev minimum: **8 GB RAM**
* Storage (HDD / SSD) -> Stores OS, code, projects ; SSD preferred (faster load & compile)
* Software Basics
    * System Software -> Operating System (Windows / Linux / macOS) ; Manages files, memory, CPU
* Application Software -> Browser (Chrome, Firefox) ; Code editor (VS Code) ; Git, Node.js

### Operating System Concepts (Important)

* File System -> Files & folders ; Path:
  ```
  C:\Projects\WebApp\index.html
  ```

    * **Extensions:**
        * `.html` → structure
        * `.css` → style
        * `.js` → logic

* Processes
    * Running programs
    * Browser tabs = processes
    * Node server = process

### Internet & Networking Basics 

#### Client–Server Model
```
Browser (Client) → Request → Server
Browser ← Response ← Server
```

#### IP Address
* Unique address of a computer
* Example: `192.168.1.1`

#### Domain Name
* Human-friendly name
* Example: `google.com`

#### DNS
* Converts domain → IP

### Web Basics (Core for Web Dev)

#### What is a Website?
**A collection of :**
* HTML files
* CSS files
* JS files

#### What is a Web App?
* Dynamic website
* Uses backend + database
* Example: Instagram, Amazon

### Programming Basics Required

#### Logic & Flow
* Variables
* Conditions (`if`)
* Loops
* Functions

#### Data Types
* Number
* String
* Boolean
* Array
* Object

### Databases (Basic Idea)

#### What is a Database?
* Stores data permanently

#### Examples
* SQL → MySQL
* NoSQL → MongoDB

### Security Basics (Web Dev Level)
* Password hashing
* HTTPS
* Authentication
* Authorization

### Tools You MUST Know

| Tool    | Purpose            |
| ------- | ------------------ |
| Browser | Run & test website |
| VS Code | Write code         |
| Git     | Version control    |
| GitHub  | Store & share code |
| Node.js | Backend runtime    |

### How Computer Executes Web Code
1. You write code in VS Code
2. Save files on disk
3. Browser reads HTML
4. CSS styles page
5. JS runs logic
6. Backend handles requests
7. Database stores data

---

###### How the web works 
---
## 🌐 How the web works (client–server, HTTP, browser)

##### **things to keep in mind while building web app :** 
* Customer perspective: The app should be simple, pleasing, and solve real user problems.
* Business perspective: It must stay aligned with its product/market fit.
* Engineering perspective: It should be scalable, reliable, and capable of handling high traffic.

#### websites and web applications
A web application is a program that runs in a browser and has three formal characteristics:

* It addresses a particular problem, even if it’s simply finding some information
* It is as interactive as a desktop application
* It works with a Content Management System <br> <br>

Traditionally, a website was just a collection of static pages. A website becomes a web application when it includes both static and dynamic pages. This is why most modern websites today are actually examples of web applications. <br> <br>

When a user makes a request on a website, several parts of the application work together. These include: 
* User interface
* Middleware systems
* Databases
* Servers
* Browser.













### 🌐 Static vs Dynamic Web Pages (clear + exam-ready)

## Static Web Pages

**Definition:** <br>
A static page shows the **same content to every user**. It does **not change automatically**.  <br>

**Technologies used:**  <br>

* HTML
* CSS
* (Optional) basic JavaScript (no backend)  <br>

**How it works:**  <br>

* Browser requests page
* Server sends **already written file**
* No processing on server  <br>

**Example:**  <br>

* Portfolio website * Company info page * Documentation page  <br>

**Features:**  <br>

* Fast loading * Simple to build * No database * Content changes only if developer edits the file  <br>

**Example flow:**  <br>

```
Browser → index.html → Display
```

---

## Dynamic Web Pages  

**Definition:**  <br>
A dynamic page shows **different content based on user, time, or data**.  <br>

**Technologies used:**  <br>

* Frontend: HTML, CSS, JS
* Backend: Node.js, PHP, Java, Python
* Database: MySQL, MongoDB  <br>

**How it works:**  <br>

* Browser sends request
* Server **processes logic**
* Fetches data from database
* Generates page dynamically  <br>

**Example:**  <br>

* Instagram feed * Amazon product page * Login dashboard  <br>

**Features:**  <br>

* Content changes dynamically * Uses database * Personalized output * Slower than static (but powerful)  <br>

**Example flow:**  <br>

```
Browser → Server → Database → Server → Browser
```



### Client–Server Model

The web works on a **client–server architecture**.

**Client**

* User’s device (browser: Chrome, Edge, Firefox)
* Sends requests

**Server**

* Powerful computer
* Stores websites, APIs, databases
* Sends responses

* **Example :**

```
Browser (Client) → Request → Server
Browser ← Response ← Server
```

### Role of the Browser

A **browser** is a client application that:

* Sends HTTP requests
* Receives responses
* Renders web pages

Browser responsibilities:

* Parses **HTML**
* Applies **CSS**
* Executes **JavaScript**
* Displays content to the user

### What Happens When You Enter a URL

Example:

```
https://www.example.com
```

Step-by-step:

1. Browser checks **cache**
2. Browser asks **DNS server** for IP address
3. DNS returns server IP
4. Browser sends **HTTP request** to server
5. Server processes request
6. Server sends **HTTP response**
7. Browser renders the webpage

### HTTP (HyperText Transfer Protocol)

HTTP is a **communication protocol** used on the web.

It defines:

* How requests are sent
* How responses are returned

### HTTP Request

An HTTP request contains:

* **Method** (GET, POST, etc.)
* **URL**
* **Headers**
* **Body** (optional)

Common methods:

| Method | Use         |
| ------ | ----------- |
| GET    | Fetch data  |
| POST   | Send data   |
| PUT    | Update data |
| DELETE | Remove data |

### HTTP Response

An HTTP response contains:

* **Status Code**
* **Headers**
* **Body** (HTML / JSON)

Common status codes:

| Code | Meaning      |
| ---- | ------------ |
| 200  | OK           |
| 404  | Not Found    |
| 500  | Server Error |
| 401  | Unauthorized |

### HTTPS (Secure HTTP)

HTTPS = HTTP + **Encryption (SSL/TLS)**

Provides:

* Secure data transfer
* Data privacy
* Protection from hackers

Used for:

* Login pages
* Payments
* Forms

### Static vs Dynamic Websites

**Static Website**

* Fixed content
* Only HTML + CSS
* Example: Portfolio site

**Dynamic Website**

* Content changes
* Uses backend + database
* Example: Instagram, Amazon

### Backend Role

Backend:

* Handles business logic
* Connects to database
* Sends response to client

Example stack:

* Node.js / Python / Java
* Database: MySQL / MongoDB

### Complete Web Flow (One Line)

```
User → Browser → HTTP Request → Server → Database → HTTP Response → Browser → User
```

---


### Internet DNS HTTP HTTPS

* **Internet**: Global network
* **DNS**: Name → IP converter
* **HTTP**: Data transfer protocol
* **HTTPS**: Secure HTTP

---

## 🌐 Internet

The **Internet** is a global network of interconnected computers and servers.

### Key Points

* Uses **TCP/IP protocol**
* Connects devices worldwide
* Enables services like:

  * Websites
  * Email
  * Cloud services
  * Video streaming

### Basic Flow

```
Device → ISP → Internet → Server → Response
```

---

## 🌍 DNS (Domain Name System)

DNS converts **domain names into IP addresses**.

### Why DNS?

Humans remember:

```
www.google.com
```

Computers understand:

```
142.250.195.46
```

### DNS Working Steps

1. User enters URL
2. Browser checks cache
3. Queries DNS server
4. DNS returns IP address
5. Browser connects to server

📌 DNS = Internet’s **phonebook**

---

## 📡 HTTP (HyperText Transfer Protocol)

HTTP is a **protocol** for communication between client and server.

### Features

* Stateless
* Request–response based
* Fast but **not secure**

### Common HTTP Methods

* GET → Fetch data
* POST → Send data
* PUT → Update data
* DELETE → Remove data

### Common Status Codes

* 200 → OK
* 404 → Not Found
* 500 → Server Error

---

## 🔐 HTTPS (Secure HTTP)

HTTPS = HTTP + **SSL/TLS encryption**

### Why HTTPS?

* Encrypts data
* Prevents data theft
* Ensures data integrity

### Differences: HTTP vs HTTPS

| Feature     | HTTP | HTTPS |
| ----------- | ---- | ----- |
| Security    | ❌ No | ✅ Yes |
| Encryption  | ❌ No | ✅ Yes |
| Port        | 80   | 443   |
| Certificate | ❌ No | ✅ SSL |

---



### What is frontend vs backend

## 🖥️ Frontend (Client Side)

**Frontend** is everything the **user sees and interacts with** in a website or web app.
*  **Examples** -> Buttons, Forms, Text, Images, Layout & design

🔹Technologies
* **HTML** → Structure
* **CSS** → Styling
* **JavaScript** → Interactivity
* Frameworks/Libraries: React, Angular, Vue

🔹 Responsibilities
* UI/UX design
* Responsive layouts
* User interaction handling
* Sending requests to backend

📌 Runs in the **browser**

---

## ⚙️ Backend (Server Side)
**Backend** is everything that happens **behind the scenes**.
* Examples -> User authentication, Database operations, Business logic, APIs

🔹**Technologies**
* Languages : JavaScript (Node.js),  Python, Java, PHP
* Frameworks : Express, Django, Spring Boot
* Databases : MySQL, MongoDB, PostgreSQL

🔹**Responsibilities**
* Process requests
* Handle logic
* Store & retrieve data
* Security & authentication

📌 Runs on the **server**

---

## 🔄 Frontend vs Backend (Table)

| Feature         | Frontend         | Backend          |
| --------------- | ---------------- | ---------------- |
| Runs on         | Browser          | Server           |
| User visible    | ✅ Yes            | ❌ No             |
| Main goal       | UI & interaction | Logic & data     |
| Languages       | HTML, CSS, JS    | JS, Python, Java |
| Database access | ❌ No             | ✅ Yes            |

---

## 🔁 How They Work Together

```
User → Frontend → Backend → Database
                     ↓
                 Response
```

---

#### Simple Analogy
🍽️ **Restaurant**
* Frontend → Menu & waiter
* Backend → Kitchen
* Database → Store room

---

## How browsers render HTML/CSS/JS

When you enter a website URL, the browser follows **multiple internal steps** to show the page on your screen.

### HTML Parsing → DOM Creation
* Browser downloads the **HTML file**
* Reads HTML **top to bottom**
* Converts HTML tags into nodes
* Builds a tree-like structure called **DOM (Document Object Model)**

📌 Example:

```html
<h1>Hello</h1>
<p>World</p>
```

Becomes:

```
Document
 ├── h1
 └── p
```

➡ DOM represents the **structure of the webpage**

---

### CSS Parsing → CSSOM Creation

* Browser downloads **CSS files**
* Parses CSS rules
* Creates **CSSOM (CSS Object Model)**

📌 CSSOM contains:

* Styles
* Selectors
* Inheritance rules
* Specificity & cascading logic

➡ CSSOM represents **how elements should look**

---

### Render Tree Construction

* Browser combines **DOM + CSSOM**
* Builds the **Render Tree**

⚠️ Important:

* Only **visible elements** are included
* Elements like `display: none` are excluded

➡ Render Tree = **What to render + how to render**

---

### Layout (Reflow)

* Browser calculates:

  * Width
  * Height
  * Position of every element
* Based on:

  * Screen size
  * CSS rules
  * Parent–child relationships

📌 Called **Reflow**
📌 Expensive operation (slow if frequent)

---

### Painting

* Browser paints pixels:

  * Text
  * Colors
  * Images
  * Borders
  * Shadows

➡ Each visual layer is drawn on screen

---

### Compositing

* Browser splits page into layers
* GPU combines layers
* Improves performance (used for animations)

---

### JavaScript Execution

* JavaScript runs **after parsing**
* JS can:

  * Change HTML (DOM)
  * Change CSS (CSSOM)
* Causes:

  * Reflow (layout recalculation)
  * Repaint (redrawing)

📌 JS is **blocking by default**

* `async` → loads independently
* `defer` → executes after DOM is ready

---

### Repaint vs Reflow

| Action              | Reflow | Repaint |
| ------------------- | ------ | ------- |
| Change color        | ❌      | ✅       |
| Change width/height | ✅      | ✅       |
| Add/remove element  | ✅      | ✅       |

---

## Complete Flow (Important for Interviews)

**HTML → DOM**
**CSS → CSSOM**
**DOM + CSSOM → Render Tree**
**Render Tree → Layout → Paint → Composite**

---

## Performance Tips

* Avoid frequent DOM changes
* Use `transform` & `opacity` for animations
* Load JS using `defer`
* Minimize reflows

---


# HTML 

- [html roadmap.sh](https://roadmap.sh/html) 
- [Headings tag](#Headings-tag)
- [Paragraph tag](#Paragraph-tag)
- [new line tag](#Break)
- [Horizontal Line](#Horizontal-Line)
- [Comments](#Comments)
- [Images](#Images)

structure of website <br>
HTML (HyperText Markup Language) is the standard markup language used to create and structure web pages.

<img width="814" height="696" alt="image" src="https://github.com/user-attachments/assets/7c9a1ea7-32df-47c4-8778-be7523096245" />

#### boiler plate code 
```html
<!DOCTYPE html>      <--tell browser you are using html 5-->
<html lang="en">         <--root of an html-->
<head>        <--container for meta data -->
    <title>Document</title>      <-- title-->
</head>   
<body>
    <!--body of html , container of all data rendered by browser -->
</body>
</html>
```
* **<html> :** Encloses the entire HTML document, serving as the root element for all HTML content.
* **<head> :** Contains header information about the webpage, including title, meta tags, and linked stylesheets. It is part of the document's structure but is not displayed on the webpage.
* **<title> :** Used within the <head> section to define the title of the HTML document. It appears in the browser tab or window and provides a brief description of the webpage's content.
* **<body> :** Encloses the visible content of the webpage, such as text, images, audio, videos, and links. All elements within this tag are displayed on the actual webpage when viewed in a browser.

### Headings tag
The HTML heading tags are used to create headings for the content of a webpage. <br>
* paired tag

```html
<h1></h1>
<h2></h2>
<h3></h3>
<h4></h4>
<h5></h5>
<h6></h6>
```

### Paragraph tag
HTML <p> tags are used to write paragraph statements on a webpage. They start with the <p> tag and end with </p>.
* paired tag
```html
<p> Content... </p>
```

### Break 
The HTML <br> tag is used to insert a single line break and does not require a closing tag. In HTML, the break tag is written as <br>.
* single tag
```html
<br>
```

### Horizontal Line
The HTML <hr> tag is used to divide a page into sections by creating a horizontal line that spans from the left to the right side of the page. This is an empty tag and does not require a closing tag or any additional attributes.
```html
<hr>
```

### Comments
HTML comments are annotations in your code that are not displayed in the browser. They are enclosed within <!-- and --> tags and are primarily used for documentation, explanation, or temporarily disabling code during debugging.

Single-line comment:
```html
<!-- This is a single-line comment -->
```
Multi-line comment:
```html
<!--
This is a multi-line comment
spanning multiple lines
-->
```
### Images
The <img> tag is used to insert an image into a webpage. The source of the image is specified within the src attribute, like this: <img src="source_of_image">.
```html
<img src="geeks.png">
```

### Source Code
1. **View HTML Source Code of Entire Page**
* **ctrl + u** on the page, **or right-click**on the page and select the **"view page source"** option.
* This will open a new tab that shows the HTML source code for that entire page.
2. **Inspect an HTML Element on a Page**
* **right-click** on the page and select the **"Inspect"** option.
* This lets you see the HTML and CSS behind that element.

* by going on on a website device icon <img width="39" height="32" alt="image" src="https://github.com/user-attachments/assets/c932b376-68ea-4ea1-a830-6bec5f611867" /> you can view how website looks on other device.

* **name = "viewport"** for responsive of site on other device.

#### important points

* on vs code we can select a tag and get it know with mdn
* **index.html** -> homepage (ny default) if not you will have to specify the homepage
* **!** -> emit boiler plate code



 
**Must know**

* Semantic tags
* Forms & inputs
* Accessibility basics

📌 Build:

* Resume page
* Blog layout

---

# CSS 

- [css roadmap.sh](https://roadmap.sh/css)


**Must know**

* Box model
* Flexbox
* Grid
* Responsive design
* Media queries

📌 Build:

* Responsive landing page
* Portfolio layout

---

## JavaScript

- [javascript roadmap.sh](https://roadmap.sh/javascript)


**Core**

* Variables, functions, loops
* Arrays & objects
* DOM manipulation
* Events
* ES6 (let, const, arrow, map/filter)

**Advanced**

* Closures
* Promises
* async/await
* Fetch API

📌 Build:

* To-do app
* Weather app (API)
* Form validation

🎯 Interview focus:

* `map vs forEach`
* `var vs let vs const`
* Event bubbling
* Async JS


---

## React.js 

**Core**

* Components
* Props & state
* Hooks (`useState`, `useEffect`)
* Conditional rendering

**Advanced**

* Context API
* Custom hooks
* React Router

📌 Build:

* Notes app
* E-commerce frontend
* Portfolio (React)

🎯 Interview focus:

* State vs props
* Virtual DOM
* useEffect lifecycle

---

# Backend 

## 6️⃣ Backend Basics

Choose **Node.js + Express** (industry-friendly)

**Learn**

* REST APIs
* HTTP methods
* Middleware
* MVC pattern

📌 Build:

* CRUD API
* Auth system (login/signup)

---

## 7️⃣ Database (Week 2–3)

Choose **MongoDB**

* Collections & documents
* CRUD operations
* Indexes

📌 Build:

* User DB
* Blog backend

🎯 Interview focus:

* SQL vs NoSQL
* Indexing
* Data modeling

---


## Full Stack Projects

Combine **React + Node + DB**

📌 MUST PROJECTS (Choose 3)

* Full auth app
* Job portal
* Expense tracker
* Blog platform

Each project must have:

* Live deployment
* Clean README
* Screenshots

---

## System and Web Concepts

* Authentication (JWT)
* Cookies vs localStorage
* CORS
* Security basics

---

# Interviews Internships 

## 🔎 Interview Preparation

### Web Dev Questions

* How browser works
* REST vs GraphQL
* HTTP status codes
* React performance

### DSA (Parallel)

* Arrays, strings
* Stack, queue
* Recursion
* Time complexity

(You’re already doing DSA → continue 🔥)

---

## 📂 Portfolio & Resume

### Portfolio

* About
* Skills
* Projects
* GitHub
* Contact

### Resume

* 1 page
* Skills → Projects → Education

---

## 🧲 Getting Internships & Jobs

### Apply On

* Internshala
* LinkedIn
* Wellfound (AngelList)
* Company career pages

### Strategy

* 5–10 applications/day
* Cold email startups
* Share projects on LinkedIn

---

# 🏁 FINAL CHECKLIST (If YES → You’re Ready)

✔ 5+ projects
✔ React + Backend
✔ GitHub active
✔ Can explain projects clearly
✔ Basic DSA

---


