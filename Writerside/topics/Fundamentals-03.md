# HTML Fundamentals

## Introduction

In the ever-evolving landscape of web development, understanding the core concepts of HTML is essential. This guide will
walk you through the fundamental building blocks of an HTML file, the importance of attributes, and a handy tip for
mobile preview.

## Basic Structure of an HTML File

HTML (HyperText Markup Language) is the backbone of web development. Let's dissect the basic structure of an HTML file:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Page Title</title>
</head>
<body>
<!-- Your content goes here -->
</body>
</html>
```

- `<!DOCTYPE html>`: Declares the HTML version.
- `<html lang="en">`: Defines the document as HTML and sets the language to English.
- `<head>`: Contains meta-information about the document.
- `<meta charset="UTF-8">`: Specifies the character encoding.
- `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Configures the viewport for mobile
  responsiveness.
- `<title>`: Sets the title of the page, displayed in the browser tab.
- `<body>`: Contains the content of the HTML document.

## HTML Attributes

Attributes provide additional information about HTML elements and help control their behavior. Common attributes
include:

- **class:** Adds a class to an element for styling or JavaScript interaction.
  ```html
  <p class="important-text">This is important!</p>
  ```

- **id:** Gives a unique identifier to an element for targeted styling or scripting.
  ```html
  <div id="header">Page Header</div>
  ```

- **src:** Specifies the source (e.g., a URL or file path) for elements like images or scripts.
  ```html
  <img src="image.jpg" alt="A beautiful image">
  ```

## Mobile Preview Tip

As you develop your web pages, it's crucial to preview how they'll appear on mobile devices. Use the following tip to
simulate a mobile view in your browser:

1. Open your webpage in Google Chrome.
2. Right-click on the page and select "Inspect" to open the Developer Tools.
3. Toggle the device toolbar icon (or press `Ctrl + Shift + M`) to simulate various device sizes.

This mobile preview feature helps you ensure a responsive design for users on different devices.

Stay tuned for more insights into HTML and web development on the next page!
