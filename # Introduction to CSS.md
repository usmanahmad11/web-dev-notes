# Introduction to CSS

## Introduction
CSS (Cascading Style Sheets) is a stylesheet language used to control the appearance of HTML elements on a web page. It allows you to add colors, layouts, fonts, and other visual styles to your website. Learning CSS is essential for creating visually appealing and user-friendly web pages.

## Learning Objectives
By the end of this lecture, you will:
- Understand what CSS is and why it is used.
- Learn the three ways to add CSS to a webpage: inline, internal, and external.
- Understand CSS syntax and basic selectors.
- Create your first styled webpage.

## Content

### What is CSS and Why Use It?
CSS is used to separate the presentation of a webpage from its structure (HTML). It allows you to:
- Style text (e.g., colors, fonts, sizes).
- Control layouts (e.g., margins, padding, positioning).
- Add visual effects (e.g., backgrounds, borders).

#### Benefits of CSS:
- Improves the visual appeal of websites.
- Makes websites responsive and adaptable to different devices.
- Simplifies maintenance by separating design from content.

### Three Ways to Add CSS
CSS can be added to a webpage in three ways: inline, internal, and external.

#### Inline CSS
Inline CSS is applied directly within an HTML element using the `style` attribute.

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

#### Internal CSS
Internal CSS is defined within a `<style>` tag inside the `<head>` section of the HTML document.

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

#### External CSS
External CSS is written in a separate `.css` file and linked to the HTML document using a `<link>` tag.

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

### CSS Syntax and Basic Selectors
CSS syntax consists of selectors and declarations.

#### Example: CSS Syntax
```css
selector {
  property: value;
}
```

#### Explanation:
- **Selector**: Targets the HTML element to style (e.g., `h1`, `p`).
- **Property**: Specifies the style to apply (e.g., `color`, `font-size`).
- **Value**: Defines the value of the property (e.g., `blue`, `16px`).

#### Basic Selectors
1. **Element Selector**: Targets all elements of a specific type.
   ```css
   h1 {
     color: red;
   }
   ```
2. **Class Selector**: Targets elements with a specific class.
   ```css
   .highlight {
     background-color: yellow;
   }
   ```
3. **ID Selector**: Targets a specific element by its ID.
   ```css
   #title {
     font-size: 24px;
   }
   ```

#### Example: Using Selectors
```html
<!DOCTYPE html>
<html>
  <head>
    <title>CSS Selectors Example</title>
    <style>
      h1 {
        color: red; /* Element selector */
      }
      .highlight {
        background-color: yellow; /* Class selector */
      }
      #title {
        font-size: 24px; /* ID selector */
      }
    </style>
  </head>
  <body>
    <h1 id="title">Welcome to My Website</h1>
    <p class="highlight">This is a highlighted paragraph.</p>
  </body>
</html>
```

### Your First Styled Webpage
Combine everything you've learned to create a styled webpage.

#### Example: Styled Webpage
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Styled Webpage</title>
    <style>
      body {
        font-family: Arial, sans-serif;
        background-color: #f0f0f0;
        margin: 20px;
      }
      h1 {
        color: blue;
        text-align: center;
      }
      p {
        font-size: 18px;
        color: gray;
      }
    </style>
  </head>
  <body>
    <h1>Welcome to My Styled Webpage</h1>
    <p>This is a paragraph styled with internal CSS.</p>
  </body>
</html>
```

### Viewing Your Styled Webpage
To view your styled webpage:
1. Save the code as `index.html`.
2. Open the file in a web browser.

## Exercises
1. Create a webpage with:
   - A heading styled with a red color.
   - A paragraph styled with a font size of 20px and a blue color.

2. Add a class to a paragraph and style it with a yellow background using internal CSS.

3. Create an external CSS file to style:
   - A heading with a green color.
   - A paragraph with a font size of 16px and a gray color.

## Summary
CSS is a powerful tool for styling web pages. It can be applied using inline, internal, or external methods. By mastering CSS syntax and selectors, you can control the appearance of HTML elements and create visually appealing websites.

## Further Reading
- [CSS Basics - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [CSS Tutorial - W3Schools](https://www.w3schools.com/css/)
- [Learn CSS - freeCodeCamp](https://www.freecodecamp.org/news/css-basics/)