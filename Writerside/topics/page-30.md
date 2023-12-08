# CSS Variables

CSS Variables, also known as Custom Properties, introduce a way to define reusable values in CSS. They are entities
defined by CSS authors that contain specific values to be reused throughout a document.

## Declaration and Syntax:

- Declaring a variable:

  ```css
  :root {
    --main-color: #3498db;
  }
  ```

  Here, `--main-color` is the variable name, and `#3498db` is the value.

## Usage:

- Using a variable in a CSS rule:

  ```css
  body {
    background-color: var(--main-color);
  }
  ```

  This assigns the background color of the `body` element to the value of `--main-color`.

## Key Points:

1. **:root Selector:**
    - Variables are often declared in the `:root` selector to make them global and accessible throughout the document.

   ```css
   :root {
     --main-font: 'Arial', sans-serif;
   }
   ```

2. **Variable Names:**
    - Variable names are preceded by two hyphens (`--`).

   ```css
   :root {
     --main-background: #f0f0f0;
   }
   ```

3. **Variable Values:**
    - Variables can store various types of values, including colors, numbers, strings, and more.

   ```css
   :root {
     --border-width: 2px;
     --main-color: #27ae60;
     --font-family: 'Helvetica Neue', sans-serif;
   }
   ```

4. **Fallback Values:**
    - Fallback values can be specified for older browsers that do not support CSS Variables.

   ```css
   body {
     font-family: var(--font-family, 'Arial', sans-serif);
   }
   ```

   This uses `'Arial', sans-serif` as a fallback if `--font-family` is not supported.

## Benefits:

1. **Reusability:**
    - Variables allow the reuse of values throughout the stylesheet, promoting consistency and easy updates.

2. **Maintainability:**
    - Centralizing variable values in one place makes it easier to manage and update styles.

3. **Dynamic Changes:**
    - Variables can be modified dynamically using JavaScript, enabling changes in real-time.

## Example:

```css
:root {
  --main-color: #3498db;
  --background-color: #ecf0f1;
  --border-radius: 5px;
}

body {
  background-color: var(--background-color);
  color: var(--main-color);
}

.container {
  border: 1px solid var(--main-color);
  border-radius: var(--border-radius);
}
```

In this example, the `--main-color`, `--background-color`, and `--border-radius` variables are defined in the `:root`
selector and used throughout the stylesheet.

CSS Variables provide a powerful way to manage and reuse values in CSS, contributing to more maintainable and adaptable
stylesheets.