# OE (Web Designing) Practical Experiments

## 1. Static Web Page Development execute index file (Only index.html)

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>My Static Website</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<header>
<h1>Welcome to My Website</h1>
<nav>
<ul>
<li><a href="index.html">Home</a></li>
<li><a href="about.html">About</a></li>
<li><a href="contact.html">Contact</a></li>
</ul>
</nav>
</header>
<section>
<h2>Introduction</h2>
<p>This is a simple static website created using HTML and CSS.</p>
<img src="travel.jpg" alt="Sample Image">
</section>
<section>
<h2>Features</h2>
<ul>
<li>Easy to use</li>
<li>Lightweight</li>
</ul>
</section>
<footer>
<p>&copy; 2025 My Static Website</p>
</footer>
</body>
</html>
```

## 2. Interactive Forms with JavaScript Validation (Only form.html)

```html
<!DOCTYPE html>
<html>
<head>
<title>Form Validation Example</title>
<script src="form.js" defer></script>
<style>
body {
font-family: Arial, sans-serif;
background-color: #f9f9f9;
margin: 20px;
}
h1 {
text-align: center;
color: #333;
}
form {
max-width: 400px;
margin: auto;
background: #fff;
padding: 20px;
border: 1px solid #ccc;
border-radius: 8px;
}
label {
display: block;
margin-top: 10px;
font-weight: bold;
}
input {
width: 95%;
padding: 8px;
margin-top: 5px;
border: 1px solid #ccc;
border-radius: 5px;
}
.error {
color: red;
font-size: 14px;
}
button {
margin-top: 15px;
padding: 10px;
width: 100%;
background-color: #0066cc;
color: white;
border: none;
border-radius: 5px;
font-size: 16px;
cursor: pointer;
}
button:hover {
background-color: #004080;
}
</style>
</head>
<body>
<h1>Registration Form</h1>
<form onsubmit="return validateForm()">
<label for="name">Name:</label>
<input type="text" id="name">
<p class="error" id="nameError"></p>
<label for="email">Email:</label>
<input type="text" id="email">
<p class="error" id="emailError"></p>
<label for="password">Password:</label>
<input type="password" id="password">
<p class="error" id="passwordError"></p>
<label for="phone">Phone Number:</label>
<input type="text" id="phone">
<p class="error" id="phoneError"></p>
<button type="submit">Submit</button>
</form>
</body>
</html>
```

## 3. Static Web Page Development execute contact file (Only contact.html)

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Contact - My Static Website</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<header>
<h1>Contact Us</h1>
<nav>
<ul>
<li><a href="index.html">Home</a></li>
<li><a href="about.html">About</a></li>
<li><a href="contact.html">Contact</a></li>
</ul>
</nav>
</header>
<section>
<h2>Get in Touch</h2>
<p>You can reach us through the following platforms:</p>
<ul>
<li>Email: <a href="mailto:info@example.com">info@example.com</a></li>
<li>Phone: +91 9876543210</li>
<li>Website: <a href="https://www.example.com" target="_blank">www.example.com</a></li>
</ul>
</section>
<footer>
<p>&copy; 2025 My Static Website</p>
</footer>
</body>
</html>
```

## 4. JavaScript Control Flow and Simple Application (Only game.html)

```html
<!DOCTYPE html>
<html>
<head>
<title>Number Guessing Game</title>
<script src="game.js" defer></script>
<style>
body {
font-family: Arial, sans-serif;
text-align: center;
margin: 50px;
background-color: #f9f9f9;
}
h1 {
color: #333;
}
input, button {
padding: 10px;
margin: 10px;
border-radius: 5px;
border: 1px solid #ccc;
font-size: 16px;
}
button {
background-color: #0073e6;
color: white;
cursor: pointer;
}
button:hover {
background-color: #005bb5;
}
#message {
margin-top: 20px;
font-size: 18px;
font-weight: bold;
}
</style>
</head>
<body>
<h1>Number Guessing Game</h1>
<p>Guess a number between 1 and 100</p>
<input type="number" id="guess" placeholder="Enter your guess">
<button onclick="checkGuess()">Submit Guess</button>
<p id="message"></p>
</body>
</html>
```

## 5. Static Web Page Development execute about file (Only About.html)

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>About - My Static Website</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<header>
<h1>About Us</h1>
<nav>
<ul>
<li><a href="index.html">Home</a></li>
<li><a href="about.html">About</a></li>
<li><a href="contact.html">Contact</a></li>
</ul>
</nav>
</header>
<section>
<h2>Who We Are</h2>
<p>We are a team passionate about building simple and beautiful websites.</p>
</section>
<section>
<h2>Team Members</h2>
<table>
<tr>
<th>Name</th>
<th>Role</th>
</tr>
<tr>
<td>Alice</td>
<td>Designer</td>
</tr>
<tr>
<td>Bob</td>
<td>Developer</td>
</tr>
<tr>
<td>Charlie</td>
<td>Tester</td>
</tr>
</table>
</section>
<footer>
<p>&copy; 2025 My Static Website</p>
</footer>
</body>
</html>
```

## 6. JavaScript DOM Manipulation and Event Handling (Only Dom.html)

```html
<!DOCTYPE html>
<html>
<head>
<title>DOM Manipulation Example</title>
<script src="dom.js" defer></script>
<style>
body {
font-family: Arial, sans-serif;
margin: 20px;
}
h1 {
text-align: center;
}
#content {
background-color: #f0f0f0;
padding: 15px;
border-radius: 8px;
margin: 20px auto;
width: 400px;
}
ul {
padding-left: 20px;
}
button {
margin: 5px;
padding: 8px 12px;
background-color: #0073e6;
color: white;
border: none;
border-radius: 5px;
cursor: pointer;
}
button:hover {
background-color: #005bb5;
}
</style>
</head>
<body>
<h1>DOM Manipulation and Events</h1>
<div id="content">
<h3>My List</h3>
<ul id="myList">
<li>Item 1</li>
<li>Item 2</li>
</ul>
</div>
<div style="text-align: center;">
<button onclick="addItem()">Add Item</button>
<button onclick="removeItem()">Remove Last Item</button>
<button onclick="toggleSection()">Hide/Show Section</button>
</div>
</body>
</html>
```