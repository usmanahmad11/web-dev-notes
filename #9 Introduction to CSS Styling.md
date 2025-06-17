# Introduction to CSS Styling

## Introduction
CSS (Cascading Style Sheets) is used to style and visually enhance web pages. It allows developers to control the layout, colors, fonts, and overall appearance of HTML elements. Learning CSS is essential for creating visually appealing websites.

## Learning Objectives
By the end of this lecture, you will:
- Understand the purpose of CSS and how it works with HTML.
- Learn how to apply CSS styles using inline, internal, and external methods.
- Be able to style basic HTML elements like headings, paragraphs, and links.

## Content

### What is CSS?
CSS is a stylesheet language that defines how HTML elements are displayed on a web page. It can be used to change colors, fonts, spacing, and layout.

### Ways to Apply CSS
There are three main ways to apply CSS to an HTML document:
1. **Inline CSS**: Styles are applied directly within an HTML element using the `style` attribute.
2. **Internal CSS**: Styles are defined within a `<style>` tag inside the `<head>` section of the HTML document.
3. **External CSS**: Styles are written in a separate `.css` file and linked to the HTML document using a `<link>` tag.

#### Example: Inline CSS
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Inline CSS Example</title>
  </head>
  <body>
    <h1 style="color: blue;">Welcome to My Website</h1> <!-- Inline style -->
    <p style="font-size: 18px; color: gray;">This is a paragraph with inline styling.</p>
  </body>
</html>
```

#### Explanation:
- The `style` attribute is used to apply CSS directly to an element.
- `color: blue;` changes the text color to blue.
- `font-size: 18px;` sets the font size to 18 pixels.

#### Example: Internal CSS
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Internal CSS Example</title>
    <style>
      h1 {
        color: green; /* Changes heading color to green */
      }
      p {
        font-size: 16px; /* Sets paragraph font size */
        color: darkgray; /* Changes paragraph color */
      }
    </style>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph styled with internal CSS.</p>
  </body>
</html>
```

#### Explanation:
- The `<style>` tag is used to define CSS rules within the HTML document.
- CSS selectors like `h1` and `p` target specific elements.

#### Example: External CSS
```html
<!-- Save this as index.html -->
<!DOCTYPE html>
<html>
  <head>
    <title>External CSS Example</title>
    <link rel="stylesheet" href="styles.css"> <!-- Links to external CSS file -->
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph styled with external CSS.</p>
  </body>
</html>
```

```css
/* Save this as styles.css */
h1 {
  color: purple; /* Changes heading color to purple */
}
p {
  font-size: 14px; /* Sets paragraph font size */
  color: black; /* Changes paragraph color */
}
```

#### Explanation:
- The `<link>` tag connects the HTML file to an external CSS file.
- External CSS keeps styles separate from the HTML structure, making it easier to manage.

### Viewing Your CSS File
To view your styled HTML file:
1. Save the HTML code as `index.html`.
2. Save the external CSS code as `styles.css` in the same folder.
3. Open `index.html` in a web browser.

## Exercises
1. Create an HTML file with:
   - A heading styled with inline CSS to have a red color.
   - A paragraph styled with internal CSS to have a font size of 20px and a blue color.

2. Create an external CSS file to style:
   - A heading with a green color.
   - A paragraph with a font size of 16px and a gray color.

3. Experiment with different CSS properties like `background-color`, `text-align`, and `margin`.

## Summary
CSS is a powerful tool for styling web pages. It can be applied using inline, internal, or external methods. By mastering CSS, you can control the appearance of HTML elements and create visually appealing websites.

## Further Reading
- [CSS Basics - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [CSS Tutorial - W3Schools](https://www.w3schools.com/css/)
- [Learn CSS - freeCodeCamp](https://www.freecodecamp.org/news/css-basics/)
