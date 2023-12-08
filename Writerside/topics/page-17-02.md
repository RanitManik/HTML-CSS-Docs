# Pseudo Selectors

## Pseudo-class Selectors

Pseudo-class selectors in CSS allow you to style elements based on their state or interaction. These selectors add a
layer of dynamism to your stylesheets, enabling you to create visually engaging and responsive designs.

### :hover Pseudo-class

The `:hover` pseudo-class selects and styles an element when the user hovers over it.

```css
/* Styles the text color of a link when hovered */
a:hover {
    color: purple;
}
```

In this example, the text color of a link changes to purple when it is hovered over.

### :active Pseudo-class

The `:active` pseudo-class selects and styles an element while it is being activated or clicked.

```css
/* Styles the background color of a button while being clicked */
button:active {
    background-color: #ff4500;
}
```

Here, the background color of a button changes to a shade of orange when it is clicked.

### :focus Pseudo-class

The `:focus` pseudo-class selects and styles an element that has received focus.

```css
/* Styles the border of a text input when it is in focus */
input:focus {
    border: 2px solid blue;
}
```

This rule adds a blue border to a text input when it is in focus.

### :nth-child Pseudo-class

The `:nth-child` pseudo-class selects and styles elements based on their position within a parent.

```css
/* Styles every second paragraph within a section */
section p:nth-child(2n) {
    font-weight: bold;
}
```

This example makes every second paragraph within a section bold.

### :not Pseudo-class

The `:not` pseudo-class selects and styles elements that do not match a specified selector.

```css
/* Styles all list items except the first one */
li:not(:first-child) {
    color: gray;
}
```

Here, all list items except the first one will have a gray text color.

---

## Pseudo-element Selectors

Pseudo-elements in CSS allow you to style a specific part of an element, adding more granularity to your designs.

### ::before Pseudo-element

The `::before` pseudo-element inserts content before the actual content of an element.

```css
/* Adds a decorative symbol before each paragraph */
p::before {
    content: "🔸";
}
```

This rule adds a small diamond symbol before each paragraph.

### ::after Pseudo-element

The `::after` pseudo-element inserts content after the actual content of an element.

```css
/* Adds a decorative line after each heading */
h2::after {
    content: "__________________";
    display: block;
    color: #999;
}
```

Here, a line is added after each heading for decorative purposes.

### ::first-line Pseudo-element

The `::first-line` pseudo-element selects and styles the first line of a block-level element.

```css
/* Styles the first line of a paragraph differently */
p::first-line {
    font-weight: bold;
    color: blue;
}
```

This example makes the first line of a paragraph bold and blue.

### ::selection Pseudo-element

The `::selection` pseudo-element selects and styles the portion of text that is selected by the user.

```css
/* Styles the background color of selected text */
::selection {
    background-color: yellow;
    color: black;
}
```

In this case, selected text will have a yellow background and black text color.

### Conclusion

Pseudo-class and pseudo-element selectors in CSS provide advanced styling capabilities, allowing you to respond to user
interactions and enhance the visual appeal of your web pages. By leveraging these selectors, you can create dynamic and
polished designs that adapt to different states and highlight specific elements.