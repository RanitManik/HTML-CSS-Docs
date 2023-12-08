# CSS Overflow Property

The `overflow` property in CSS is used to control how content that is too large to fit inside a container should be
handled. It helps in managing overflow when the content exceeds the dimensions of the containing element.

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
    - Use `overflow: ellipsis;` to truncate text content with an ellipsis (...) when it overflows.

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

The `overflow` property provides flexibility in handling different scenarios where content may exceed the dimensions of
its container. Understanding and appropriately using this property is crucial for creating well-designed and
user-friendly interfaces.