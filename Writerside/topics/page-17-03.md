# Attribute Selectors in CSS

Attribute selectors in CSS provide a versatile and powerful way to target HTML elements based on the presence or value
of their attributes. This allows for more granular and dynamic styling, enhancing the flexibility of your stylesheets.

## Basic Attribute Selector

The basic attribute selector allows you to select elements with a specific attribute, regardless of its value. Here's an
example:

```css
/* Selects all elements with a "data-theme" attribute */
[data-theme] {
    color: blue;
}
```

In this case, any element that includes the `data-theme` attribute, regardless of its value, will have a blue text
color.

## Attribute with a Specific Value

You can also target elements with a specific attribute value using the attribute selector. For instance:

```css
/* Selects elements with a "type" attribute set to "submit" */
input[type="submit"] {
    background-color: green;
}
```

This rule styles all `input` elements with a `type` attribute set to "submit" and gives them a green background color.

## Attribute Presence Selector

If you simply want to select elements with a specific attribute, regardless of its value, you can use the attribute
presence selector. Example:

```css
/* Selects all elements with a "target" attribute */
[target] {
    border: 1px solid red;
}
```

This rule applies a red border to any element that has a `target` attribute.

## Substring Matching Attribute Selector

CSS also provides substring matching attribute selectors for more advanced selection. For example:

```css
/* Selects links with an "href" attribute containing "example.com" */
a[href*="example.com"] {
    color: purple;
}
```

This styles all anchor (`a`) elements whose `href` attribute contains the substring "example.com" with a purple text
color.

## Attribute Starts With Selector

You can target elements whose attribute value starts with a specific string. Here's an illustration:

```css
/* Selects images with a "src" attribute starting with "icon-" */
img[src^="icon-"] {
    width: 20px;
    height: 20px;
}
```

This rule sets a width and height for all `img` elements whose `src` attribute starts with "icon-".

## Attribute Ends With Selector

Similarly, the attribute ends with selector allows you to style elements with an attribute ending in a specific string:

```css
/* Selects elements with a "class" attribute ending with "-highlight" */
[class$="-highlight"] {
    background-color: yellow;
}
```

This example applies a yellow background color to elements whose `class` attribute ends with "-highlight".

## Attribute Value Prefix Selector

You can target elements with an attribute value that starts with a specified prefix:

```css
/* Selects elements with a "data-" attribute */
[data|="value"] {
    font-weight: bold;
}
```

This rule makes text bold for elements with an attribute that starts with "data-".

## Attribute Negation Selector

If you want to select elements that do not have a specific attribute, you can use the attribute negation selector:

```css
/* Selects all images without an "alt" attribute */
img:not([alt]) {
    border: 2px solid red;
}
```

This styles images without an `alt` attribute with a red border.

## Conclusion

Attribute selectors in CSS empower developers to precisely target and style elements based on their attributes. Whether
you're selecting by presence, value, substring, prefix, or negation, these selectors provide a robust toolset for
creating dynamic and responsive stylesheets. Understanding and leveraging attribute selectors enhances your ability to
craft sophisticated and tailored designs in web development.