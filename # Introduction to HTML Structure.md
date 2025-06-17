# Introduction to HTML Structure

## Introduction
HTML (HyperText Markup Language) is the backbone of web development. It provides the structure for web pages, allowing developers to organize content and define elements like headings, paragraphs, images, and links. Understanding HTML is the first step toward building websites.

## Learning Objectives
By the end of this lecture, you will:
- Understand the basic structure of an HTML document.
- Learn how to use common HTML tags like `<html>`, `<head>`, `<body>`, `<h1>`, `<p>`, and `<a>`.
- Be able to create a simple web page with text and links.

## Content

### Basic HTML Document Structure
An HTML document consists of nested elements that define the structure of a web page. Below is the basic structure of an HTML document:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Web Page</title> <!-- This sets the page title -->
  </head>
  <body>
    <h1>Welcome to My Website</h1> <!-- This is a heading -->
    <p>This is a paragraph of text.</p> <!-- This is a paragraph -->
    <a href="https://www.example.com">Visit Example</a> <!-- This is a link -->
  </body>
</html>
```

#### Explanation:
- `<!DOCTYPE html>`: Declares the document type and version of HTML.
- `<html>`: The root element that contains all other elements.
- `<head>`: Contains metadata about the document (e.g., title, styles).
- `<body>`: Contains the visible content of the web page.
- `<h1>`: A heading tag used for titles.
- `<p>`: A paragraph tag for text.
- `<a>`: An anchor tag for hyperlinks.

### Adding More Content
You can add multiple headings, paragraphs, and links to your web page. Here's an example:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>About Me</title>
  </head>
  <body>
    <h1>About Me</h1>
    <p>Hello! My name is Alex, and I love web development.</p>
    <h2>My Hobbies</h2>
    <ul>
      <li>Coding</li>
      <li>Reading</li>
      <li>Traveling</li>
    </ul>
    <a href="https://www.myportfolio.com">Check out my portfolio</a>
  </body>
</html>
```

#### Explanation:
- `<h2>`: A smaller heading for subtopics.
- `<ul>`: An unordered list for bullet points.
- `<li>`: List items within the unordered list.

### Viewing Your HTML File
To view your HTML file:
1. Save the code in a file named `index.html`.
2. Open the file in a web browser (e.g., Chrome, Firefox).

## Exercises
1. Create an HTML file with the following:
   - A title of "My Favorite Foods."
   - A heading that says "My Favorite Foods."
   - A paragraph describing your favorite foods.
   - A link to a recipe website.

2. Add an unordered list of three hobbies to your HTML file.

3. Modify the example code to include a second paragraph and a second link.

## Summary
HTML provides the structure for web pages using elements like `<html>`, `<head>`, `<body>`, `<h1>`, `<p>`, and `<a>`. By mastering these basic tags, you can create simple yet functional web pages. Practice writing and viewing HTML files to build your skills.

## Further Reading
- [HTML Basics - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [HTML Tutorial - W3Schools](https://www.w3schools.com/html/)
- [Introduction to HTML - freeCodeCamp](https://www.freecodecamp.org/news/html-basics/)