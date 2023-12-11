# Id & Classes in HTML

## Introduction

In this section, we'll explore the concepts of IDs and classes, understanding how they serve as styling hooks for HTML elements. Additionally, we'll delve into a hands-on CSS demonstration to showcase the practical application of these styling techniques.

## Id and Classes

In CSS, both IDs and classes act as selectors, allowing you to apply styles to specific HTML elements.

### Id:

- An ID is a unique identifier for an HTML element.
- Applied using the `id` attribute: `<element id="uniqueId">`.
- Example: `<p id="introText">This is a unique paragraph.</p>`.

### Classes:

- Classes are reusable styling hooks that can be applied to multiple elements.
- Applied using the `class` attribute: `<element class="commonClass">`.
- Example: `<ul class="navigation">...</ul>`.

## CSS Demo

Let's dive into a practical CSS demonstration to see how IDs and classes come to life.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Demo</title>
    <style>
        /* Styling by ID */
        #introText {
            color: blue;
            font-size: 18px;
        }

        /* Styling by Class */
        .navigation {
            list-style-type: none;
            padding: 0;
            background-color: #f1f1f1;
        }

        .navItem {
            display: inline-block;
            padding: 10px 20px;
            text-decoration: none;
            color: #333;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <p id="introText">Welcome to the CSS Demo!</p>

    <ul class="navigation">
        <li class="navItem"><a href="#">Home</a></li>
        <li class="navItem"><a href="#">About</a></li>
        <li class="navItem"><a href="#">Contact</a></li>
    </ul>
</body>
</html>
```

In this demonstration:
- The text with the ID `introText` is styled with blue color and an increased font size.
- The navigation list with the class `navigation` has a gray background and no list-style.
- Each navigation item with the class `navItem` is styled as an inline block with padding, color, and bold font.

Feel free to experiment and modify the styles to see the immediate visual impact on the webpage.

As you continue your journey into CSS, these fundamental concepts of IDs and classes will serve as building blocks for creating visually appealing and well-styled web pages.