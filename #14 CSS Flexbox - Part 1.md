# CSS Flexbox - Part 1

## Introduction
Flexbox (Flexible Box Layout) is a CSS layout model designed to provide efficient alignment, distribution, and spacing of elements within a container. It simplifies the process of creating responsive layouts and is widely used in modern web design.

## Learning Objectives
By the end of this lecture, you will:
- Understand the basics of Flexbox and its purpose.
- Learn about flex containers and flex items.
- Understand the concepts of the main axis and cross axis.
- Use `justify-content` and `align-items` to align and distribute flex items.

## Content

### Introduction to Flexbox
Flexbox is a one-dimensional layout model that organizes items along a single axis (either horizontally or vertically). It is ideal for creating layouts where items need to be aligned, spaced, or resized dynamically.

#### Key Features of Flexbox:
- Align items horizontally or vertically.
- Distribute space between items.
- Resize items to fit available space.

### Flex Container and Flex Items
Flexbox works by designating a parent element as a **flex container**. The child elements inside the container become **flex items**.

#### Example: Flex Container and Flex Items
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Flex Container Example</title>
    <style>
      .container {
        display: flex; /* Makes the container a flex container */
        background-color: lightgray;
        padding: 10px;
      }
      .item {
        background-color: lightblue;
        margin: 5px;
        padding: 10px;
        width: 100px;
        text-align: center;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="item">Item 1</div>
      <div class="item">Item 2</div>
      <div class="item">Item 3</div>
    </div>
  </body>
</html>
```

#### Explanation:
- `display: flex;` turns the `.container` into a flex container.
- The `.item` elements become flex items and are aligned horizontally by default.

### Main Axis and Cross Axis Concepts
Flexbox organizes items along two axes:
1. **Main Axis**: The primary axis along which items are placed. It is horizontal by default.
2. **Cross Axis**: The perpendicular axis to the main axis. It is vertical by default.

#### Example: Main Axis and Cross Axis
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Main and Cross Axis Example</title>
    <style>
      .container {
        display: flex;
        height: 200px;
        background-color: lightgray;
      }
      .item {
        background-color: lightblue;
        margin: 5px;
        padding: 10px;
        text-align: center;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="item">Item 1</div>
      <div class="item">Item 2</div>
      <div class="item">Item 3</div>
    </div>
  </body>
</html>
```

#### Explanation:
- The main axis is horizontal, and items are aligned side by side.
- The cross axis is vertical, and items can be aligned along this axis using additional properties.

### Justify-Content
The `justify-content` property aligns flex items along the main axis.

#### Common Values of `justify-content`:
1. **`flex-start`**: Aligns items at the start of the main axis (default).
2. **`flex-end`**: Aligns items at the end of the main axis.
3. **`center`**: Centers items along the main axis.
4. **`space-between`**: Distributes items with equal space between them.
5. **`space-around`**: Distributes items with equal space around them.

#### Example: Justify-Content
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Justify-Content Example</title>
    <style>
      .container {
        display: flex;
        justify-content: space-between; /* Distributes items with equal space between */
        background-color: lightgray;
        padding: 10px;
      }
      .item {
        background-color: lightblue;
        margin: 5px;
        padding: 10px;
        text-align: center;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="item">Item 1</div>
      <div class="item">Item 2</div>
      <div class="item">Item 3</div>
    </div>
  </body>
</html>
```

#### Explanation:
- `justify-content: space-between;` distributes items evenly with space between them.

### Align-Items
The `align-items` property aligns flex items along the cross axis.

#### Common Values of `align-items`:
1. **`flex-start`**: Aligns items at the start of the cross axis.
2. **`flex-end`**: Aligns items at the end of the cross axis.
3. **`center`**: Centers items along the cross axis.
4. **`stretch`**: Stretches items to fill the container (default).

#### Example: Align-Items
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Align-Items Example</title>
    <style>
      .container {
        display: flex;
        align-items: center; /* Centers items along the cross axis */
        height: 200px;
        background-color: lightgray;
      }
      .item {
        background-color: lightblue;
        margin: 5px;
        padding: 10px;
        text-align: center;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="item">Item 1</div>
      <div class="item">Item 2</div>
      <div class="item">Item 3</div>
    </div>
  </body>
</html>
```

#### Explanation:
- `align-items: center;` vertically centers items within the container.

### Viewing Your Styled Webpage
To view your styled webpage:
1. Save the code as `index.html`.
2. Open the file in a web browser.

## Exercises
1. Create a flex container with three items:
   - Use `justify-content: space-around` to distribute items.
   - Use `align-items: flex-end` to align items at the bottom of the container.

2. Experiment with different values of `justify-content` and `align-items` to see their effects.

3. Create a flex container with a height of 300px and center items both horizontally and vertically.

## Summary
Flexbox simplifies layout creation by aligning and distributing items efficiently. The `justify-content` property aligns items along the main axis, while `align-items` aligns items along the cross axis. Understanding these concepts is essential for building responsive and flexible layouts.

## Further Reading
- [CSS Flexbox - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout)
- [CSS Flexbox Tutorial - W3Schools](https://www.w3schools.com/css/css3_flexbox.asp)
- [Learn Flexbox - freeCodeCamp](https://www.freecodecamp.org/news/an-animated-guide-to-flexbox/)
