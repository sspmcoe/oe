# Web Development Practicals (HTML, CSS, and JavaScript)

Save each program in a separate HTML file using the filename shown in its heading and open it in a web browser to run it.

---

## 1. Static Web Page Development (`index.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Home Page</title>
<style>
body { font-family: Arial, sans-serif; margin: 0; background: #f2f2f2; text-align: center; }
header { background: navy; color: white; padding: 20px; }
nav { background: #333; padding: 12px; }
nav a { color: white; margin: 15px; text-decoration: none; }
main { padding: 30px; }
footer { background: navy; color: white; padding: 12px; }
</style>
</head>
<body>
<header>
<h1>Welcome to My Website</h1>
<p>My First Static Web Page</p>
</header>
<nav>
<a href="index.html">Home</a>
<a href="about.html">About</a>
<a href="contact.html">Contact</a>
</nav>
<main>
<h2>Home Page</h2>
<p>This is a simple static website created using HTML and CSS.</p>
<img src="[https://placehold.co/300x150](https://placehold.co/300x150)" alt="Sample Image">
</main>
<footer><p>&copy; 2026 My Website</p></footer>
</body>
</html>
```

---

## 2. Interactive Forms with JavaScript Validation (`form.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Registration Form</title>
<style>
body { font-family: Arial, sans-serif; margin: 30px; background: #eef2f3; }
form { max-width: 350px; margin: auto; background: white; padding: 20px; border-radius: 8px; }
input { width: 95%; padding: 8px; margin: 8px 0; }
button { padding: 10px 20px; background: green; color: white; border: none; }
</style>
</head>
<body>
<form id="myForm">
<h2>Registration Form</h2>
<label>Name:</label>
<input type="text" id="name" required>
<label>Email:</label>
<input type="email" id="email" required>
<label>Password:</label>
<input type="password" id="password" required>
<button type="submit">Submit</button>
<p id="message"></p>
</form>
<script>
document.getElementById("myForm")
.addEventListener("submit", function(event) {
event.preventDefault();
let name = document.getElementById("name").value.trim();
let email = document.getElementById("email").value.trim();
let password = document.getElementById("password").value;
if (name === "") {
alert("Please enter your name");
} else if (!email.includes("@")) {
alert("Please enter a valid email");
} else if (password.length < 6) {
alert("Password must be at least 6 characters");
} else {
document.getElementById("message").textContent = "Registration successful!";
}
});
</script>
</body>
</html>
```

---

## 3. Static Web Page Development (`contact.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Contact Us</title>
<style>
body { font-family: Arial, sans-serif; background: #f0f8ff; text-align: center; margin: 0; }
header { background: teal; color: white; padding: 20px; }
section { background: white; margin: 30px auto; padding: 25px; max-width: 400px; }
a { color: blue; }
</style>
</head>
<body>
<header><h1>Contact Us</h1></header>
<section>
<h2>Our Contact Details</h2>
<p><strong>Name:</strong> ABC Company</p>
<p><strong>Email:</strong> <a href="mailto:abc@example.com">abc@example.com</a></p>
<p><strong>Phone:</strong> 9876543210</p>
<p><strong>Address:</strong> Mumbai, Maharashtra</p>
</section>
</body>
</html>
```

---

## 4. JavaScript Control Flow and Simple Application (`game.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Number Guessing Game</title>
<style>
body { font-family: Arial, sans-serif; text-align: center; margin-top: 70px; background: #fff8dc; }
input, button { padding: 10px; margin: 5px; }
button { cursor: pointer; }
</style>
</head>
<body>
<h1>Number Guessing Game</h1>
<p>Guess a number between 1 and 10.</p>
<input type="number" id="guess" min="1" max="10" placeholder="Enter number">
<button onclick="checkGuess()">Check</button>
<button onclick="restartGame()">Restart</button>
<p id="result"></p>
<p id="attempts">Attempts: 0</p>
<script>
let secretNumber = Math.floor(Math.random() * 10) + 1;
let count = 0;

function checkGuess() {
let guess = Number(document.getElementById("guess").value);
let result = document.getElementById("result");

if (document.getElementById("guess").value === "" || guess < 1 || guess > 10) {
result.textContent = "Enter a number from 1 to 10.";
return;
}

count++;

if (guess === secretNumber) {
result.textContent = "Correct! You won!";
} else if (guess < secretNumber) {
result.textContent = "Too low! Try again.";
} else {
result.textContent = "Too high! Try again.";
}

document.getElementById("attempts").textContent = "Attempts: " + count;
}

function restartGame() {
secretNumber = Math.floor(Math.random() * 10) + 1;
count = 0;
document.getElementById("guess").value = "";
document.getElementById("result").textContent = "";
document.getElementById("attempts").textContent = "Attempts: 0";
}
</script>
</body>
</html>
```

---

## 5. Static Web Page Development (`About.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>About Us</title>
<style>
body { font-family: Arial, sans-serif; margin: 0; background: #f5f5f5; }
header { background: darkblue; color: white; text-align: center; padding: 20px; }
main { background: white; max-width: 700px; margin: 30px auto; padding: 25px; line-height: 1.6; }
footer { background: darkblue; color: white; text-align: center; padding: 10px; }
</style>
</head>
<body>
<header><h1>About Us</h1></header>
<main>
<h2>Who We Are</h2>
<p>Welcome to our website.</p>
<h2>Our Mission</h2>
<p>Our mission is to provide quality services and useful information to everyone.</p>
<h2>Our Vision</h2>
<p>We aim to create a better future through knowledge and technology.</p>
</main>
<footer><p>&copy; 2026 About Us</p></footer>
</body>
</html>
```

---

## 6. JavaScript DOM Manipulation and Event Handling (`Dom.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>DOM Manipulation</title>
<style>
body { font-family: Arial, sans-serif; text-align: center; margin-top: 80px; background: #e6f7ff; }
button { padding: 12px 20px; margin: 5px; cursor: pointer; background: blue; color: white; border: none; border-radius: 5px; }
#message { font-size: 22px; color: darkgreen; }
</style>
</head>
<body>
<h1>DOM Manipulation</h1>
<p id="message">Welcome to JavaScript!</p>
<button id="changeBtn">Change Text</button>
<button id="colorBtn">Change Color</button>
<button id="resetBtn">Reset</button>
<script>
let message = document.getElementById("message");

document.getElementById("changeBtn")
.addEventListener("click", function() {
message.textContent = "Text changed successfully!";
});

document.getElementById("colorBtn")
.addEventListener("click", function() {
message.style.color = "red";
});

document.getElementById("resetBtn")
.addEventListener("click", function() {
message.textContent = "Welcome to JavaScript!";
message.style.color = "darkgreen";
});
</script>
</body>
</html>
```
