# Styling Lists using CSS

Lists are a fundamental part of HTML, and CSS provides powerful tools to style and enhance them. In this guide, we will
explore various techniques for list styling, including using images as list styles and creating a navigation bar using
lists.

## Introduction

Lists in HTML come in two main flavors: ordered lists (`<ol>`) and unordered lists (`<ul>`). Both can be styled using
CSS to achieve a desired visual appearance. Additionally, you can create navigation bars and other interactive elements
by leveraging the flexibility of list styling.

## List Styling

### Styling Ordered Lists (`<ol>`) and Unordered Lists (`<ul>`)

You can style the basic list elements to enhance their appearance. For example, changing the list item marker and
adjusting margins and paddings can significantly impact the list's overall look.

```css
/* Styling unordered list */
ul {
  list-style-type: square; /* Change marker to a square */
}

/* Styling ordered list */
ol {
  list-style-type: decimal; /* Change marker to numbers */
}

/* Removing list marker */
ul.no-marker {
  list-style-type: none;
}
```

#### for unordered list list-style-type can be:

* `disc:` (default) - Filled circle marker
* `circle:` hollow circle marker
* `square:` a filled square marker
* `None:` No marker (remove bullets)

#### for ordered list list-style-type can be:

* `decimal:` (default) - Decimal numbers (1, 2, 3, etc.)
* `decimal-leading-zero:` Decimal numbers with leading zeros (01, 02, 03, etc.)
* `lower-roman:` lowercase Roman numbers (i, ii, iii,...)
* `upper-roman:` uppercase Roman numbers (I, II, III,...)
* `lower-alpha:` lowercase alphabetical letters (a, b, c, etc.)
* `upper-alpha:` uppercase alphabetical letters (A, B, C, etc.)

### Using Image as List Style

You can replace the default list item marker with a custom image to create a more visually appealing list.

```css
/* Using image as list style */
ul.image-list {
  list-style-image: url('bullet.png'); /* Replace marker with image */
}
```

### Using Emoji as Markers

You can use emojis as list item markers, adding a playful touch to your lists.

```CSS
/* Using emoji as list item marker */
ul.emoji-marker {
list-style-type: "🌟"; /* Use emoji as marker */
}
```

## Creating a Navbar Using List

Lists are often used to create navigation bars. By styling list items as inline or inline-block elements, you can create
a horizontal navigation menu.

```css
/* Styling navbar */
ul.navbar {
  list-style-type: none; /* Remove default list styles */
  margin: 0;
  padding: 0;
}

ul.navbar li {
  display: inline-block; /* Arrange items horizontally */
  margin-right: 10px;    /* Add right margin for spacing */
}
```

## Conclusion

Styling lists in CSS allows you to customize their appearance to match the design of your website. Whether it's changing
list item markers, using images, or creating navigation bars, CSS provides the flexibility needed for creative and
effective list styling. Experiment with these techniques to enhance the visual appeal and user experience of your web
pages.