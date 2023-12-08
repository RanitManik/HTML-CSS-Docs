# CSS Inheritance

In CSS, inheritance is a mechanism that enables certain properties of an element to be passed down from its parent to
its children. This can greatly simplify styling, as properties defined for a parent element can automatically apply to
its descendants.

## How Inheritance Works

Not all CSS properties are inherited. Only specific properties, such as `color`, `font-size`, `line-height`, and others,
are inherited by default. However, many properties, especially those related to layout and positioning, are not
inherited.

When an element does not have a specified value for an inherited property, it inherits the value of that property from
its parent. This process continues up the chain until the root element is reached.

## Example of Inheritance

Let's consider an example to illustrate inheritance:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        body {
            font-family: Arial, sans-serif;
            font-size: 16px;
            color: #333;
        }

        h1 {
            color: #ff4500; /* Overrides the inherited color property */
        }

        p {
            line-height: 1.5; /* Inherits the font-size and color from the body */
        }
    </style>
</head>
<body>
<h1>Welcome to my Website</h1>
<p>This is a paragraph with some text.</p>
</body>
</html>
```

In this example:

- The `body` element sets a default `font-family`, `font-size`, and `color`.
- The `h1` element overrides the inherited `color` property to `#ff4500`.
- The `p` element inherits the `font-size` and `color` from the `body` element.

## Using `inherit` Keyword

The `inherit` keyword can be explicitly used to force an element to inherit a property from its parent, even if it has a
specific value defined.

```css
p {
    color: blue; /* Specific color for paragraphs */
}

span {
    color: inherit; /* Inherit the color property from the parent (body or a containing element) */
}
```

In this case, the `span` element within a `p` element will inherit the color from its parent `p`, which, in turn,
inherits it from the `body`.

## Non-Inherited Properties

Not all properties are inherited by default. Properties related to layout, such
as `width`, `height`, `margin`, `padding`, and others, are generally not inherited. Each element must explicitly define
these properties.

Understanding inheritance is crucial in creating a consistent and maintainable stylesheet. It allows developers to
establish global styles at higher levels in the document structure and then fine-tune styles for specific elements as
needed.