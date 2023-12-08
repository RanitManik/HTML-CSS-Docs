# CSS Grid

CSS Grid is a powerful layout system that allows developers to create complex two-dimensional layouts with ease. It
provides precise control over the positioning and sizing of elements in a grid-based structure. Let's explore the key
concepts and properties of CSS Grid.

## Introduction

CSS Grid Layout, often referred to as Grid, is a layout system designed for the arrangement of elements in a
two-dimensional grid. It enables the creation of complex and responsive layouts by dividing a container into rows and
columns.

## Grid Container and Grid Items

- **Grid Container:** The parent element becomes a grid container by setting its `display` property to `grid`
  or `inline-grid`. This establishes a grid formatting context for its children.

    ```css
    .grid-container {
        display: grid; /* or inline-grid */
    }
    ```

- **Grid Items:** The direct children of a grid container are referred to as grid items. These items are placed within
  the grid defined by the container.

    ```css
    .grid-item {
        /* Styles for grid items */
    }
    ```

## Grid Template Columns and Rows

The `grid-template-columns` and `grid-template-rows` properties define the size of columns and rows in the grid. They
accept values like length units, percentages, or the `fr` unit (fraction of available space).

```css
.grid-container {
    grid-template-columns: 100px 200px 1fr;
    grid-template-rows: 50% auto;
}
```

This example creates three columns where the first is 100 pixels wide, the second is 200 pixels wide, and the third
takes up the remaining space. The rows are set to be 50% of the container height and take up the remaining space.

## Grid Gap

The `grid-gap` property sets the gap between columns and rows in the grid. It is a shorthand for `grid-column-gap`
and `grid-row-gap`.

```css
.grid-container {
    grid-gap: 10px;
}
```

This example sets a 10-pixel gap between columns and rows.

## Grid Areas

The `grid-template-areas` property allows the creation of named grid areas. Grid items can then be placed into these
areas using the `grid-area` property.

```css
.grid-container {
    grid-template-areas:
        'header header header'
        'sidebar main main'
        'footer footer footer';
}

.grid-item {
    grid-area: header;
}
```

In this example, the grid is divided into three rows and three columns with named areas. The grid item with the
class `.grid-item` is placed in the 'header' area.

## Justify Content and Align Items

The `justify-content` and `align-items` properties control the placement of grid items along the grid's main axis and
cross axis, respectively.

```css
.grid-container {
    justify-content: center;
    align-items: center;
}
```

This example centers the grid items both horizontally and vertically.

## Grid Auto Flow

The `grid-auto-flow` property defines how the grid items are placed in the grid when there are more items than grid
cells.

```css
.grid-container {
    grid-auto-flow: row;
}
```

This example specifies that the grid items should be placed in rows.

## Responsive Grids

CSS Grid is excellent for creating responsive layouts. By using media queries, developers can change the grid structure
based on the screen size.

```css
@media (max-width: 600px) {
    .grid-container {
        grid-template-columns: 1fr;
    }
}
```

In this example, when the screen width is 600 pixels or less, the grid is set to a single column.

## Conclusion

CSS Grid is a versatile and powerful layout system that simplifies the creation of complex and responsive designs. By
mastering the properties and concepts discussed, developers can efficiently build grid-based layouts and enhance the
visual structure of web pages.