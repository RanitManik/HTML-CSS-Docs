# CSS Shadows and Outlines

### Box Shadow

The `box-shadow` property in CSS enables the creation of shadows around an element. It offers versatility in customizing
the shadow's appearance. The syntax is as follows:

```css
box-shadow: horizontal-offset vertical-offset blur spread color inset;
```

1. **Horizontal/Vertical Shadow:**
    - Specifies the shadow's position in the horizontal and vertical directions.

2. **Blur:**
    - Determines the amount of blur in the shadow.
    - A large value results in a darker, more pronounced blur.

3. **Spread:**
    - Sets the size of the shadow relative to the element.

4. **Color:**
    - Specifies the color of the shadow.

5. **Inset:**
    - An optional keyword for creating an inner shadow.

**Example:**

```css
box-shadow: 5px 2px 3px 4px red;
```

- Horizontal offset: 5px
- Vertical offset: 2px
- Blur: 3px
- Spread: 4px
- Color: Red

### Text Shadow

The `text-shadow` property adds a shadow effect to the text within an element. The syntax is as follows:

```css
text-shadow: horizontal-offset vertical-offset blur color;
```

**Example:**

```css
text-shadow: 2px 2px 3px #00ff00;
```

- Horizontal offset: 2px
- Vertical offset: 2px
- Blur: 3px
- Color: Green

### Outline

The `outline` property allows the addition of an outline around an element. It is distinct from the border, lying
outside the box model.

```css
outline: width style color;
```

1. **Width:**
    - Sets the width of the outline.

2. **Style:**
    - Specifies the style of the outline (e.g., dotted, solid).

3. **Color:**
    - Determines the color of the outline.

**Example:**

```css
outline: 2px dotted red;
```

### Outline Offset

The `outline-offset` property adjusts the distance or size of the outline from the element.

```css
outline-offset: Npx;
```

**Example:**

```css
outline-offset: 5px;
```

### Border Radius

The `border-radius` property adds rounded corners to an element's border. It affects all four corners simultaneously.

```css
border-radius: Npx;
```

**Example:**

```css
border-radius: 2px;
```

- All four corners have a radius of 2 pixels.

### Difference Between Outline and Border

- **Outline:**
    - Lies outside the box model.
    - Can be customized separately using `outline-offset`.

- **Border:**
    - Lies inside the box model.
    - Size/distance cannot be changed separately.

By understanding and utilizing these properties, you can enhance the aesthetics and design of your web elements
effectively. Experiment with different values and combinations to achieve the desired visual effects.