# CSS Display Property

## Introduction

The `display` property in CSS plays a pivotal role in shaping the layout and visibility of HTML elements on a webpage.
It is a versatile tool that determines how elements are rendered and how they interact with other elements.

## Inline & Block Properties

CSS elements fall into two primary categories: inline and block. The `display` property allows for defining these
fundamental characteristics.

### Inline Elements

Inline elements don't initiate a new line and occupy only as much width as necessary. Examples include `<span>`, `<a>`,
and `<img>`.

**Example:**

```css
span {
    display: inline;
}
```

### Block Elements

Block elements commence on a new line and expand to fill the entire available width. Examples encompass `<div>`, `<p>`,
and `<h1>`.

**Example:**

```css
div {
    display: block;
}
```

## Display None

The `display: none;` property serves the purpose of concealing an element entirely. This effectively removes the element
from the document flow, rendering it invisible and reclaiming the space it would occupy.

**Example:**

```css
.hide-element {
    display: none;
}
```

## Visibility

While `display: none;` completely eradicates an element, the `visibility` property provides a means to hide an element
while retaining its space in the layout.

**Example:**

```css
.invisible-element {
    visibility: hidden;
}
```

## Flexbox Example

Flexbox is a robust layout model that facilitates the creation of intricate layouts in a more efficient and predictable
manner. The `display: flex;` property initiates a flex container.

**Example:**

```css
.container {
    display: flex;
    justify-content: space-between;
}
```

## Grid

CSS Grid introduces a two-dimensional grid-based layout system. The `display: grid;` property transforms an element into
a grid container.

**Example:**

```css
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto;
}
```

## Precomposed Display Values

In CSS3, the `display` property provides precomposed values that offer convenient ways to control the layout and
behavior of elements. Let's explore some of these values with examples:

### `inline-block`

The `inline-block` value generates a block box that behaves like an inline element. It's useful when you want an element
to have block-level properties but still flow with surrounding content. Example:

```css
.inline-block-example {
  display: inline-block;
  width: 200px;
  height: 100px;
  background-color: lightblue;
  margin: 10px;
}
```

```html

<div class="inline-block-example">Inline Block</div>
```

### `inline-table`

The `inline-table` value behaves like an HTML `<table>` element but as an inline box rather than a block-level box. It
creates a table layout within an inline context. Example:

```css
.inline-table-example {
  display: inline-table;
  border: 1px solid black;
}
```

```html

<div class="inline-table-example">
    <div>Table Cell 1</div>
    <div>Table Cell 2</div>
</div>
```

### `inline-flex`

The `inline-flex` value makes an element behave like an inline-level element and lays out its content according to the
flexbox model. Example:

```css
.inline-flex-example {
  display: inline-flex;
  flex-direction: column;
  align-items: center;
  background-color: lightgreen;
  padding: 10px;
}
```

```html

<div class="inline-flex-example">
    <span>Flex Item 1</span>
    <span>Flex Item 2</span>
</div>
```

### `inline-grid`

The `inline-grid` value makes an element behave like an inline-level element and lays out its content according to the
grid model. Example:

```css
.inline-grid-example {
  display: inline-grid;
  grid-template-columns: repeat(3, 50px);
  gap: 5px;
}
```

```html

<div class="inline-grid-example">
    <div>Grid Item 1</div>
    <div>Grid Item 2</div>
    <div>Grid Item 3</div>
</div>
```

These examples showcase the use of precomposed values in the `display` property, providing flexibility in creating
diverse and responsive layouts. Keep in mind that browser support may vary, so it's essential to check compatibility
when using these features.

## Conclusion

Mastery of the CSS `display` property empowers developers to craft flexible and responsive layouts, elevating the design
and user experience of web pages. Whether dealing with inline, block, flex, or grid elements, a profound understanding
of how to leverage the `display` property is a fundamental skill in web development.