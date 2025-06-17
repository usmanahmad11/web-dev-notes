# CSS Layout - Display and Positioning

## Introduction
CSS layout properties control how elements are displayed and positioned on a webpage. By understanding the `display` property, positioning methods, and stacking contexts, you can create flexible and visually appealing layouts. This lecture introduces the basics of CSS layout and positioning.

## Learning Objectives
By the end of this lecture, you will:
- Understand the `display` property and its values (`block`, `inline`, `inline-block`, `none`).
- Learn positioning methods: `static`, `relative`, `absolute`, and `fixed`.
- Understand the `z-index` property and stacking contexts.
- Create simple layouts using CSS.

## Content

### Display Property
The `display` property determines how an element is rendered on the page.

#### Common Values of `display`:
1. **`block`**: The element takes up the full width of its container.
2. **`inline`**: The element takes up only as much width as its content.
3. **`inline-block`**: Combines features of `inline` and `block` elements.
4. **`none`**: Hides the element completely.

#### Example: Display Property
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Display Property Example</title>
    <style>
      .block {
        display: block;
        background-color: lightblue;
        margin: 10px;
      }
      .inline {
        display: inline;
        background-color: lightgreen;
        margin: 10px;
      }
      .inline-block {
        display: inline-block;
        background-color: lightcoral;
        margin: 10px;
        width: 100px;
      }
      .none {
        display: none; /* Hides the element */
      }
    </style>
  </head>
  <body>
    <div class="block">Block Element</div>
    <span class="inline">Inline Element</span>
    <div class="inline-block">Inline-Block Element</div>
    <div class="none">Hidden Element</div>
  </body>
</html>
```

#### Explanation:
- `block`: Takes up the full width of the container.
- `inline`: Does not start on a new line and only takes up as much width as its content.
- `inline-block`: Behaves like `inline` but allows block-level styling (e.g., width, height).
- `none`: Removes the element from the layout.

### Positioning Methods
CSS provides four positioning methods to control the placement of elements.

#### Static Positioning
Static is the default positioning. Elements are placed in the normal document flow.

#### Example: Static Positioning
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Static Positioning Example</title>
    <style>
      div {
        background-color: lightblue;
        margin: 10px;
      }
    </style>
  </head>
  <body>
    <div>Static Positioning</div>
  </body>
</html>
```

#### Relative Positioning
Relative positioning moves an element relative to its normal position.

#### Example: Relative Positioning
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Relative Positioning Example</title>
    <style>
      div {
        position: relative;
        top: 20px; /* Moves the element down */
        left: 30px; /* Moves the element to the right */
        background-color: lightgreen;
      }
    </style>
  </head>
  <body>
    <div>Relative Positioning</div>
  </body>
</html>
```

#### Absolute Positioning
Absolute positioning places an element relative to its nearest positioned ancestor.

#### Example: Absolute Positioning
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Absolute Positioning Example</title>
    <style>
      .container {
        position: relative;
        background-color: lightgray;
        width: 300px;
        height: 200px;
      }
      .absolute {
        position: absolute;
        top: 50px;
        left: 50px;
        background-color: lightcoral;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="absolute">Absolute Positioning</div>
    </div>
  </body>
</html>
```

#### Explanation:
- The `.absolute` element is positioned relative to the `.container` element.

#### Fixed Positioning
Fixed positioning places an element relative to the viewport and does not move when scrolling.

#### Example: Fixed Positioning
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Fixed Positioning Example</title>
    <style>
      .fixed {
        position: fixed;
        top: 10px;
        right: 10px;
        background-color: lightblue;
      }
    </style>
  </head>
  <body>
    <div class="fixed">Fixed Positioning</div>
    <p>Scroll down to see the fixed element stay in place.</p>
    <p style="margin-top: 1000px;">End of page</p>
  </body>
</html>
```

#### Explanation:
- The `.fixed` element remains in the same position regardless of scrolling.

### Z-Index and Stacking Contexts
The `z-index` property controls the stacking order of elements. Higher values appear on top of lower values.

#### Example: Z-Index
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Z-Index Example</title>
    <style>
      .box1 {
        position: absolute;
        top: 50px;
        left: 50px;
        width: 100px;
        height: 100px;
        background-color: lightblue;
        z-index: 1; /* Lower stacking order */
      }
      .box2 {
        position: absolute;
        top: 70px;
        left: 70px;
        width: 100px;
        height: 100px;
        background-color: lightgreen;
        z-index: 2; /* Higher stacking order */
      }
    </style>
  </head>
  <body>
    <div class="box1">Box 1</div>
    <div class="box2">Box 2</div>
  </body>
</html>
```

#### Explanation:
- `z-index: 2` makes `.box2` appear on top of `.box1`.

### Creating Simple Layouts
Combine `display` and positioning properties to create layouts.

#### Example: Simple Layout
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Simple Layout Example</title>
    <style>
      header {
        background-color: lightblue;
        text-align: center;
        padding: 10px;
      }
      nav {
        background-color: lightgray;
        padding: 10px;
      }
      main {
        background-color: white;
        padding: 20px;
      }
      footer {
        background-color: lightblue;
        text-align: center;
        padding: 10px;
        position: fixed;
        bottom: 0;
        width: 100%;
      }
    </style>
  </head>
  <body>
    <header>Header</header>
    <nav>Navigation</nav>
    <main>Main Content</main>
    <footer>Footer</footer>
  </body>
</html>
```

### Viewing Your Styled Webpage
To view your styled webpage:
1. Save the code as `index.html`.
2. Open the file in a web browser.

## Exercises
1. Create a webpage with:
   - A block element and an inline element.
   - An element positioned relative to its normal position.

2. Create a container with an absolutely positioned child element.

3. Add a fixed header and footer to a webpage.

4. Experiment with `z-index` by overlapping two elements.

## Summary
CSS layout properties like `display` and positioning (`static`, `relative`, `absolute`, `fixed`) control how elements are rendered and placed on a webpage. The `z-index` property manages stacking order, while combining these techniques allows you to create flexible layouts.

## Further Reading
- [CSS Display - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/display)
- [CSS Position - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/position)
- [CSS Z-Index - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/z-index)