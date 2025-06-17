# Introduction to JavaScript Basics

## Introduction
JavaScript is a programming language that allows you to add interactivity and dynamic behavior to web pages. It works alongside HTML and CSS to create engaging user experiences. Learning JavaScript is essential for building modern websites and web applications.

## Learning Objectives
By the end of this lecture, you will:
- Understand what JavaScript is and how it interacts with HTML and CSS.
- Learn how to write basic JavaScript code.
- Be able to use JavaScript to display messages and perform simple calculations.

## Content

### What is JavaScript?
JavaScript is a scripting language that runs in the browser. It allows you to:
- Manipulate HTML elements (e.g., change text or styles).
- Respond to user actions (e.g., button clicks).
- Perform calculations and logic.

### Writing JavaScript Code
JavaScript code can be written:
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
// Save this as script.js
document.getElementById('myButton').onclick = function() {
  alert('Button clicked using external JavaScript!');
};
```

#### Explanation:
- The `<script>` tag links the HTML file to an external JavaScript file.
- External JavaScript keeps the code separate from the HTML structure, making it easier to manage.

### Basic JavaScript Syntax
Here are some basic JavaScript concepts:
1. **Variables**: Used to store data.
   ```javascript
   let name = 'Alex'; // Stores a string
   let age = 25; // Stores a number
   ```
2. **Functions**: Used to group reusable code.
   ```javascript
   function greet() {
     alert('Hello, World!');
   }
   greet(); // Calls the function
   ```
3. **Events**: Used to respond to user actions.
   ```javascript
   document.getElementById('myButton').onclick = function() {
     alert('Button clicked!');
   };
   ```

### Viewing Your JavaScript File
To view your JavaScript code:
1. Save the HTML code as `index.html`.
2. Save the external JavaScript code as `script.js` in the same folder.
3. Open `index.html` in a web browser.

## Exercises
1. Create an HTML file with:
   - A button that displays an alert message when clicked using inline JavaScript.
   - A heading that changes its text when clicked using internal JavaScript.

2. Create an external JavaScript file to:
   - Display an alert message when a button is clicked.
   - Log a message to the browser console using `console.log()`.

3. Experiment with creating variables and functions in JavaScript.

## Summary
JavaScript adds interactivity and dynamic behavior to web pages. It can be written inline, internally, or externally. By mastering JavaScript basics, you can create engaging user experiences and build modern websites.

## Further Reading
- [JavaScript Basics - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [JavaScript Tutorial - W3Schools](https://www.w3schools.com/js/)
- [Learn JavaScript - freeCodeCamp](https://www.freecodecamp.org/news/javascript-basics/)
