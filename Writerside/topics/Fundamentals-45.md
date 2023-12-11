# CSS Transitions

CSS transitions allow for the smooth and gradual change of property values over a specified duration. They enhance the
user experience by adding animations and visual effects to web pages. In this guide, we'll explore the key concepts of
CSS transitions, including their syntax, properties, and common use cases.

## Introduction

CSS transitions provide a way to animate changes in property values. They are triggered by changes in state, such as a
hover or click event, and can be applied to various properties, including color, size, position, and more. Transitions
make web interfaces more dynamic and engaging.

## Syntax

The basic syntax for a CSS transition involves specifying the property to transition, the duration of the transition,
and the timing function that determines the acceleration curve of the transition.

```css
/* Property to transition | Duration | Timing Function */
.element {
    transition: property duration timing-function;
}
```

For example, to create a smooth color transition on a button when hovered over:

```css
.button {
    transition: background-color 0.3s ease;
}

.button:hover {
    background-color: #3498db;
}
```

In this example, the background color will transition over 0.3 seconds with an easing timing function when the button is
hovered over.

## Transition Properties

### Property

The `property` value specifies the CSS property to transition. It can include multiple properties separated by commas.

```css
.element {
    transition: opacity 0.5s ease, transform 0.5s ease;
}
```

### Duration

The `duration` value determines how long the transition takes to complete. It is specified in seconds (s) or
milliseconds (ms).

```css
.element {
    transition: opacity 1s ease;
}
```

### Timing Function

The `timing-function` value defines the acceleration curve of the transition. Common values
include `ease`, `ease-in`, `ease-out`, and `ease-in-out`. Custom cubic bezier functions can also be used for more
control.

```css
.element {
    transition: opacity 0.5s cubic-bezier(0.4, 0, 0.2, 1);
}
```

### Delay

The `delay` value (optional) specifies a delay before the transition starts. It is also specified in seconds or
milliseconds.

```css
.element {
    transition: opacity 0.5s ease 0.2s;
}
```

## Common Use Cases

### Hover Effects

```css
.button {
    transition: background-color 0.3s ease;
}

.button:hover {
    background-color: #27ae60;
}
```

### Size Changes

```css
.box {
    transition: width 0.5s ease, height 0.5s ease;
}

.box:hover {
    width: 200px;
    height: 200px;
}
```

### Fading In/Out

```css
.fade {
    transition: opacity 0.5s ease;
}

.fade:hover {
    opacity: 0.5;
}
```

## Conclusion

CSS transitions provide a straightforward way to add animations to web pages. By carefully choosing transition
properties, durations, and timing functions, developers can create visually appealing and responsive user interfaces.