# HTML Tables

## Introduction
Tables in HTML are used to organize data in rows and columns. They are ideal for displaying structured information, such as schedules, pricing tables, or comparison charts. Understanding how to create and style tables is essential for presenting data effectively.

## Learning Objectives
By the end of this lecture, you will:
- Understand the basic structure of an HTML table using `<table>`, `<tr>`, `<td>`, and `<th>` tags.
- Learn how to add headers and captions to tables.
- Use `colspan` and `rowspan` attributes to merge cells.
- Understand when and how to use tables properly in web development.

## Content

### Table Structure (`<table>`, `<tr>`, `<td>`, `<th>`)
An HTML table is created using the `<table>` tag. Rows are defined using `<tr>`, cells using `<td>`, and headers using `<th>`.

#### Example: Basic Table
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Basic Table Example</title>
  </head>
  <body>
    <h1>Student Grades</h1>
    <table border="1">
      <tr>
        <th>Name</th> <!-- Header cell -->
        <th>Grade</th>
      </tr>
      <tr>
        <td>John</td> <!-- Data cell -->
        <td>A</td>
      </tr>
      <tr>
        <td>Jane</td>
        <td>B</td>
      </tr>
    </table>
  </body>
</html>
```

#### Explanation:
- `<table>`: Defines the table.
- `<tr>`: Defines a row.
- `<td>`: Defines a data cell.
- `<th>`: Defines a header cell, which is bold and centered by default.
- `border="1"`: Adds a border to the table for better visibility.

### Table Headers and Captions
Headers provide context for the table's data, while captions describe the table's purpose.

#### Example: Table with Caption
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Table with Caption Example</title>
  </head>
  <body>
    <h1>Monthly Sales Report</h1>
    <table border="1">
      <caption>Sales Data for January</caption> <!-- Table caption -->
      <tr>
        <th>Product</th>
        <th>Quantity</th>
        <th>Revenue</th>
      </tr>
      <tr>
        <td>Apples</td>
        <td>50</td>
        <td>$100</td>
      </tr>
      <tr>
        <td>Bananas</td>
        <td>30</td>
        <td>$60</td>
      </tr>
    </table>
  </body>
</html>
```

#### Explanation:
- `<caption>`: Provides a title for the table.
- Captions are displayed above the table by default.

### Colspan and Rowspan Attributes
The `colspan` and `rowspan` attributes are used to merge cells across columns or rows.

#### Example: Using Colspan
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Colspan Example</title>
  </head>
  <body>
    <h1>Schedule</h1>
    <table border="1">
      <tr>
        <th colspan="2">Monday</th> <!-- Merges two columns -->
      </tr>
      <tr>
        <td>Morning</td>
        <td>Afternoon</td>
      </tr>
    </table>
  </body>
</html>
```

#### Example: Using Rowspan
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Rowspan Example</title>
  </head>
  <body>
    <h1>Schedule</h1>
    <table border="1">
      <tr>
        <th>Day</th>
        <th>Activity</th>
      </tr>
      <tr>
        <td rowspan="2">Monday</td> <!-- Merges two rows -->
        <td>Morning</td>
      </tr>
      <tr>
        <td>Afternoon</td>
      </tr>
    </table>
  </body>
</html>
```

#### Explanation:
- `colspan="2"`: Merges two columns into one cell.
- `rowspan="2"`: Merges two rows into one cell.

### When and How to Use Tables Properly
Tables should be used for tabular data, not for layout purposes. Modern CSS techniques (e.g., Flexbox, Grid) are better suited for page layouts. Use tables when:
- You need to display structured data.
- The data is best understood in rows and columns.

### Viewing Your HTML File
To view your table:
1. Save the code as `index.html`.
2. Open the file in a web browser.

## Exercises
1. Create a table with:
   - Three columns: "Name," "Age," and "City."
   - Three rows of data.

2. Add a caption to the table describing its purpose.

3. Create a table with:
   - A header row that spans two columns using `colspan`.
   - A cell that spans two rows using `rowspan`.

## Summary
HTML tables organize data in rows and columns using `<table>`, `<tr>`, `<td>`, and `<th>` tags. Captions provide context, while `colspan` and `rowspan` attributes allow merging cells. Tables should be used for structured data, not for layout purposes.

## Further Reading
- [HTML Tables - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/table)
- [HTML Tables Tutorial - W3Schools](https://www.w3schools.com/html/html_tables.asp)
- [Accessible Tables - WebAIM](https://webaim.org/techniques/tables/)