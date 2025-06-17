# CSS Colors and Typography

## Introduction
Colors and typography are essential aspects of web design that influence the visual appeal and readability of a website. CSS provides powerful tools to style text and backgrounds, control fonts, and align text. Learning these properties will help you create visually engaging and professional-looking websites.

## Learning Objectives
By the end of this lecture, you will:
- Understand how to use CSS color properties like `color` and `background-color`.
- Learn font properties such as `font-family`, `font-size`, and `font-weight`.
- Use text properties like `text-align`, `text-decoration`, and `line-height`.
- Understand web-safe fonts and font stacks.

## Content

### CSS Color Properties
CSS allows you to style text and backgrounds using color properties.

#### `color` Property
The `color` property sets the text color.

#### Example: Text Color
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Text Color Example</title>
    <style>
      h1 {
        color: blue; /* Sets text color to blue */
      }
      p {
        color: gray; /* Sets text color to gray */
      }
    </style>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph with styled text color.</p>
  </body>
</html>
```

#### `background-color` Property
The `background-color` property sets the background color of an element.

#### Example: Background Color
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Background Color Example</title>
    <style>
      h1 {
        background-color: yellow; /* Sets background color to yellow */
      }
      p {
        background-color: lightgray; /* Sets background color to light gray */
      }
    </style>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph with styled background color.</p>
  </body>
</html>
```

#### Explanation:
- Colors can be specified using names (`blue`, `gray`), hexadecimal codes (`#0000FF`), RGB values (`rgb(0, 0, 255)`), or HSL values (`hsl(240, 100%, 50%)`).

### CSS Font Properties
Font properties control the appearance of text, including its size, weight, and family.

#### `font-family` Property
The `font-family` property specifies the font to use for text.

#### Example: Font Family
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Font Family Example</title>
    <style>
      h1 {
        font-family: Arial, sans-serif; /* Sets font to Arial */
      }
      p {
        font-family: "Times New Roman", serif; /* Sets font to Times New Roman */
      }
    </style>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph with styled font family.</p>
  </body>
</html>
```

#### Explanation:
- Use web-safe fonts like Arial, Verdana, and Times New Roman.
- Font stacks provide fallback options if the primary font is unavailable.

#### `font-size` Property
The `font-size` property sets the size of text.

#### Example: Font Size
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Font Size Example</title>
    <style>
      h1 {
        font-size: 32px; /* Sets font size to 32 pixels */
      }
      p {
        font-size: 18px; /* Sets font size to 18 pixels */
      }
    </style>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph with styled font size.</p>
  </body>
</html>
```

#### `font-weight` Property
The `font-weight` property controls the thickness of text.

#### Example: Font Weight
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Font Weight Example</title>
    <style>
      h1 {
        font-weight: bold; /* Makes text bold */
      }
      p {
        font-weight: normal; /* Sets text to normal weight */
      }
    </style>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph with styled font weight.</p>
  </body>
</html>
```

### CSS Text Properties
Text properties control alignment, decoration, and spacing.

#### `text-align` Property
The `text-align` property aligns text horizontally.

#### Example: Text Alignment
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Text Alignment Example</title>
    <style>
      h1 {
        text-align: center; /* Centers text */
      }
      p {
        text-align: justify; /* Justifies text */
      }
    </style>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph with styled text alignment.</p>
  </body>
</html>
```

#### `text-decoration` Property
The `text-decoration` property adds or removes decorations like underlines.

#### Example: Text Decoration
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Text Decoration Example</title>
    <style>
      a {
        text-decoration: none; /* Removes underline from links */
      }
    </style>
  </head>
  <body>
    <a href="#">Click Here</a>
  </body>
</html>
```

#### `line-height` Property
The `line-height` property controls the spacing between lines of text.

#### Example: Line Height
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Line Height Example</title>
    <style>
      p {
        line-height: 1.5; /* Sets line spacing to 1.5 times the font size */
      }
    </style>
  </head>
  <body>
    <p>This is a paragraph with styled line height. The spacing between lines is increased for better readability.</p>
  </body>
</html>
```

### Web-Safe Fonts and Font Stacks
Web-safe fonts are widely supported across browsers and devices. Font stacks provide fallback options.

#### Example: Font Stack
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Font Stack Example</title>
    <style>
      p {
        font-family: "Helvetica", "Arial", sans-serif; /* Font stack with fallback options */
      }
    </style>
  </head>
  <body>
    <p>This is a paragraph with a font stack.</p>
  </body>
</html>
```

#### Explanation:
- The browser uses the first available font in the stack.

### Viewing Your Styled Webpage
To view your styled webpage:
1. Save the code as `index.html`.
2. Open the file in a web browser.

## Exercises
1. Create a webpage with:
   - A heading styled with a blue text color and a yellow background.
   - A paragraph styled with a font size of 20px and a bold font weight.

2. Add a link to your webpage and remove its underline using `text-decoration`.

3. Experiment with different font stacks and line heights to improve readability.

## Summary
CSS provides powerful tools for styling colors and typography. Properties like `color`, `background-color`, `font-family`, `font-size`, `font-weight`, `text-align`, `text-decoration`, and `line-height` allow you to control the appearance and readability of text. Using web-safe fonts and font stacks ensures consistent styling across devices.

## Further Reading
- [CSS Colors - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/color)
- [CSS Fonts - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family)
- [CSS Typography Tutorial - W3Schools](https://www.w3schools.com/css/css_font.asp)