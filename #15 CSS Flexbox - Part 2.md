# CSS Flexbox - Part 2

## Introduction
In this lecture, we will dive deeper into Flexbox properties, including `flex-direction`, `flex-wrap`, `align-self`, and the flex properties (`flex-grow`, `flex-shrink`, and `flex-basis`). You will also learn how to build responsive navigation bars and explore common Flexbox patterns.

## Learning Objectives
By the end of this lecture, you will:
- Understand how `flex-direction` and `flex-wrap` control the layout of flex items.
- Learn how `align-self` and the flex properties (`flex-grow`, `flex-shrink`, `flex-basis`) work.
- Build a responsive navigation bar using Flexbox.
- Explore common Flexbox patterns for layouts.

## Content

### Flex-Direction
The `flex-direction` property defines the direction of the main axis and the order of flex items.

#### Common Values of `flex-direction`:
1. **`row`** (default): Items are placed horizontally, left to right.
2. **`row-reverse`**: Items are placed horizontally, right to left.
3. **`column`**: Items are placed vertically, top to bottom.
4. **`column-reverse`**: Items are placed vertically, bottom to top.

#### Example: Flex-Direction
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Flex-Direction Example</title>
    <style>
      .container {
        display: flex;
        flex-direction: column; /* Changes direction to vertical */
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
- `flex-direction: column;` arranges items vertically instead of horizontally.

### Flex-Wrap
The `flex-wrap` property controls whether flex items wrap onto multiple lines when they exceed the container's width.

#### Common Values of `flex-wrap`:
1. **`nowrap`** (default): Items stay on a single line.
2. **`wrap`**: Items wrap onto multiple lines.
3. **`wrap-reverse`**: Items wrap onto multiple lines in reverse order.

#### Example: Flex-Wrap
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Flex-Wrap Example</title>
    <style>
      .container {
        display: flex;
        flex-wrap: wrap; /* Allows items to wrap onto multiple lines */
        background-color: lightgray;
      }
      .item {
        background-color: lightblue;
        margin: 5px;
        padding: 10px;
        width: 150px; /* Fixed width for items */
        text-align: center;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="item">Item 1</div>
      <div class="item">Item 2</div>
      <div class="item">Item 3</div>
      <div class="item">Item 4</div>
      <div class="item">Item 5</div>
    </div>
  </body>
</html>
```

#### Explanation:
- `flex-wrap: wrap;` allows items to wrap onto the next line when they exceed the container's width.

### Align-Self
The `align-self` property allows individual flex items to override the `align-items` property of the container.

#### Common Values of `align-self`:
1. **`auto`** (default): Inherits the container's `align-items` value.
2. **`flex-start`**: Aligns the item at the start of the cross axis.
3. **`flex-end`**: Aligns the item at the end of the cross axis.
4. **`center`**: Centers the item along the cross axis.
5. **`stretch`**: Stretches the item to fill the container.

#### Example: Align-Self
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Align-Self Example</title>
    <style>
      .container {
        display: flex;
        align-items: center; /* Centers all items by default */
        height: 200px;
        background-color: lightgray;
      }
      .item {
        background-color: lightblue;
        margin: 5px;
        padding: 10px;
        text-align: center;
      }
      .item:nth-child(2) {
        align-self: flex-end; /* Overrides the container's alignment */
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
- `align-self: flex-end;` aligns the second item at the bottom of the container.

### Flex-Grow, Flex-Shrink, and Flex-Basis
The `flex` shorthand property combines `flex-grow`, `flex-shrink`, and `flex-basis` to control how flex items grow, shrink, and set their initial size.

#### Example: Flex Properties
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Flex Properties Example</title>
    <style>
      .container {
        display: flex;
        background-color: lightgray;
      }
      .item {
        background-color: lightblue;
        margin: 5px;
        padding: 10px;
        text-align: center;
        flex: 1; /* All items grow equally */
      }
      .item:nth-child(2) {
        flex: 2; /* Second item grows twice as much */
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
- `flex: 1;` makes all items grow equally.
- `flex: 2;` makes the second item grow twice as much as the others.

### Building Responsive Navigation Bars
Flexbox is ideal for creating responsive navigation bars.

#### Example: Responsive Navigation Bar
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Responsive Navigation Bar</title>
    <style>
      nav {
        display: flex;
        justify-content: space-around; /* Distributes links evenly */
        background-color: lightblue;
        padding: 10px;
      }
      a {
        text-decoration: none;
        color: black;
        padding: 10px;
      }
    </style>
  </head>
  <body>
    <nav>
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#contact">Contact</a>
    </nav>
  </body>
</html>
```

#### Explanation:
- `justify-content: space-around;` ensures equal spacing between navigation links.

### Common Flexbox Patterns
Flexbox can be used to create various layout patterns, such as:
1. **Centered Content**:
   ```css
   display: flex;
   justify-content: center;
   align-items: center;
   ```
2. **Two-Column Layout**:
   ```css
   display: flex;
   flex-direction: row;
   justify-content: space-between;
   ```
3. **Responsive Grid**:
   ```css
   display: flex;
   flex-wrap: wrap;
   ```

### Viewing Your Styled Webpage
To view your styled webpage:
1. Save the code as `index.html`.
2. Open the file in a web browser.

## Exercises
1. Create a flex container with:
   - Items arranged vertically using `flex-direction: column`.
   - Items wrapping onto multiple lines using `flex-wrap: wrap`.

2. Use `align-self` to align one item differently from the others.

3. Build a responsive navigation bar with links spaced evenly.

4. Experiment with `flex-grow` and `flex-shrink` to control item sizes.

## Summary
Flexbox provides powerful tools for creating responsive layouts. Properties like `flex-direction`, `flex-wrap`, `align-self`, and `flex-grow/shrink/basis` allow you to control the arrangement and sizing of flex items. By mastering these properties, you can build flexible and modern web designs.

## Further Reading
- [CSS Flexbox - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout)
- [CSS Flexbox Tutorial - W3Schools](https://www.w3schools.com/css/css3_flexbox.asp)
- [Flexbox Patterns - CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
