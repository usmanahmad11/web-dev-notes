# HTML Links and Images

## Introduction
Links and images are essential components of web pages. Links allow users to navigate between pages, while images enhance the visual appeal of a website. Understanding how to create hyperlinks and add images is crucial for building functional and accessible websites.

## Learning Objectives
By the end of this lecture, you will:
- Learn how to create hyperlinks using anchor (`<a>`) tags.
- Understand the difference between absolute and relative URLs.
- Learn how to add images using the `<img>` tag with proper `alt` text.
- Be able to resize images and ensure basic accessibility.

## Content

### Creating Hyperlinks with Anchor Tags
Hyperlinks are created using the `<a>` tag. The `href` attribute specifies the URL of the page or resource to link to.

#### Example: Basic Hyperlink
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Basic Hyperlink Example</title>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>Click <a href="https://www.example.com">here</a> to visit Example.com.</p>
  </body>
</html>
```

#### Explanation:
- `<a>`: Defines a hyperlink.
- `href`: Specifies the URL to navigate to when the link is clicked.
- The text between `<a>` and `</a>` is clickable.

### Absolute vs Relative URLs
URLs can be absolute or relative:
- **Absolute URLs**: Specify the full path to a resource, including the domain name.
  - Example: `https://www.example.com/page.html`
- **Relative URLs**: Specify the path relative to the current document.
  - Example: `page.html` (links to a file in the same folder).

#### Example: Relative URL
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Relative URL Example</title>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>Click <a href="about.html">here</a> to learn more about me.</p>
  </body>
</html>
```

#### Explanation:
- Relative URLs are useful for linking pages within the same website.

### Adding Images with Proper Alt Text
Images are added using the `<img>` tag. The `src` attribute specifies the image file's location, and the `alt` attribute provides alternative text for accessibility.

#### Example: Adding an Image
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Image Example</title>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <img src="example.jpg" alt="A beautiful landscape" />
  </body>
</html>
```

#### Explanation:
- `<img>`: Defines an image.
- `src`: Specifies the image file's location.
- `alt`: Provides a description of the image for screen readers and accessibility.

### Image Sizing and Basic Accessibility
You can resize images using the `width` and `height` attributes or CSS.

#### Example: Resizing an Image
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Image Resizing Example</title>
    <style>
      img {
        width: 300px; /* Sets the width to 300 pixels */
        height: auto; /* Maintains the aspect ratio */
      }
    </style>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <img src="example.jpg" alt="A beautiful landscape" />
  </body>
</html>
```

#### Explanation:
- `width` and `height` attributes can be used directly in the `<img>` tag or via CSS.
- Using `height: auto;` ensures the image maintains its original aspect ratio.

### Combining Links and Images
You can make images clickable by wrapping them in an `<a>` tag.

#### Example: Clickable Image
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Clickable Image Example</title>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <a href="https://www.example.com">
      <img src="example.jpg" alt="A beautiful landscape" />
    </a>
  </body>
</html>
```

#### Explanation:
- Wrapping an `<img>` tag inside an `<a>` tag makes the image a clickable link.

### Viewing Your HTML File
To view your links and images:
1. Save the code as `index.html`.
2. Place any referenced images (e.g., `example.jpg`) in the same folder.
3. Open `index.html` in a web browser.

## Exercises
1. Create an HTML file with:
   - A hyperlink to an external website using an absolute URL.
   - A hyperlink to another page in the same folder using a relative URL.

2. Add an image to your HTML file with:
   - Proper `alt` text describing the image.
   - CSS to resize the image to 400px wide while maintaining its aspect ratio.

3. Create a clickable image that links to an external website.

## Summary
Links and images are essential for creating functional and visually appealing web pages. Anchor tags (`<a>`) create hyperlinks, while the `<img>` tag adds images. Using proper `alt` text ensures accessibility, and resizing images improves layout and design.

## Further Reading
- [HTML Links - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a)
- [HTML Images - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img)
- [HTML Links and Images Tutorial - W3Schools](https://www.w3schools.com/html/html_links.asp)