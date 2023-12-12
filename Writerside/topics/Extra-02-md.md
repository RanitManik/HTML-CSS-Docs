# CSS Z-index and Order

In CSS, `z-index` and the `order` property are used to control the stacking order of elements, but they are applied in
different contexts.

### `z-index`

The `z-index` property is used to control the stacking order of positioned elements along the z-axis. Elements with a
higher `z-index` value are stacked above elements with a lower value. If two elements have the same `z-index`, their
stacking order is determined by their order in the HTML document (the element that comes later in the document will be
stacked on top).

**Example**

```css
div {
  position: absolute;
  z-index: 2;
}

p {
  position: absolute;
  z-index: 1;
}
```

In this example, the `div` with a `z-index` of 2 will be stacked above the `p` with a `z-index` of 1.

### `order`

The `order` property is part of Flexbox and Grid layout systems and is used to specify the order of flex or grid items
within their container. It does not affect the stacking order along the z-axis.

**Example (Flexbox)**

```css
.container {
  display: flex;
}

.item1 {
  order: 2;
}

.item2 {
  order: 1;
}
```

In this example, `item1` will be displayed before `item2` in the flex container, despite the default order in the HTML.

It's important to note that the `order` property only works within a flex container or a grid container. If you're not
using Flexbox or Grid, it won't have any effect.

### Combining `z-index` and `order`

If you're working with a combination of positioned elements and Flexbox/Grid layouts, it's important to understand
that `z-index` and `order` operate independently of each other. `z-index` influences the stacking order in the z-axis
for positioned elements, while `order` influences the order of flex/grid items within their containers.

**Example**

```css
.container {
  position: relative;
}

.item1 {
  position: absolute;
  z-index: 2;
}

.item2 {
  position: absolute;
  z-index: 1;
}

.flex-container {
  display: flex;
}

.flex-item1 {
  order: 2;
}

.flex-item2 {
  order: 1;
}
```

In this example, the `item1` with a higher `z-index` will be stacked above `item2` in the z-axis, regardless of their
order in the HTML. Meanwhile, within the Flexbox container, `flex-item1` will be visually displayed after `flex-item2`
based on their `order` values.

Understanding how `z-index` and `order` work in their respective contexts allows you to control both the stacking and
visual order of elements, providing flexibility in designing complex layouts.