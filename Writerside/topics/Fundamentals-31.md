# CSS Media Queries

CSS Media Queries enable the styling of web pages to adapt based on various device characteristics, such as screen size,
resolution, or device type. By using media queries, you can create responsive designs that cater to different devices
and screen dimensions. Here's an overview of how media queries work and how to implement them:

## Basic Syntax

A media query begins with the `@media` rule, followed by a media type and, if needed, one or more expressions to check
for specific conditions.

```css
/* Example of a media query for screens smaller than 600 pixels */
@media screen and (max-width: 600px) {
  /* CSS rules for screens smaller than 600 pixels go here */
}
```

## Media Types

- **all:** Used for all devices.
- **print:** Used for printers.
- **screen:** Used for computer screens, tablets, smartphones, etc.
- **speech:** Used for screen readers that "reads" the page out loud.

## Media Features

Media features check characteristics of the user's device. Common features include:

- **width:** Width of the viewport.
- **height:** Height of the viewport.
- **device-width:** Width of the device screen.
- **device-height:** Height of the device screen.
- **orientation:** Checks whether the device is in landscape or portrait mode.
- **aspect-ratio:** Aspect ratio of the viewport.
- **color:** Number of bits per color component for the output device.
- **resolution:** Resolution of the output device.

## Example

```css
/* Responsive styles for screens smaller than 768 pixels */
@media screen and (max-width: 768px) {
  body {
    font-size: 14px;
  }

  .container {
    width: 100%;
  }
}
```

## Combining Multiple Conditions

You can use logical operators such as `and`, `or`, and `not` to combine multiple conditions within a media query.

```css
/* Example of a media query combining conditions */
@media screen and (min-width: 600px) and (orientation: landscape) {
  /* CSS rules for screens wider than 600 pixels in landscape mode go here */
}
```

## Using Media Queries in HTML

Media queries can also be specified directly in the HTML file using the `<link>` tag.

```html

<link rel="stylesheet" media="screen and (max-width: 600px)" href="styles.css">
```

## Conclusion

CSS Media Queries play a crucial role in creating responsive web designs. They allow developers to optimize layouts and
styles based on the characteristics of the user's device, providing a better user experience across various screens and
devices.