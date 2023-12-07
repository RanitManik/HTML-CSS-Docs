# CSS Fonts, Text & Color Properties

## Introduction

Welcome to the world of text styling in CSS! In this guide, we'll delve into the various properties that allow you to
manipulate and enhance the visual aspects of text on your web pages. From fonts to colors, join us on a journey to
master the art of crafting beautifully styled text content.

## Fonts

The choice of fonts plays a crucial role in defining the visual identity of your website. CSS provides a variety of
options for specifying fonts, from generic families to custom font imports.

## CSS Font Properties

### 1. **font-family:**

- Specifies the font for text.
- Example:
  ```css
  body {
      font-family: 'Arial', sans-serif;
  }
  ```

### 2. **font-size:**

- Sets the size of the font.
- Example:
  ```css
  h1 {
      font-size: 24px;
  }
  ```

### 3. **font-weight:**

- Defines the thickness of the font characters.
- Example:
  ```css
  p {
      font-weight: bold;
  }
  ```

### 4. **font-style:**

- Sets the style of the font (normal, italic, or oblique).
- Example:
  ```css
  em {
      font-style: italic;
  }
  ```

### 5. **font-variant:**

- Controls the usage of alternate glyphs.
- Example:
  ```css
  p {
      font-variant: small-caps;
  }
  ```

### 6. **line-height:**

- Specifies the height of a line of text.
- Example:
  ```css
  body {
      line-height: 1.5;
  }
  ```

### 7. **letter-spacing:**

- Adjusts the space between characters.
- Example:
  ```css
  h2 {
      letter-spacing: 2px;
  }
  ```

### 8. **text-transform:**

- Controls the capitalization of text.
- Example:
  ```css
  p {
      text-transform: uppercase;
  }
  ```

### 9. **color:**

- Sets the color of the text.
- Example:
  ```css
  a {
      color: #3498db;
  }
  ```

### 10. **text-shadow:**

- Adds a shadow to the text.
- Example:
  ```css
  h1 {
      text-shadow: 2px 3px 4px red;
  }
  ```

## Colors

Bring your text to life with color! Define text color, background color, and explore various color formats to achieve
the desired visual impact.

## CSS Colors properties

### 1. **Named Colors:**

- CSS provides a set of predefined color names.
- Example:
  ```css
  h1 {
      color: red;
  }
  ```

### 2. **Hexadecimal Notation:**

- Represents colors using a six-digit code.
- Example:
  ```css
  p {
      background-color: #00ff00;
  }
  ```

### 3. **RGB Notation:**

- Represents colors using red, green, and blue values.
- Example:
  ```css
  a {
      color: rgb(255, 0, 0);
  }
  ```

### 4. **RGBA Notation:**

- Similar to RGB but includes an alpha channel for transparency.
- Example:
  ```css
  div {
      background-color: rgba(0, 0, 255, 0.5);
  }
  ```

### 5. **HSL Notation:**

- Represents colors using hue, saturation, and lightness.
- Example:
  ```css
  span {
      color: hsl(120, 100%, 50%);
  }
  ```

### 6. **HSLA Notation:**

- Similar to HSL but includes an alpha channel for transparency.
- Example:
  ```css
  h2 {
      background-color: hsla(240, 100%, 50%, 0.7);
  }
  ```

### 7. **Keyword Values:**

- In addition to named colors, CSS supports certain keyword values.
- Example:
  ```css
  body {
      background-color: white;
  }
  ```

### 8. **System Colors:**

- Uses system-specific color values.
- Example:
  ```css
  button {
      border-color: ButtonShadow;
  }
  ```

## More properties

Certainly! Here's the detailed explanation for each property along with the corresponding code examples:

1. **Specify Font Family**
    - *Explanation:* Sets the preferred font for the entire document, prioritizing 'a' and 'b', and falling back to a
      generic sans-serif font.
    - *Code:*
      ```css
      body {
          font-family: 'a', 'b', sans-serif;
      }
      ```

2. **Make Font Italic (Oblique)**
    - *Explanation:* Applies italic style to emphasize or differentiate specific text.
    - *Code:*
      ```css
      em {
          font-style: italic;
      }
      ```

3. **Make Text Bolder**
    - *Explanation:* Increases the thickness of the text to create a bold visual effect.
    - *Code:*
      ```css
      strong {
          font-weight: 700; /* Values from 100 to 900 */
      }
      ```

