# HTML Forms - Part 1

## Introduction
Forms are a crucial part of web development, enabling user interaction and data collection. They allow users to input information, such as text, passwords, and comments, and submit it to a server. Learning how to create and organize forms is essential for building interactive websites.

## Learning Objectives
By the end of this lecture, you will:
- Understand the basic structure of an HTML form using the `<form>` element.
- Learn how to create text inputs, password fields, and textareas.
- Use labels to improve form organization and accessibility.
- Understand basic form validation techniques.

## Content

### Form Element and Basic Structure
The `<form>` element is used to create a form. It acts as a container for input fields and other elements.

#### Example: Basic Form
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Basic Form Example</title>
  </head>
  <body>
    <h1>Contact Us</h1>
    <form action="/submit" method="post">
      <input type="text" name="name" placeholder="Your Name" /> <!-- Text input -->
      <input type="submit" value="Submit" /> <!-- Submit button -->
    </form>
  </body>
</html>
```

#### Explanation:
- `<form>`: Defines the form.
  - `action`: Specifies the URL where the form data will be sent.
  - `method`: Specifies the HTTP method (`get` or `post`) for submitting the form.
- `<input>`: Defines