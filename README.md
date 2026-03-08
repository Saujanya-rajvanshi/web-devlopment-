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
- [Static vs Dynamic Web Pages](#Static-vs-Dynamic-Web-Pages)
- [Internet DNS HTTP HTTPS](#Internet-DNS-HTTP-HTTPS)
- [What is frontend vs backend](#What-is-frontend-vs-backend)
- [How browsers render HTML/CSS/JS](#How-browsers-render-HTMLCSS-JS)


## Computer Basics

A **computer** is an electronic machine that:

```
Input → Processing → Output → Storage
```

### Hardware Components

* CPU (Processor)
* RAM (Memory)
* Storage (HDD / SSD)

### Software Types

* System Software
* Application Software

### File System Basics

Files are organized in folders with a **path**.

Example:

```
C:\Projects\WebApp\index.html
```

Common web file extensions:

```
.html → HTML structure
.css  → CSS styling
.js   → JavaScript logic
```

### Processes

A **process** is a running program.

---




## How the Web Works

<img width="807" height="501" alt="image" src="https://github.com/user-attachments/assets/fa36be72-a7f0-49f9-a94e-0a45c058cde6" />

### 1. User

A **user** opens a browser and types a website URL.

Example:

```
https://www.academind.com
```

The user expects the website to appear on the screen.

### 2. Browser

The **browser** receives the URL and starts the process.

Examples of browsers:

* Google Chrome
* Mozilla Firefox
* Microsoft Edge

The browser sends a **request** to find the website.

### 3. Request Sent

The browser sends a **request through the internet** asking:

> "Where is this website located?"

But computers do not understand domain names like
`academind.com`.

They understand **IP addresses**.

Example:

```
142.250.182.14
```

### 4. DNS Server

The request goes to a **DNS server**.

DNS = **Domain Name System**

Its job is to **translate domain names into IP addresses**.

Example:

```
academind.com → 192.168.1.1
```

So the DNS server tells the browser:

> "This website is located at this IP address."

### 5. Server

Now the browser sends the request to the **web server** using the IP address.

A **server** is a powerful computer that stores websites.

Example servers:

* Apache HTTP Server
* Nginx

The server processes the request and finds the website files.

These files usually include:

```
HTML
CSS
JavaScript
Images
```

### 6. Response

The server sends a **response back to the browser**.

This response contains the website files.

Example:

```
index.html
style.css
script.js
images
```

### 7. Browser Renders the Website

The browser receives the files and **builds the webpage**.

Process:

1. HTML → Structure
2. CSS → Styling
3. JavaScript → Interactivity

Finally, the **website appears on the screen**.

### Simple Flow (Easy to Remember)

```
User
 ↓
Browser
 ↓
DNS Server (Domain → IP)
 ↓
Server
 ↓
Response
 ↓
Browser Displays Website
```

---



## Static vs Dynamic Web Pages

### Static Web Pages

* Same content for every user
* No server-side processing

Technologies:

```
HTML
CSS
Basic JavaScript
```

Example:

```
Portfolio website
Documentation site
```

Flow:

```
Browser → HTML file → Display
```

### Dynamic Web Pages

* Content changes based on user or data
* Uses backend and database

Technologies:

```
Frontend → HTML, CSS, JS
Backend → Node.js / Python / Java
Database → MySQL / MongoDB
```

Flow:

```
Browser → Server → Database → Server → Browser
```

Example:

```
Instagram
Amazon
Dashboard systems
```

## Internet DNS HTTP HTTPS 

### Internet

The **Internet** is a global network connecting computers and servers worldwide.

Uses the **TCP/IP protocol** to communicate.

---

### DNS (Domain Name System)

DNS converts a **domain name** into an **IP address**.

Example:

```
google.com → 142.250.195.46
```

Steps:

1. User enters URL
2. Browser asks DNS server
3. DNS returns IP
4. Browser connects to server


### HTTP (HyperText Transfer Protocol)

HTTP is a protocol used for **communication between client and server**.

Common methods:

| Method | Purpose     |
| ------ | ----------- |
| GET    | Fetch data  |
| POST   | Send data   |
| PUT    | Update data |
| DELETE | Remove data |


### HTTP Status Codes

| Code | Meaning      |
| ---- | ------------ |
| 200  | OK           |
| 404  | Not Found    |
| 500  | Server Error |
| 401  | Unauthorized |


### HTTPS (Secure HTTP)

HTTPS = **HTTP + encryption (SSL/TLS)**

Benefits:

* Secure communication
* Data privacy
* Protection from attacks

Default port:

```
HTTPS → 443
HTTP  → 80
```

## Frontend vs Backend

### Frontend (Client Side)

Frontend is everything **visible to the user**.

Technologies:

```
HTML → Structure
CSS → Styling
JavaScript → Interactivity
```

Examples:

* Buttons
* Forms
* Layout
* Animations

Runs inside the **browser**.


### Backend (Server Side)

Backend handles **logic and data processing**.

Responsibilities:

* Authentication
* Database operations
* Business logic
* API responses

Technologies:

```
Node.js
Python
Java
PHP
```

Databases:

```
MySQL
MongoDB
PostgreSQL
```

Runs on the **server**.


### How They Work Together

```
User → Frontend → Backend → Database
                    ↓
                Response
```

## Browser Rendering HTML CSS JS

When a browser loads a webpage, it performs several steps.


### 1. HTML Parsing

The browser reads HTML and builds the **DOM (Document Object Model)**.

Example:

```html
<h1>Hello</h1>
<p>World</p>
```

DOM structure:

```
Document
 ├── h1
 └── p
```

### 2. CSS Parsing

CSS files are parsed to build the **CSSOM (CSS Object Model)**.

CSSOM contains:

* style rules
* selectors
* inheritance

### 3. Render Tree

The browser combines:

```
DOM + CSSOM
```

to create the **Render Tree**.

Only **visible elements** are included.

### 4. Layout (Reflow)

Browser calculates:

* element size
* element position
* page layout

### 5. Painting

Browser draws:

* text
* colors
* images
* borders

on the screen.

### 6. Compositing

The browser combines layers using the **GPU** for better performance.

### Complete Rendering Flow

```
HTML → DOM
CSS → CSSOM
DOM + CSSOM → Render Tree
Render Tree → Layout → Paint → Composite
```

### Performance Tips

* Minimize DOM updates
* Avoid frequent layout changes
* Use `defer` for JavaScript
* Optimize CSS and images

---

























# HTML

## Table of Contents 
* [Web Fundamentals](#web-fundamentals)
* [HTML Document Structure](#HTML-Document-Structure)
* [Elements, Tags & Content Model](#Elements-Tags-and-Content-Model)
* [Elements](#Elements)
* [Tags](#Tags)
* [Content Model](#Content-Model)
* [Text & Typography Elements](#text--typography-elements)
* [Links & Navigation](#links--navigation)
* [Images & Multimedia](#images--multimedia)
* [Lists](#lists)
* [Tables](#tables)
* [Forms & Input Controls](#forms--input-controls)
* [Semantic HTML & Page Layout](#semantic-html--page-layout)
* [Global Attributes](#global-attributes)
* [Metadata & SEO](#metadata--seo)
* [Accessibility (A11Y)](#accessibility-a11y)
* [HTML Entities & Symbols](#html-entities--symbols)
* [Embedding External Content](#embedding-external-content)
* [HTML5 APIs (Canvas, SVG, Media)](#html5-apis-canvas-svg-media)
* [Best Practices & Validation](#best-practices--validation)
* [Performance Basics](#performance-basics)
* [Browser Rendering & DOM Basics](#browser-rendering--dom-basics)
* [Real-World Page Structure Patterns](#real-world-page-structure-patterns)
* [HTML Project Building](#html-project-building)


HTML is the **standard markup language used to structure web pages**.

* HTML = HyperText Markup Language
* Defines **structure of web content**
* Not a programming language
* Uses **elements (tags)** to describe content
* Works in a **client–server architecture**

Basic web flow:

1. Browser sends **HTTP request**
2. Server sends **HTML response**
3. Browser renders the page

Technology roles:

* **HTML** → Structure
* **CSS** → Styling
* **JavaScript** → Behavior

Rendering occurs inside the **browser rendering engine**, which parses HTML into the DOM.

Reference: **MDN Web Docs**

# Web Fundamentals

Core technologies of the web:

**HTML**

* Structures the content of a webpage

**CSS**

* Controls layout, colors, fonts, and design

**JavaScript**

* Adds interactivity and dynamic behavior

Other fundamental concepts:

* URL (Uniform Resource Locator)
* HTTP / HTTPS protocol
* Client–Server communication
* Browser rendering engine


# HTML Document Structure

<img width="814" height="696" alt="image" src="https://github.com/user-attachments/assets/7c9a1ea7-32df-47c4-8778-be7523096245" />

Every HTML page follows a basic structure.

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

**Important elements**

`<!DOCTYPE html>`
Declares HTML5 document type.

`<html>`
Root element containing the entire page.

`<head>`
Contains metadata, links, and document information.

`<title>`
Displayed in browser tab.

`<body>`
Contains all visible webpage content.


# Elements, Tags & Content Model

## Elements

HTML documents are built from **elements**.

Structure:

```
<tagname>Content</tagname>
```

Components:

* Opening tag
* Content
* Closing tag
* Attributes

Example

```html
<p class="text">Hello</p>
```

### Types of Elements

**Container elements**

Have opening and closing tags.

Examples

```
<p>
<div>
<section>
<article>
```

**Void elements**

No closing tag.

Examples

```
<br>
<hr>
<img>
<input>
<meta>
<link>
```


## Tags

Tags define **meaning and structure**.

### Structural Tags

```
<html>
<head>
<body>
<header>
<nav>
<main>
<section>
<article>
<aside>
<footer>
```

### Text Semantic Tags

```
<h1>–<h6>
<p>
<strong>
<em>
<mark>
<small>
<cite>
<time>
```

### Formatting Tags

```
<b>
<i>
<u>
<sub>
<sup>
<pre>
<code>
<kbd>
```

### Content Grouping

```
<div>
<span>
<ul>
<ol>
<li>
<dl>
<dt>
<dd>
```

### Media Tags

```
<img>
<audio>
<video>
<source>
<track>
<figure>
<figcaption>
```

### Form Tags

```
<form>
<input>
<label>
<textarea>
<select>
<option>
<button>
fieldset>
legend>
```


## Content Model

HTML elements follow **content categories**.

Main categories:

**Flow content**
Most elements allowed inside `<body>`.

**Phrasing content**
Inline elements used inside text.

Examples:

```
<span>
<a>
<strong>
<em>
```

**Heading content**

```
<h1>
<h2>
<h3>
<h4>
<h5>
<h6>
```

**Sectioning content**

```
<section>
<article>
<nav>
<aside>
```

**Embedded content**

```
<img>
<video>
<audio>
<iframe>
```

**Interactive content**

```
<a>
<button>
<input>
<select>
```

Invalid nesting example:

```html
<p>
  <div></div>
</p>
```


# Text & Typography Elements

Headings

```
<h1> <h2> <h3> <h4> <h5> <h6>
```

Text structure

```
<p>
<br>
<hr>
```

Text emphasis

```
<strong>
<em>
<b>
<i>
<u>
```

Special text

```
<mark>
<small>
<sub>
<sup>
<del>
<ins>
```

Code and formatting

```
<code>
<pre>
<kbd>
<samp>
```

Quotations

```
<q>
<blockquote>
<cite>
```


# Links & Navigation

Main tag:

```
<a>
```

Example

```html
<a href="https://example.com">Visit</a>
```

Important attributes:

* `href`
* `target`
* `download`
* `rel`

Navigation structures often use:

```
<nav>
<ul>
<li>
```

Link types:

* Absolute URL
* Relative URL
* Fragment link (`#id`)

# Images & Multimedia

Image element

```
<img>
```

Example

```html
<img src="image.jpg" alt="description">
```

Related elements

```
<figure>
<figcaption>
```

Audio

```
<audio>
<source>
<track>
```

Video

```
<video>
<source>
<track>
```

Important attributes:

* `src`
* `alt`
* `controls`
* `autoplay`
* `loop`

# Lists

Unordered list

```
<ul>
<li>
```

Ordered list

```
<ol>
<li>
```

Description list

```
<dl>
<dt>
<dd>
```

Lists organize structured data.


# Tables

Table elements

```
<table>
<tr>
<th>
<td>
<thead>
<tbody>
<tfoot>
<caption>
<colgroup>
<col>
```

Attributes

* `rowspan`
* `colspan`

Tables should be used for **data representation**, not layout.


# Forms & Input Controls

Form container

```
<form>
```

Input controls

```
<input>
<textarea>
<select>
<option>
<button>
```

Supporting elements

```
<label>
<fieldset>
<legend>
<datalist>
<output>
```

Common input types

```
text
email
password
number
date
checkbox
radio
file
submit
```

Form attributes

* `action`
* `method`
* `required`
* `placeholder`
* `pattern`


# Semantic HTML & Page Layout

Semantic elements describe page structure.

Main layout tags

```
<header>
<nav>
<main>
<section>
<article>
<aside>
<footer>
```

Benefits:

* Better accessibility
* Better SEO
* Clearer code structure



# Global Attributes

Attributes usable on most elements.

Common global attributes:

```
id
class
style
title
hidden
lang
tabindex
contenteditable
data-*
dir
```

Used for styling, scripting, and accessibility.


# Metadata & SEO

Metadata is placed inside `<head>`.

Important elements

```
<meta>
<title>
<link>
<base>
```

Common metadata examples

```
<meta charset="UTF-8">
<meta name="viewport">
<meta name="description">
<meta name="author">
```

Also used for:

* search engine optimization
* social media previews



# Accessibility (A11Y)

Accessibility ensures websites are usable by everyone.

Key practices:

* Use semantic elements
* Add `alt` text to images
* Associate labels with inputs
* Maintain heading hierarchy
* Ensure keyboard navigation
* Use ARIA attributes when necessary

Example

```html
<label for="email">Email</label>
<input id="email" type="email">
```



# HTML Entities & Symbols

Entities represent reserved characters.

Examples

```
&lt;   <
&gt;   >
&amp;  &
&nbsp; non-breaking space
&copy; copyright
&reg; registered
```

Used to prevent parsing conflicts.



# Embedding External Content

Elements used to embed external resources.

```
<iframe>
<embed>
<object>
<script>
<link>
```

Example

```html
<iframe src="https://example.com"></iframe>
```

Security features:

* sandbox attribute
* content security policies



# HTML5 APIs (Canvas, SVG, Media)

Canvas

```
<canvas>
```

Used with JavaScript for drawing graphics.

SVG

```
<svg>
```

Defines scalable vector graphics.

Media APIs

```
<audio>
<video>
<track>
```

Used for multimedia playback.



# Best Practices & Validation

Recommended practices:

* Use semantic HTML
* Maintain proper indentation
* Close elements correctly
* Avoid unnecessary nesting
* Separate HTML, CSS, and JavaScript
* Validate using W3C validator



# Performance Basics

HTML structure affects page performance.

Key considerations:

* Optimize images
* Reduce DOM depth
* Avoid excessive elements
* Use lazy loading

Example

```html
<img src="image.jpg" loading="lazy">
```



# Browser Rendering & DOM Basics

Rendering process:

1. Browser parses HTML
2. Builds **DOM (Document Object Model)**
3. Parses CSS to create CSSOM
4. Combines them to build Render Tree
5. Paints pixels on screen

DOM represents the page structure in memory and allows JavaScript interaction.



# Real-World Page Structure Patterns

Typical page layout

```html
<header>
<nav></nav>
</header>

<main>
  <section>
  <article>
</main>

<footer>
</footer>
```

Common patterns:

* Hero section
* Card layouts
* Sidebar layouts
* Grid-based layouts



# HTML Project Building

Suggested workflow:

1. Plan page structure
2. Use semantic layout
3. Add content
4. Ensure accessibility
5. Validate HTML
6. Add CSS styling
7. Add JavaScript functionality

Development mindset:

Structure → Semantics → Accessibility → Performance.

---



































# CSS 

## Table of Contents

* [CSS Fundamentals](#css-Fundamentals)
* [Selectors](#selectors)
* [CSS Units & Measurements](#css-units--measurements)
* [Typography & Fonts](#typography--Text-Styling)
* [Colors & Backgrounds](#colors--Backgrounds)
* [Box Model](#box-model)
* [Borders & Outline](#borders--outline)
* [Box Shadow](#box-shadow)
* [Display & Visibility](#display--visibility)
* [Positioning](#positioning)
* [Z-Index & Stacking Context](#z-index--stacking-context)
* [Lists & Tables Styling](#lists--tables-styling)
* [Images & Filters](#images--filters)
* [Layouting Techniques](#layouting-techniques)
* [Flow Layout](#flow-layout)
* [Floating Elements](#floating-elements)
* [Multicolumn Layout](#multicolumn-layout)
* [Flexbox](#flexbox)
* [CSS Grid](#css-grid)
* [Transforms](#transforms)
* [Transitions](#transitions)
* [Animations](#animations)
* [Keyframe Animations](#keyframe-animations)
* [CSS Variables](#css-variables)
* [Responsive Design](#responsive-design)
* [Media Queries](#media-queries)
* [Container Queries](#container-queries)
* [Responsive Typography](#responsive-typography)
* [Accessibility](#accessibility)
* [Performance](#performance)
* [CSS Best Practices](#css-best-practices)
* [CSS Architecture & Methodologies](#css-architecture--methodologies)
* [BEM](#bem)
* [CSS Modules](#css-modules)
* [CSS-in-JS](#css-in-js)
* [CSS Preprocessors & Tools](#css-preprocessors--tools)
* [Sass](#sass)
* [PostCSS](#postcss)


# CSS Fundamentals

CSS controls the **visual presentation of HTML elements**, including layout, colors, fonts, spacing, and responsiveness.

- [CSS Introduction](#CSS-Introduction)
- [CSS Syntax Basics](#CSS-Syntax-Basics)
- [Applying CSS to HTML](Applying-CSS-to-HTML)
- [CSS Rules, Properties & Values](#CSS-Rules--Properties--Values)
- [CSS Comments](#CSS-Comments)

## CSS Introduction

### What is CSS

CSS stands for **Cascading Style Sheets**.
It is a stylesheet language used to describe **how HTML elements should be displayed** on a webpage.

CSS separates **content from design**.

Example:

```css
p {
  color: blue;
  font-size: 18px;
}
```

This styles all `<p>` elements with blue text and a font size of 18px.

### Why CSS is Used

CSS is used to:

* Style HTML elements
* Control page layout
* Improve visual appearance
* Make websites responsive
* Maintain consistent design across pages

Example uses:

* Changing text color
* Adding spacing between elements
* Creating responsive layouts
* Adding animations

### CSS vs HTML Responsibilities

| HTML              | CSS                 |
| ----------------- | ------------------- |
| Defines structure | Defines style       |
| Creates elements  | Controls appearance |
| Adds content      | Controls layout     |
| Semantic meaning  | Visual presentation |

Example:

HTML structure:

```html
<h1>Welcome</h1>
<p>This is a paragraph</p>
```

CSS styling:

```css
h1 {
  color: green;
}

p {
  font-size: 16px;
}
```

### Advantages of CSS

1. **Separation of content and design**
2. **Reusable styles across multiple pages**
3. **Better maintainability**
4. **Faster website performance**
5. **Responsive design support**

Example:

One CSS file can style **multiple pages**.

```
index.html
about.html
contact.html
style.css
```

# CSS Syntax Basics

CSS follows a simple rule-based syntax.

Example:

```css
h1 {
  color: red;
  font-size: 32px;
}
```

Structure:

```
selector {
  property: value;
}
```

### CSS Rule Structure

A CSS rule consists of two main parts:

1. **Selector**
2. **Declaration block**

Example:

```css
p {
  color: blue;
}
```

Breakdown:

```
p → selector
color → property
blue → value
```

### Selectors, Properties, and Values

#### Selector

Specifies **which HTML element to style**.

Example:

```css
p
h1
div
```

#### Property

The **style attribute** you want to change.

Examples:

```
color
font-size
margin
background
```

#### Value

Defines the **setting of the property**.

Example:

```css
color: red;
font-size: 20px;
margin: 10px;
```

### Declaration Blocks

A **declaration block** contains one or more CSS declarations.

Example:

```css
p {
  color: red;
  font-size: 16px;
  line-height: 1.5;
}
```

Structure:

```
selector {
  declaration;
  declaration;
}
```

Each declaration ends with a **semicolon**.

## Applying CSS to HTML

CSS can be applied to HTML in **three ways**.

### Inline CSS

CSS is written **directly inside an HTML element** using the `style` attribute.

Example:

```html
<p style="color: red;">Hello World</p>
```

Characteristics:

* Applies only to that element
* Hard to maintain
* Not recommended for large projects

### Internal CSS

CSS is written inside a `<style>` tag within the `<head>` section.

Example:

```html
<head>
<style>
p {
  color: blue;
}
</style>
</head>
```

Characteristics:

* Applies to one HTML page
* Useful for small projects

### External CSS

CSS is written in a **separate file**.

Example:

```
style.css
```

HTML link:

```html
<link rel="stylesheet" href="style.css">
```

Advantages:

* Reusable across pages
* Easier maintenance
* Better performance

This is the **recommended approach**.

### Linking Stylesheets

External CSS files are connected using the `<link>` tag.

Example:

```html
<head>
<link rel="stylesheet" href="styles.css">
</head>
```

Attributes:

| Attribute | Description                       |
| --------- | --------------------------------- |
| rel       | Relationship between HTML and CSS |
| href      | Path to CSS file                  |


## CSS Rules, Properties & Values

CSS works by applying **rules to HTML elements**.

Rule example:

```css
h1 {
  color: blue;
}
```

Meaning:

* `h1` → selector
* `color` → property
* `blue` → value

### How CSS Rules Are Interpreted by Browsers

The browser processes CSS in this order:

1. Parse HTML
2. Parse CSS
3. Match selectors to elements
4. Apply styles
5. Render the page

This process is handled by browser engines like:

* Blink
* Gecko
* WebKit

### Property–Value Pairs

Each CSS declaration consists of a **property and value pair**.

Example:

```css
color: red;
margin: 20px;
font-size: 18px;
```

Format:

```
property : value ;
```

### Shorthand Properties

Some CSS properties combine **multiple properties into one**.

Example:

Instead of:

```css
margin-top: 10px;
margin-right: 20px;
margin-bottom: 10px;
margin-left: 20px;
```

You can write:

```css
margin: 10px 20px;
```

Example shorthand properties:

```
margin
padding
border
background
font
```

## CSS Comments

Comments are used to **explain code and improve readability**. 

They are ignored by the browser.

### Syntax of Comments

CSS comments start with `/*` and end with `*/`.

Example:

```css
/* This is a CSS comment */

p {
  color: red;
}
```

### Purpose of Comments in CSS

Comments help developers:

* Explain code
* Organize sections
* Disable styles temporarily
* Improve collaboration

Example:

```css
/* Header styles */
header {
  background: black;
  color: white;
}
```

---







## CSS Selectors

Selectors determine **which HTML elements CSS will style**.
They allow you to target specific elements in the HTML document.

Example:

```css
p {
  color: blue;
}
```

Here `p` is the **selector**, and it targets all `<p>` elements.

* [Combinator Selectors](#combinator-selectors)
* [Attribute Selectors](#attribute-selectors)
* [Pseudo-classes & Pseudo-elements](#pseudo-classes--pseudo-elements)

### Basic Selectors

Basic selectors are the **most commonly used selectors** in CSS.

### Element Selector

Targets **all elements of a specific HTML tag**.

Example:

```css
p {
  color: red;
}
```

This applies the style to **all `<p>` elements**.

Example HTML:

```html
<p>Hello</p>
<p>World</p>
```

Both paragraphs will be red.

### Class Selector

Targets elements using the **class attribute**.

Syntax:

```css
.classname {
  property: value;
}
```

Example:

```css
.box {
  background: yellow;
}
```

HTML:

```html
<div class="box">Content</div>
```

Characteristics:

* Reusable
* Multiple elements can share the same class

Example:

```html
<p class="box">Text</p>
<div class="box">Box</div>
```

### ID Selector

Targets a **specific element with a unique ID**.

Syntax:

```css
#idname {
  property: value;
}
```

Example:

```css
#header {
  background: black;
  color: white;
}
```

HTML:

```html
<div id="header">Header</div>
```

Characteristics:

* Must be **unique in the page**
* Higher specificity than class selectors

## Universal Selector

Targets **all elements on the page**.

Syntax:

```css
* {
  margin: 0;
  padding: 0;
}
```

Commonly used for **CSS reset**.

Example effect:

```css
* {
  box-sizing: border-box;
}
```

## Combinator Selectors

Combinator selectors select elements **based on relationships between elements**.

### Descendant Selector

Targets elements **inside another element (at any depth)**.

Syntax:

```css
parent child
```

Example:

```css
div p {
  color: blue;
}
```

HTML:

```html
<div>
  <p>Selected</p>
</div>
```

All `<p>` inside `<div>` will be styled.

### Child Selector

Targets **direct children only**.

Syntax:

```css
parent > child
```

Example:

```css
div > p {
  color: green;
}
```

HTML:

```html
<div>
  <p>Selected</p>
  <section>
    <p>Not selected</p>
  </section>
</div>
```

Only the **direct child `<p>`** is selected.

### Adjacent Sibling Selector

Targets the **immediate sibling element**.

Syntax:

```css
element + element
```

Example:

```css
h1 + p {
  color: red;
}
```

HTML:

```html
<h1>Title</h1>
<p>Styled paragraph</p>
```

Only the **first `<p>` after `<h1>`** is selected.

### General Sibling Selector

Targets **all sibling elements after a specific element**.

Syntax:

```css
element ~ element
```

Example:

```css
h1 ~ p {
  color: purple;
}
```

HTML:

```html
<h1>Title</h1>
<p>Styled</p>
<p>Styled</p>
```

All `<p>` after `<h1>` are styled.

## Attribute Selectors

Attribute selectors target elements **based on HTML attributes**.

Example attribute:

```html
<input type="text">
```

### Selecting Elements Based on Attributes

Syntax:

```css
element[attribute]
```

Example:

```css
input[type] {
  border: 1px solid black;
}
```

This targets **all inputs that have a `type` attribute**.

### Exact Value Match

Select elements where the attribute **exactly matches a value**.

Syntax:

```css
element[attribute="value"]
```

Example:

```css
input[type="text"] {
  background: lightyellow;
}
```

This selects only **text inputs**.

### Partial Attribute Matches

Used when **only part of the attribute value matches**.

Common operators:

| Operator | Meaning     |
| -------- | ----------- |
| `^=`     | Starts with |
| `$=`     | Ends with   |
| `*=`     | Contains    |

Example:

```css
a[href^="https"] {
  color: green;
}
```

This selects links that **start with https**.

## Pseudo-classes & Pseudo-elements

These selectors target **special states or parts of elements**.

## Pseudo-classes

Pseudo-classes select elements **based on their state**.

Syntax:

```css
selector:pseudo-class
```

Example:

```css
button:hover {
  background: blue;
}
```

### :hover

Targets elements when the **mouse pointer is over them**.

Example:

```css
a:hover {
  color: red;
}
```

Used for:

* buttons
* links
* menus

### :focus

Targets elements when they **receive focus** (like input fields).

Example:

```css
input:focus {
  border: 2px solid blue;
}
```

Used for **form accessibility and UX**.

### :nth-child()

Targets elements based on their **position in a parent**.

Example:

```css
li:nth-child(2) {
  color: red;
}
```

This selects the **second list item**.

Example patterns:

```css
li:nth-child(odd)
li:nth-child(even)
li:nth-child(3n)
```

## Pseudo-elements

Pseudo-elements style **specific parts of elements**.

Syntax:

```css
selector::pseudo-element
```

### ::before

Inserts **content before an element**.

Example:

```css
p::before {
  content: "Note: ";
}
```

### ::after

Inserts **content after an element**.

Example:

```css
p::after {
  content: " ✔";
}
```

### ::first-letter

Styles the **first letter of a text element**.

Example:

```css
p::first-letter {
  font-size: 30px;
  color: red;
}
```

Commonly used in **article styling**.

#### Quick Selector Summary

| Selector   | Example   | Purpose                |
| ---------- | --------- | ---------------------- |
| Element    | `p`       | Select tag             |
| Class      | `.box`    | Select class           |
| ID         | `#header` | Select unique element  |
| Universal  | `*`       | Select all             |
| Descendant | `div p`   | Nested elements        |
| Child      | `div > p` | Direct children        |
| Adjacent   | `h1 + p`  | Immediate sibling      |
| General    | `h1 ~ p`  | All following siblings |

---











## CSS Units & Measurements

CSS units define **how sizes, spacing, and dimensions are measured** in web layouts.

* [Absolute vs Relative Units](#absolute-vs-relative-units)
* [CSS Functions](#css-functions)

They are used in properties like:

```css
width
height
margin
padding
font-size
border-width
```

Example:

```css
p {
  font-size: 16px;
  margin: 10px;
}
```

In this example:

* `16px` → font size unit
* `10px` → spacing unit

## CSS Units & Measurements

CSS measurements mainly fall into two categories:

1. **Length Units**
2. **Percentage Units**

### Length Units

Length units define **fixed or relative sizes** for elements.

Example:

```css
div {
  width: 300px;
}
```

Here the element width is **300 pixels**.

### Percentage Units

Percentage (`%`) values are **relative to the parent element**.

Example:

```css
div {
  width: 50%;
}
```

If the parent element is **800px wide**, the child becomes:

```
400px
```

Common uses:

* responsive layouts
* flexible containers

## Absolute Units

Absolute units represent **fixed measurements** that do not depend on other elements.

They are **not responsive**.

### `px` (Pixels)

The most commonly used CSS unit.

Example:

```css
h1 {
  font-size: 24px;
}
```

Characteristics:

* Fixed size
* Precise control
* Widely supported

Example layout:

```css
.container {
  width: 1200px;
}
```

### `cm` (Centimeters)

Represents **centimeters** in physical measurement.

Example:

```css
div {
  width: 5cm;
}
```

Rarely used in web design.

Mostly used for:

* printing layouts

### `mm` (Millimeters)

Represents **millimeters**.

Example:

```css
div {
  height: 10mm;
}
```

Also rarely used on websites.

### `in` (Inches)

Represents **inches**.

Example:

```css
div {
  width: 2in;
}
```

Used mainly in **print styling**.

## Relative Units

Relative units scale **based on another value** like font size, viewport, or parent element.

These are **essential for responsive design**.

## `em`

Relative to the **font size of the parent element**.

Example:

```css
p {
  font-size: 2em;
}
```

If parent font size = `16px`

```
2em = 32px
```

Example:

```css
.container {
  font-size: 20px;
}

p {
  font-size: 1.5em;
}
```

Result:

```
1.5 × 20px = 30px
```

## `rem`

Relative to the **root element (`html`) font size**.

Example:

```css
p {
  font-size: 2rem;
}
```

If root font size = `16px`

```
2rem = 32px
```

Example:

```css
html {
  font-size: 16px;
}

h1 {
  font-size: 3rem;
}
```

Result:

```
3 × 16px = 48px
```

`rem` is preferred because it is **more predictable than em**.

### `%` (Percentage)

Relative to the **parent element size**.

Example:

```css
div {
  width: 50%;
}
```

If parent width = `1000px`

```
child width = 500px
```

Common uses:

* responsive containers
* flexible images

### `vw` (Viewport Width)

Represents **percentage of the browser width**.

```
1vw = 1% of viewport width
```

Example:

```css
div {
  width: 50vw;
}
```

If screen width = `1200px`

```
50vw = 600px
```

Used for **responsive layouts**.

### `vh` (Viewport Height)

Represents **percentage of the browser height**.

```
1vh = 1% of viewport height
```

Example:

```css
section {
  height: 100vh;
}
```

This makes the section **fill the entire screen height**.

Common use:

* full-screen hero sections

## CSS Functions

CSS functions perform **dynamic calculations and responsive sizing**.

## `calc()`

Performs mathematical calculations in CSS.

Example:

```css
div {
  width: calc(100% - 200px);
}
```

Meaning:

```
Container width minus 200px
```

Useful for:

* flexible layouts
* dynamic spacing

### `min()`

Chooses the **smallest value**.

Example:

```css
width: min(500px, 90%);
```

Meaning:

The width will be **whichever value is smaller**.

### `max()`

Chooses the **largest value**.

Example:

```css
width: max(300px, 50%);
```

Meaning:

The width will be **whichever value is larger**.

### `clamp()`

Sets **minimum, preferred, and maximum values**.

Syntax:

```
clamp(min, preferred, max)
```

Example:

```css
font-size: clamp(16px, 4vw, 32px);
```

Meaning:

* Minimum → `16px`
* Preferred → `4vw`
* Maximum → `32px`

This is very useful for **responsive typography**.

### Quick Unit Comparison

| Unit | Type     | Relative To      |
| ---- | -------- | ---------------- |
| px   | Absolute | Fixed pixels     |
| em   | Relative | Parent font size |
| rem  | Relative | Root font size   |
| %    | Relative | Parent element   |
| vw   | Relative | Viewport width   |
| vh   | Relative | Viewport height  |

**Best Practice**

Modern CSS typically uses:

```
rem for fonts
% for layouts
vw/vh for full-screen sections
clamp() for responsive typography
```

---














# 4. Typography & Text Styling

Typography controls **how text appears and is presented on a webpage**.
It affects readability, accessibility, and overall design.

CSS typography properties allow developers to control:

* Font type
* Font size
* Text alignment
* Spacing between letters and lines
* Text transformation

Example:

```css
p {
  font-family: Arial, sans-serif;
  font-size: 16px;
  line-height: 1.6;
}
```

---

# Typography & Fonts

Typography in CSS mainly deals with **fonts and how they are displayed**.

Important typography properties include:

```css
font-family
font-size
font-weight
line-height
letter-spacing
```

---

## Font Families

The `font-family` property defines **which font will be used for text**.

Example:

```css
body {
  font-family: Arial, Helvetica, sans-serif;
}
```

Multiple fonts are listed as **fallbacks**.

Explanation:

```text
Arial → first choice
Helvetica → used if Arial not available
sans-serif → default fallback
```

Types of font families:

| Type       | Example         |
| ---------- | --------------- |
| Serif      | Times New Roman |
| Sans-serif | Arial           |
| Monospace  | Courier New     |
| Cursive    | Comic Sans      |
| Fantasy    | Impact          |

Example:

```css
h1 {
  font-family: "Times New Roman", serif;
}
```

---

## Web Safe Fonts

Web safe fonts are **fonts supported by almost all browsers and operating systems**.

Common web safe fonts:

| Font            | Type       |
| --------------- | ---------- |
| Arial           | Sans-serif |
| Helvetica       | Sans-serif |
| Times New Roman | Serif      |
| Georgia         | Serif      |
| Verdana         | Sans-serif |
| Courier New     | Monospace  |

Example:

```css
p {
  font-family: Verdana, Geneva, sans-serif;
}
```

Advantages:

* Compatible across browsers
* No external loading required
* Faster performance

---

## Google Fonts Usage

Developers often use custom fonts from
Google Fonts.

Steps to use Google Fonts:

### 1. Import font in HTML

```html
<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
```

### 2. Apply in CSS

```css
body {
  font-family: 'Roboto', sans-serif;
}
```

Benefits:

* Large font library
* Easy integration
* Free to use

---

# Text Styling

Text styling controls **how text is aligned, decorated, and spaced**.

Common properties include:

```css
text-align
text-decoration
text-transform
letter-spacing
line-height
```

---

## `text-align`

Controls **horizontal alignment of text** inside an element.

Values:

| Value   | Description         |
| ------- | ------------------- |
| left    | Align text to left  |
| right   | Align text to right |
| center  | Center text         |
| justify | Spread text evenly  |

Example:

```css
p {
  text-align: center;
}
```

---

## `text-decoration`

Adds **decorative lines to text**.

Common values:

| Value        | Effect              |
| ------------ | ------------------- |
| none         | Removes decoration  |
| underline    | Underline text      |
| overline     | Line above text     |
| line-through | Strike-through text |

Example:

```css
a {
  text-decoration: none;
}
```

Often used to remove default link underline.

Example:

```css
h2 {
  text-decoration: underline;
}
```

---

## `text-transform`

Controls **capitalization of text**.

Values:

| Value      | Result               |
| ---------- | -------------------- |
| uppercase  | ALL LETTERS CAPITAL  |
| lowercase  | all letters small    |
| capitalize | First letter capital |

Example:

```css
h1 {
  text-transform: uppercase;
}
```

---

## `letter-spacing`

Controls **space between characters**.

Example:

```css
h1 {
  letter-spacing: 2px;
}
```

Uses:

* Improve readability
* Create stylistic text

Example:

```css
p {
  letter-spacing: 1px;
}
```

---

## `line-height`

Controls **vertical spacing between lines of text**.

Example:

```css
p {
  line-height: 1.5;
}
```

This means:

```text
Line height = 1.5 × font size
```

Example:

```css
p {
  font-size: 16px;
  line-height: 24px;
}
```

Benefits:

* Improves readability
* Better paragraph spacing

### Example Typography Styling

Example CSS combining multiple typography properties:

```css
body {
  font-family: "Roboto", Arial, sans-serif;
  line-height: 1.6;
}

h1 {
  text-align: center;
  text-transform: uppercase;
  letter-spacing: 2px;
}

p {
  font-size: 16px;
  line-height: 1.5;
}
```

#### Best Practices for Typography

* Use **readable fonts**
* Maintain **consistent font sizes**
* Use **sufficient line height**
* Avoid too many font families
* Ensure **good color contrast for accessibility**

---









# 5. Colors & Backgrounds

Controls **visual appearance and color design**.

* Colors

  * Named colors
  * HEX colors
  * RGB colors
  * HSL colors
  * Opacity

* Backgrounds

  * `background-color`
  * `background-image`
  * `background-size`
  * `background-repeat`
  * `background-position`

---

# 6. Box Model

Every HTML element is treated as a **rectangular box**.

* Box Model Structure

  * Content
  * Padding
  * Border
  * Margin

* Box Model Behavior

  * `box-sizing`
  * `border-box` vs `content-box`

---

# 7. Borders, Outline & Shadows

Visual styling for element boundaries.

* Borders

  * Border width
  * Border style
  * Border color
  * Border radius

* Outline

  * Difference between border and outline

* Box Shadow

  * Creating depth effects
  * Shadow properties

---

# 8. Display & Visibility

Controls **how elements appear and occupy space**.

* Display Property

  * `block`
  * `inline`
  * `inline-block`
  * `none`

* Visibility

  * `visible`
  * `hidden`

---

# 9. Positioning

Controls **where elements appear on the page**.

* Static positioning
* Relative positioning
* Absolute positioning
* Fixed positioning
* Sticky positioning

---

# 10. Z-Index & Stacking Context

Determines **which element appears above another**.

* Layer ordering
* Stacking contexts
* z-index behavior

---

# 11. Styling Lists & Tables

Customizing default HTML list and table appearance.

* Lists styling

  * list-style-type
  * list-style-position

* Tables styling

  * borders
  * spacing
  * alignment

---

# 12. Images & Filters

Styling images and applying visual effects.

* Image sizing
* Object-fit
* Filters

  * blur
  * brightness
  * contrast
  * grayscale

---

# 13. Layout Techniques

Methods for arranging elements on a page.

* Flow Layout
  Default browser layout behavior.

* Floating Elements

  * `float`
  * `clear`

* Multicolumn Layout

  * Creating newspaper-like layouts

---

# 14. Modern Layout Systems

### Flexbox

Used for **one-dimensional layouts**.

Concepts:

* Main axis
* Cross axis
* Flex container
* Flex items

Properties:

* justify-content
* align-items
* flex-direction
* flex-wrap

---

### CSS Grid

Used for **two-dimensional layouts**.

Concepts:

* Grid container
* Grid tracks
* Grid areas

Properties:

* grid-template-columns
* grid-template-rows
* grid-gap

---

# 15. CSS Effects

Adds motion and visual interaction.

### Transforms

* rotate
* scale
* translate
* skew

---

### Transitions

Smooth change between CSS values.

---

### Animations

Create complex animations using CSS.

---

### Keyframe Animations

Define animation steps using `@keyframes`.

---

# 16. CSS Variables

Reusable values stored as **custom properties**.

Benefits:

* Maintainable code
* Dynamic theming

---

# 17. Responsive Design

Making websites work across **different devices**.

* Responsive layouts
* Fluid grids

---

### Media Queries

Apply styles based on screen size.

---

### Container Queries

Apply styles based on **container size instead of screen**.

---

### Responsive Typography

Scaling fonts for different screen sizes.

---

# 18. Accessibility (A11Y)

Ensuring websites are usable for **all users**.

Examples:

* Good color contrast
* Readable font sizes
* Focus states

---

# 19. CSS Performance

Optimizing CSS for faster websites.

* Reduce unused CSS
* Avoid deep selectors
* Minification

---

# 20. CSS Best Practices

Guidelines for writing maintainable CSS.

* Consistent naming
* Modular styles
* Avoid inline CSS

---

# 21. CSS Architecture & Methodologies

Techniques for organizing large CSS projects.

### BEM

Block Element Modifier naming methodology.

---

### CSS Modules

Scoped CSS for components.

---

### CSS-in-JS

Styling directly inside JavaScript frameworks.

---

# 22. CSS Preprocessors & Tools

Tools that extend CSS capabilities.

### Sass

Adds variables, nesting, and functions.

---

### PostCSS

Transforms CSS with plugins.































## JavaScript

## Table of Contents

* [Introduction to JavaScript](#introduction-to-javascript)
* [JavaScript Environment & Execution](#javascript-environment--execution)
* [Variables & Declarations](#variables--declarations)
* [Data Types](#data-types)
* [Type Conversion & Type Casting](#type-conversion--type-casting)
* [Operators & Expressions](#operators--expressions)
* [Control Flow](#control-flow)
* [Loops & Iterations](#loops--iterations)
* [Functions](#functions)
* [Scope & Closures](#scope--closures)
* [Objects & Prototypes](#objects--prototypes)
* [Data Structures](#data-structures)
* [Equality Comparisons](#equality-comparisons)
* [Strict Mode](#strict-mode)
* [`this` Keyword](#this-keyword)
* [Error Handling](#error-handling)
* [Asynchronous JavaScript](#asynchronous-javascript)
* [Working with APIs](#working-with-apis)
* [Modules in JavaScript](#modules-in-javascript)
* [DOM & Browser APIs](#dom--browser-apis)
* [Memory Management](#memory-management)
* [Debugging & DevTools](#debugging--devtools)
* [Advanced JavaScript Concepts](#advanced-javascript-concepts)
* [JavaScript Ecosystem](#javascript-ecosystem)

---
