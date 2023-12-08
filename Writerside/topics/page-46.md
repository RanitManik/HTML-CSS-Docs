# CSS Animations

CSS animations enable developers to create dynamic and engaging user interfaces by smoothly transitioning between
different styles. In this guide, we'll explore the fundamentals of CSS animations, covering their syntax, key
properties, and common use cases.

## Introduction

CSS animations allow for the gradual change of property values over a set period, creating visually appealing effects.
Animations are often triggered by events like hover, click, or page load. They provide a way to enhance user experience
and add a sense of liveliness to web interfaces.

## Syntax

The basic syntax for a CSS animation involves defining a set of keyframes that describe the style changes at different
points during the animation.

```css
@keyframes animationName {
    0% {
        /* Styles at the start of the animation */
    }

    50% {
        /* Styles at the midpoint of the animation */
    }

    100% {
        /* Styles at the end of the animation */
    }
}

.element {
    animation: animationName duration timing-function delay iteration-count direction fill-mode;
}
```

- **animationName**: A name to identify the animation.
- **duration**: The total time the animation takes to complete (specified in seconds or milliseconds).
- **timing-function**: The acceleration curve of the animation (e.g., ease, ease-in, ease-out).
- **delay**: An optional delay before the animation starts.
- **iteration-count**: The number of times the animation should repeat (e.g., 1, 2, infinite).
- **direction**: The direction of the animation (normal, reverse, alternate, alternate-reverse).
- **fill-mode**: Specifies the styles applied to the element before and after the animation (forwards, backwards, both,
  none).

## Keyframes

Keyframes define the styles at various points during the animation. The percentage values represent the progression of
the animation.

```css
@keyframes fadeInOut {
    0% {
        opacity: 0;
    }

    50% {
        opacity: 1;
    }

    100% {
        opacity: 0;
    }
}
```

In this example, the element will fade in during the first half of the animation and then fade out during the second
half.

## Common Use Cases

### Continuous Rotation

```css
@keyframes rotate360 {
    to {
        transform: rotate(360deg);
    }
}

.rotating-element {
    animation: rotate360 2s linear infinite;
}
```

### Bouncing Animation

```css
@keyframes bounce {
    0%, 20%, 50%, 80%, 100% {
        transform: translateY(0);
    }

    40% {
        transform: translateY(-30px);
    }

    60% {
        transform: translateY(-15px);
    }
}

.bouncing-element {
    animation: bounce 2s infinite;
}
```

### Pulse Animation

```css
@keyframes pulse {
    0%, 100% {
        transform: scale(1);
    }

    50% {
        transform: scale(1.2);
    }
}

.pulsating-element {
    animation: pulse 1s infinite;
}
```

## Conclusion

CSS animations offer a powerful way to create visually appealing and interactive web designs. By understanding the
keyframe syntax and animation properties, developers can bring life to elements on a webpage and provide a more engaging
user experience.