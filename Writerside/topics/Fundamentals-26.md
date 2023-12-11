# CSS Overflow Property

The `overflow` property in CSS is fundamental for controlling how content that is too large to fit inside a container
should be handled, particularly when the content exceeds the dimensions of the containing element.

## Values of `overflow` Property

1. **visible (default):**
    - Content overflows the box, and it may be rendered outside the box.

   ```css
   overflow: visible;
   ```

2. **hidden:**
    - Content that overflows is clipped and not visible.

   ```css
   overflow: hidden;
   ```

3. **scroll:**
    - Adds a scrollbar to see the rest of the content if it overflows.

   ```css
   overflow: scroll;
   ```

4. **auto:**
    - Similar to scroll, but a scrollbar is only added if the content overflows.

   ```css
   overflow: auto;
   ```

## Overflow in X and Y Directions

- **overflow-x:**
    - Specifies the behavior for horizontal overflow.

  ```css
  overflow-x: visible | hidden | scroll | auto;
  ```

- **overflow-y:**
    - Specifies the behavior for vertical overflow.

  ```css
  overflow-y: visible | hidden | scroll | auto;
  ```

## White-Space Property

The `white-space` property defines how white spaces inside an element are handled.

   ```css
   white-space: normal | nowrap | pre | pre-wrap | pre-line;
   ```

- `normal`: Sequences of white spaces are collapsed, and text wraps as necessary.
- `nowrap`: Sequences of white spaces are collapsed, and text does not wrap, overflowing the container.
- `pre`: Sequences of white spaces are preserved, and text does not wrap, overflowing the container.
- `pre-wrap`: Sequences of white spaces are preserved, and text wraps as necessary.
- `pre-line`: Sequences of white spaces are collapsed, and text wraps as necessary. Newline characters are preserved.

**Example:**

   ```css
   .text-container {
     white-space: nowrap;
     overflow: hidden;
     text-overflow: ellipsis;
   }
   ```

This example ensures that text inside the `.text-container` does not wrap, and if it overflows, it will be truncated
with an ellipsis (...).

## Text-Overflow Property

The `text-overflow` property specifies how overflowed content that is not displayed should be signaled to the user.

   ```css
   text-overflow: clip | ellipsis | string;
   ```

* `clip`: Content is simply clipped, and the overflow is not displayed.
* `ellipsis`: If the content overflows, it is truncated with an ellipsis (...) to indicate hidden content.
* `string`: A custom string is used to indicate overflow.

**Example:**

   ```css
   .text-container {
     white-space: nowrap;
     overflow: hidden;
     text-overflow: ellipsis;
   }
   ```

Here, the `text-overflow: ellipsis;` property is used to indicate overflow with an ellipsis.

## Example Usage

```css
.container {
  width: 200px;
  height: 200px;
  overflow: hidden;
}
```

In this example, the `.container` element has a fixed width and height. If the content inside this container exceeds
these dimensions, it will be hidden.

## Use Cases

1. **Overflow in Text Containers:**
    - Use `white-space` and `text-overflow` to control the display of text overflow.

   ```css
   .text-container {
     white-space: nowrap;
     overflow: hidden;
     text-overflow: ellipsis;
   }
   ```

2. **Scrollable Containers:**
    - Create scrollable containers for large amounts of content.

   ```css
   .scrollable-container {
     width: 300px;
     height: 200px;
     overflow: auto;
   }
   ```

3. **Hide Overflowing Content:**
    - Hide content that exceeds the container.

   ```css
   .hidden-overflow {
     width: 150px;
     height: 100px;
     overflow: hidden;
   }
   ```

The `overflow` property, along with related properties like `white-space` and `text-overflow`, provides flexibility in
handling different scenarios where content may exceed the dimensions of its container. Understanding and appropriately
using these properties are crucial for creating well-designed and user-friendly interfaces.