4. **Set Font Size**
    - *Explanation:* Defines the font size for h1 elements to be 24 pixels.
    - *Code:*
      ```css
      h1 {
          font-size: 24px;
      }
      ```

5. **Set Line Height**
    - *Explanation:* Adjusts the space between lines in paragraphs to 1.5 times the font size.
    - *Code:*
      ```css
      p {
          line-height: 1.5;
      }
      ```

6. **Set Letter Spacing**
    - *Explanation:* Increases the space between characters in h2 for better readability.
    - *Code:*
      ```css
      h2 {
          letter-spacing: 2px;
      }
      ```

7. **Text Transformation**
    - *i. Capitalize:* Capitalizes the first letter of each word in paragraphs.
    - *ii. Lowercase:* Transforms text to lowercase in paragraphs.
    - *iii. Uppercase:* Transforms text to uppercase in paragraphs.
    - *Code:*
      ```css
      /* i. Capitalize */
      p.capitalize {
          text-transform: capitalize;
      }
 
      /* ii. Lowercase */
      p.lowercase {
          text-transform: lowercase;
      }
 
      /* iii. Uppercase */
      p.uppercase {
          text-transform: uppercase;
      }
      ```

8. **Text Decoration**
    - *i. Dotted Underline with Red Color:* Adds a dotted red underline to anchor elements.
    - *Code:*
      ```css
      /* i. Dotted Underline with Red Color */
      a {
          text-decoration-style: dotted;
          text-decoration-color: red;
          text-decoration-thickness: 2px;
          text-decoration-line: underline;
      }
      ```

9. **Text Indent**
    - *Explanation:* Indents the first line of blockquote elements by 20 pixels.
    - *Code:*
      ```css
      blockquote {
          text-indent: 20px;
      }
      ```

10. **Text Overflow**
    - *Explanation:* Uses an ellipsis (...) to indicate text overflow in a hidden div.
    - *Code:*
      ```css
      div.overflow {
          text-overflow: ellipsis;
          overflow: hidden;
      }
      ```

11. **Word Break**
    - *Explanation:* Allows breaking words at any character to prevent overflow in a specific div.
    - *Code:*
      ```css
      div.break {
          word-break: break-all;
      }
      ```

12. **Text Align Center**
    - *Explanation:* Aligns text in h3 elements to the center.
    - *Code:*
      ```css
      h3 {
          text-align: center;
      }
      ```

13. **Color Properties**
    - *i. Color Keyword:* Sets the color of a span with the class 'keyword' to green.
    - *ii. Hex Color:* Sets the color of a span with the class 'hex' to a specific hex code.
    - *iii. RGB Color:* Sets the color of a span with the class 'rgb' using RGB values.
    - *iv. RGBA Color:* Sets the color of a span with the class 'rgba' using RGBA values with alpha (opacity).
    - *v. HSL Color:* Sets the color of a span with the class 'hsl' using HSL values.
    - *Code:*
      ```css
      /* i. Color Keyword */
      span.keyword {
          color: green;
      }

      /* ii. Hex Color */
      span.hex {
          color: #ff4500;
      }

      /* iii. RGB Color */
      span.rgb {
          color: rgb(0, 0, 255);
      }

      /* iv. RGBA Color */
      span.rgba {
          color: rgba(255, 0, 0, 0.5);
      }

      /* v. HSL Color */
      span.hsl {
          color: hsl(120, 100%, 50%);
      }
      ```

14. **Background Color**
    - *Explanation:* Sets the background color of a specific div to green.
    - *Code:*
      ```css
      div.background {
          background-color: green;
      }
      ```

15. **Specific Font Families**
    - *Explanation:* Applies specific font families to the entire document.
    - *Code:*
      ```css
      body {
          font-family: 'Baloo Bhai 2', 'Poppins', sans-serif;
      }
      ```

These methods provide flexibility in specifying colors for text, backgrounds, borders, and other elements in your CSS
styles. Choose the method that suits your needs and design preferences.

## Conclusion

As we conclude this exploration of text styling in CSS, you've gained insights into a variety of properties that can
transform your text into a visually appealing and well-designed element on your web pages. The art of text styling is a
powerful tool in the web developer's toolkit, allowing you to create engaging and aesthetically pleasing content. Keep
experimenting and refining your text styling skills to make your web pages truly stand out. Happy styling!