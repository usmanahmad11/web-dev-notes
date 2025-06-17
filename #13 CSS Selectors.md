# CSS Selectors

## Introduction
CSS selectors are used to target HTML elements for styling. They allow you to apply styles to specific elements, groups of elements, or elements based on their state or position. Understanding selectors is essential for writing efficient and organized CSS.

## Learning Objectives
By the end of this lecture, you will:
- Understand basic selectors like element, class, and ID selectors.
- Learn advanced selectors like descendant and child selectors.
- Use pseudo-classes like `:hover`, `:focus`, and `:nth-child`.
- Understand selector specificity and the cascade.

## Content

### Basic Selectors

#### Element Selector
The element selector targets all elements of a specific type.

#### Example: Element Selector
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Element Selector Example</title>
    <style>
      p {
        color: blue; /* Styles all <p> elements */
      }
    </style>
  </head>
  <body>
    <p>This is a paragraph.</p>
    <p>This is another paragraph.</p>
  </body>
</html>
```

#### Class Selector
The class selector targets elements with a specific class.

#### Example: Class Selector
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Class Selector Example</title>
    <style>
      .highlight {
        background-color: yellow; /* Styles elements with the "highlight" class */
      }
    </style>
  </head>
  <body>
    <p class="highlight">This is a highlighted paragraph.</p>
    <p>This is a normal paragraph.</p>
  </body>
</html>
```

#### ID Selector
The ID selector targets a specific element by its ID.

#### Example: ID Selector
```html
<!DOCTYPE html>
<html>
  <head>
    <title>ID Selector Example</title>
    <style>
      #title {
        font-size: 24px; /* Styles the element with the ID "title" */
      }
    </style>
  </head>
  <body>
    <h1 id="title">Welcome to My Website</h1>
    <p>This is a paragraph.</p>
  </body>
</html>
```

### Descendant and Child Selectors

#### Descendant Selector
The descendant selector targets elements nested within another element.

#### Example: Descendant Selector
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Descendant Selector Example</title>
    <style>
      div p {
        color: green; /* Styles all <p> elements inside <div> */
      }
    </style>
  </head>
  <body>
    <div>
      <p>This is a paragraph inside a div.</p>
    </div>
    <p>This is a paragraph outside the div.</p>
  </body>
</html>
```

#### Child Selector
The child selector targets direct children of an element.

#### Example: Child Selector
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Child Selector Example</title>
    <style>
      div > p {
        color: red; /* Styles direct child <p> elements of <div> */
      }
    </style>
  </head>
  <body>
    <div>
      <p>This is a direct child paragraph.</p>
      <div>
        <p>This is a nested paragraph.</p>
      </div>
    </div>
  </body>
</html>
```

### Pseudo-Classes

#### `:hover`
The `:hover` pseudo-class applies styles when the user hovers over an element.

#### Example: Hover Effect
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Hover Example</title>
    <style>
      a:hover {
        color: red; /* Changes link color when hovered */
      }
    </style>
  </head>
  <body>
    <a href="#">Hover over this link</a>
  </body>
</html>
```

#### `:focus`
The `:focus` pseudo-class applies styles when an element gains focus (e.g., a text input).

#### Example: Focus Effect
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Focus Example</title>
    <style>
      input:focus {
        border-color: blue; /* Changes border color when focused */
      }
    </style>
  </head>
  <body>
    <input type="text" placeholder="Focus on me" />
  </body>
</html>
```

#### `:nth-child`
The `:nth-child` pseudo-class targets elements based on their position within a parent.

#### Example: nth-child Selector
```html
<!DOCTYPE html>
<html>
  <head>
    <title>nth-child Example</title>
    <style>
      li:nth-child(odd) {
        background-color: lightgray; /* Styles odd list items */
      }
      li:nth-child(even) {
        background-color: white; /* Styles even list items */
      }
    </style>
  </head>
  <body>
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
      <li>Item 4</li>
    </ul>
  </body>
</html>
```

### Selector Specificity and the Cascade
CSS specificity determines which styles are applied when multiple rules target the same element. The cascade resolves conflicts based on specificity, importance, and order.

#### Specificity Levels:
1. Inline styles (highest specificity).
2. ID selectors.
3. Class selectors.
4. Element selectors (lowest specificity).

#### Example: Specificity
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Specificity Example</title>
    <style>
      p {
        color: blue; /* Element selector */
      }
      .highlight {
        color: green; /* Class selector */
      }
      #title {
        color: red; /* ID selector */
      }
    </style>
  </head>
  <body>
    <p id="title" class="highlight">This is a paragraph.</p>
  </body>
</html>
```

#### Explanation:
- The ID selector (`#title`) overrides the class selector (`.highlight`) and element selector (`p`) due to higher specificity.

### Viewing Your Styled Webpage
To view your styled webpage:
1. Save the code as `index.html`.
2. Open the file in a web browser.

## Exercises
1. Create a webpage with:
   - A paragraph styled using an element selector.
   - A heading styled using an ID selector.
   - A list styled using a class selector.

2. Add hover effects to links on your webpage.

3. Use the `nth-child` pseudo-class to style odd and even rows in a table.

4. Experiment with specificity by combining element, class, and ID selectors.

## Summary
CSS selectors allow you to target and style HTML elements efficiently. Basic selectors include element, class, and ID selectors, while advanced selectors like descendant, child, and pseudo-classes provide more control. Understanding specificity and the cascade ensures your styles are applied correctly.

## Further Reading
- [CSS Selectors - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)
- [CSS Pseudo-classes - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes)
- [CSS Selectors Tutorial - W3Schools](https://www.w3schools.com/css/css_selectors.asp)
