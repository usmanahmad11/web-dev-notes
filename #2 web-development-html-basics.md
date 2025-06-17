# Web Development - Next Steps: HTML Basics

In this lecture, we will dive deeper into **HTML** (HyperText Markup Language), the backbone of every web page. You will learn about commonly used tags, attributes, and how to structure a web page.

---

## Step 1: Understand the Structure of an HTML Document

An HTML document is divided into two main parts:
1. **Head Section (`<head>`)**
   - Contains metadata (information about the page).
   - Includes the title, links to stylesheets, and other meta information.

2. **Body Section (`<body>`)**
   - Contains the visible content of the webpage.

Example:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Basics</title>
</head>
<body>
    <h1>Welcome to HTML Basics!</h1>
    <p>This is where the visible content goes.</p>
</body>
</html>
```

---

## Step 2: Learn Basic HTML Tags

1. **Headings**
   - HTML provides six levels of headings, from `<h1>` (largest) to `<h6>` (smallest).

   Example:
   ```html
   <h1>Main Heading</h1>
   <h2>Subheading</h2>
   <h3>Smaller Subheading</h3>
   ```

2. **Paragraphs**
   - Use `<p>` tags to create paragraphs.

   Example:
   ```html
   <p>This is a paragraph of text.</p>
   ```

3. **Links**
   - Create hyperlinks using `<a>` tags.

   Example:
   ```html
   <a href="https://www.example.com" target="_blank">Visit Example</a>
   ```

4. **Images**
   - Display images using `<img>` tags. Images require the `src` attribute (source) and the `alt` attribute (alternative text).

   Example:
   ```html
   <img src="image.jpg" alt="Description of the image">
   ```

5. **Lists**
   - Create ordered lists (`<ol>`) or unordered lists (`<ul>`) with list items (`<li>`).

   Example:
   ```html
   <ul>
       <li>First item</li>
       <li>Second item</li>
   </ul>

   <ol>
       <li>First item</li>
       <li>Second item</li>
   </ol>
   ```

6. **Divs and Spans**
   - Use `<div>` for block-level elements and `<span>` for inline elements.

   Example:
   ```html
   <div>
       <p>This is a block-level element.</p>
   </div>
   <span>This is an inline element.</span>
   ```

---

## Step 3: Add Attributes to Tags

Attributes provide additional information about an element. They are written inside the opening tag.

Example:
```html
<a href="https://www.example.com" target="_blank" title="Go to Example">Visit Example</a>
```

- `href`: Specifies the URL for a link.
- `target`: Opens the link in a new tab (`_blank`).
- `title`: Adds a tooltip when you hover over the link.

---

## Step 4: Create a Practice HTML File

1. Open your project folder in VS Code.
2. Create a new file named `html_basics.html`.
3. Write the following code:

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>HTML Basics Practice</title>
   </head>
   <body>
       <h1>HTML Basics</h1>
       <p>This is a paragraph.</p>
       <a href="https://www.google.com" target="_blank">Visit Google</a>
       <img src="https://via.placeholder.com/150" alt="Placeholder Image">
       <h2>My Favorite Things</h2>
       <ul>
           <li>Coding</li>
           <li>Music</li>
           <li>Books</li>
       </ul>
   </body>
   </html>
   ```

4. Open the file with **Live Server** to view your changes in real-time.

---

## Step 5: Experiment with More Tags

Try adding these tags to your practice file:
1. **Horizontal Rule (`<hr>`)**:
   ```html
   <hr>
   ```

2. **Bold Text (`<b>`)**:
   ```html
   <b>This text is bold.</b>
   ```

3. **Italic Text (`<i>`)**:
   ```html
   <i>This text is italic.</i>
   ```

4. **Blockquote (`<blockquote>`)**:
   ```html
   <blockquote>This is a blockquote.</blockquote>
   ```

---

## Summary

In this lecture, you learned:
- The structure of an HTML document.
- Commonly used HTML tags and their attributes.
- How to create and experiment with an HTML file.

---

In the next lecture, we will learn about **CSS (Cascading Style Sheets)** to style your web pages and make them visually appealing.

Happy coding!
