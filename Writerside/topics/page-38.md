# CSS Flexbox

Flexbox, or the Flexible Box Layout, is a layout model in CSS that allows the design of complex layouts and structures
with a more efficient and predictable way than traditional models. Flexbox is particularly well-suited for designing
dynamic and resizable layouts. Let's delve into the key concepts and properties of CSS Flexbox.

## Introduction

CSS Flexbox provides an efficient way to design layouts, align items, and distribute space within a container. It's
especially useful for creating responsive designs and managing the arrangement of items in a row or column.

## Flex Container and Flex Items

- **Flex Container:** The parent element becomes a flex container by setting its `display` property to `flex`
  or `inline-flex`. This establishes a flex formatting context for its children.

    ```css
    .flex-container {
        display: flex; /* or inline-flex */
    }
    ```

- **Flex Items:** The direct children of a flex container are referred to as flex items. They automatically become
  flexible boxes that can be horizontally or vertically aligned.

    ```css
    .flex-item {
        /* Styles for flex items */
    }
    ```

## Flex Direction

The `flex-direction` property defines the direction of the main axis and the cross axis in the flex container. The main
axis is the primary axis along which flex items are placed.

- **Row:** Items are placed along the horizontal axis (default).

    ```css
    .flex-container {
        flex-direction: row;
    }
    ```

- **Column:** Items are placed along the vertical axis.

    ```css
    .flex-container {
        flex-direction: column;
    }
    ```

## Justify Content

The `justify-content` property aligns flex items along the main axis of the flex container.

- **Flex Start:** Items are packed toward the start of the main axis.

    ```css
    .flex-container {
        justify-content: flex-start;
    }
    ```

- **Flex End:** Items are packed toward the end of the main axis.

    ```css
    .flex-container {
        justify-content: flex-end;
    }
    ```

- **Center:** Items are centered along the main axis.

    ```css
    .flex-container {
        justify-content: center;
    }
    ```

- **Space Between:** Items are evenly distributed with the first item at the start and the last item at the end.

    ```css
    .flex-container {
        justify-content: space-between;
    }
    ```

- **Space Around:** Items are evenly distributed with equal space around them.

    ```css
    .flex-container {
        justify-content: space-around;
    }
    ```

## Align Items

The `align-items` property aligns flex items along the cross axis of the flex container.

- **Flex Start:** Items are packed toward the start of the cross axis.

    ```css
    .flex-container {
        align-items: flex-start;
    }
    ```

- **Flex End:** Items are packed toward the end of the cross axis.

    ```css
    .flex-container {
        align-items: flex-end;
    }
    ```

- **Center:** Items are centered along the cross axis.

    ```css
    .flex-container {
        align-items: center;
    }
    ```

- **Baseline:** Items are aligned such that their baselines align.

    ```css
    .flex-container {
        align-items: baseline;
    }
    ```

- **Stretch:** Items are stretched to fill the container.

    ```css
    .flex-container {
        align-items: stretch;
    }
    ```

## Flex Wrap

The `flex-wrap` property controls whether flex items are forced onto a single line or can wrap onto multiple lines.

- **No Wrap:** All flex items are on one line (default).

    ```css
    .flex-container {
        flex-wrap: nowrap;
    }
    ```

- **Wrap:** Flex items can wrap onto multiple lines if needed.

    ```css
    .flex-container {
        flex-wrap: wrap;
    }
    ```

- **Wrap Reverse:** Flex items wrap onto multiple lines in reverse order.

    ```css
    .flex-container {
        flex-wrap: wrap-reverse;
    }
    ```

## Align Content

The `align-content` property aligns a flex container's lines within the flex container when there's extra space on the
cross axis.

- **Flex Start:** Lines are packed toward the start of the cross axis.

    ```css
    .flex-container {
        align-content: flex-start;
    }
    ```

- **Flex End:** Lines are packed toward the end of the cross axis.

    ```css
    .flex-container {
        align-content: flex-end;
    }
    ```

- **Center:** Lines are centered along the cross axis.

    ```css
    .flex-container {
        align-content: center;
    }
    ```

- **Space Between:** Lines are evenly distributed with the first line at the start and the last line at the end.

    ```css
        .flex-container {
            align-content: space-between;
        }
    ```

- **Space Around:** Lines are evenly distributed with equal space around them.

    ```css
    .flex-container {
        align-content: space-around;
    }
    ```

- **Stretch:** Lines are stretched to fill the container.

    ```css
    .flex-container {
        align-content: stretch;
    }
  ```

## Conclusion

CSS Flexbox is a powerful layout model that simplifies the creation of flexible and responsive designs. By understanding
and applying the properties discussed, developers can efficiently structure web layouts and improve user experiences.