# HTML Image, Lists, and Tables

## Introduction

Welcome to the in-depth exploration of HTML elements, where we'll unravel the intricacies of incorporating images,
organizing data with tables, and structuring content using lists. Understanding the nuances of these elements is crucial
for crafting visually appealing and well-organized web pages.

## HTML Image

Images are powerful visual elements that enhance the overall appeal of your web pages. The `<img>` element is used to
embed images, and it supports various attributes for customization:

```html
<img src="image.jpg" alt="A descriptive text for the image"
     width="300" height="200" title="Image Title">
```

- **`src`:** Specifies the source URL or file path of the image.
- **`alt`:** Provides alternative text for accessibility and SEO.
- **`width` and `height`:** Define the dimensions of the image.
- **`title`:** Adds a tooltip when the user hovers over the image.

## HTML Tables

Tables are fundamental for organizing and presenting data in a structured format. The basic structure of an HTML table
includes the `<table>`, `<tr>` (table row), `<td>` (table data/cell), and `<th>` (table header) elements:

```html

<table border="1">
    <tr>
        <th>Header 1</th>
        <th>Header 2</th>
    </tr>
    <tr>
        <td>Data 1</td>
        <td>Data 2</td>
    </tr>
</table>
```

- **`border`:** Sets the border thickness. Common values are 0 for no border and 1 for a thin border.

Additional attributes for customization:

- **`colspan` and `rowspan`:** Merge cells horizontally or vertically.
- **`align` and `valign`:** Align content horizontally and vertically.

## HTML Lists

Lists are versatile elements for organizing content. HTML supports ordered lists (`<ol>`), unordered lists (`<ul>`), and
list items (`<li>`):

### Ordered List:

```html

<ol type="1" start="3">
    <li>First item</li>
    <li>Second item</li>
</ol>
```

- **`type`:** Specifies the numbering style. Values include "1" (default), "A", "a", "I", "i".
- **`start`:** Defines the starting number.

### Unordered List:

```html

<ul>
    <li>Item 1</li>
    <li>Item 2</li>
</ul>
```

- **`type`:** Specifies the bullet style. Values include "disc" (default), "circle", "square".

## Conclusion

You've now delved into the details of HTML elements for images, tables, and lists. Understanding the attributes and
customization options empowers you to create visually appealing, well-structured web pages. In the upcoming sections,
we'll explore more HTML elements and dive deeper into the world of web development.
