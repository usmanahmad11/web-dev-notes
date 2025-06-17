# Introduction to JavaScript

## Introduction
JavaScript is a programming language that enables interactivity and dynamic behavior on web pages. It works alongside HTML and CSS to create engaging user experiences. Learning JavaScript is essential for building modern websites and web applications.

## Learning Objectives
By the end of this lecture, you will:
- Understand what JavaScript is and its role in web development.
- Learn how to add JavaScript to HTML pages.
- Explore browser developer tools and the console.
- Write your first JavaScript program.

## Content

### What is JavaScript and Its Role in Web Development
JavaScript is a scripting language that runs in the browser. It allows you to:
- Manipulate HTML elements (e.g., change text or styles).
- Respond to user actions (e.g., button clicks).
- Perform calculations and logic.
- Communicate with servers (e.g., fetch data).

#### Example Use Cases:
- Form validation.
- Animations and transitions.
- Interactive features like dropdown menus and sliders.

### Adding JavaScript to HTML Pages
JavaScript can be added to an HTML document in three ways:
1. **Inline**: Inside an HTML element using the `onclick` attribute.
2. **Internal**: Inside a `<script>` tag within the HTML file.
3. **External**: In a separate `.js` file linked to the HTML file.

#### Example: Inline JavaScript
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Inline JavaScript Example</title>
  </head>
  <body>
    <button onclick="alert('Hello, World!')">Click Me</button> <!-- Inline JavaScript -->
  </body>
</html>
```

#### Explanation:
- The `onclick` attribute runs JavaScript code when the button is clicked.
- `alert('Hello, World!')` displays a popup message.

#### Example: Internal JavaScript
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Internal JavaScript Example</title>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <button id="myButton">Click Me</button>
    <script>
      // JavaScript code inside a <script> tag
      document.getElementById('myButton').onclick = function() {
        alert('Button clicked!');
      };
    </script>
  </body>
</html>
```

#### Explanation:
- The `<script>` tag contains JavaScript code.
- `document.getElementById('myButton')` selects the button element by its ID.
- The `onclick` event triggers the `alert` function when the button is clicked.

#### Example: External JavaScript
```html
<!-- Save this as index.html -->
<!DOCTYPE html>
<html>
  <head>
    <title>External JavaScript Example</title>
    <script src="script.js"></script> <!-- Links to external JavaScript file -->
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <button id="myButton">Click Me</button>
  </body>
</html>
```

```javascript