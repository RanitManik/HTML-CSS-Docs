# CSS Selectors

## Introduction

Welcome to the CSS Selectors MasterClass, where we embark on a detailed exploration of CSS selectors. These selectors
are the architects of style, allowing you to precisely target and enhance HTML elements. Join us as we dissect each
selector, providing detailed examples and sub-properties to empower you in crafting visually stunning web pages.

## Types of Selectors

We can divide CSS selectors into five categories:

- Simple selectors (select elements based on name, id, class)
- Combinator selectors (select elements based on a specific relationship between them)
- Pseudo-class selectors (select elements based on a certain state)
- Pseudo-elements selectors (select and style a part of an element)
- Attribute selectors (select elements based on an attribute or attribute value)

## Simple Selectors

In this section, we will be discussing all types of simple selectors. In the next section, we will discuss the remaining
topics.

* ### Element Selector (Selection of Div)

The Element Selector is the fundamental selector, targeting HTML elements directly. Let's begin with the selection and
styling of `<div>` elements.

```css
div {
    border: 2px solid #008080;
    padding: 10px;
    margin: 10px;
}
```

* ### Class Selector

Class selectors enable you to style multiple elements sharing a common class attribute. They provide consistency and
flexibility in styling.

```css
.button {
    background-color: #4CAF50;
    color: white;
    padding: 10px 20px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    cursor: pointer;
}
```

* ### ID Selector

ID selectors uniquely style a specific HTML element. They are precise and useful when an individual element requires
distinct styling.

```css
#header {
    background-color: #333;
    color: white;
    padding: 10px;
    text-align: center;
}
```

* ### Child Selector

The Child Selector targets direct children of a specified parent element. It allows you to style specific levels of
hierarchy within your HTML structure.

```css
nav > ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}
```

* ### Descendant Selector

The Descendant Selector reaches deep into nested HTML structures, allowing you to style elements based on their
ancestry.

```css
article p {
    color: #555;
    font-size: 14px;
}
```

* ### Universal Selector

The Universal Selector is a wildcard, selecting all elements on the page. Use it with caution, as it applies styles
globally.

```css
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}
```

* ### Grouping Selector

The grouping selector selects all the HTML elements with the same style definitions.

Look at the following CSS code (the h1, h2, and p elements have the same style definitions):

```css
h1 {
text-align: center;
color: red;
}

h2 {
text-align: center;
color: red;
}

p {
text-align: center;
color: red;
}
```

It will be better to group the selectors, to minimize the code.
To group selectors, separate each selector with a comma.In this example we have grouped the selectors from the code
above:

```css
h1, h2, p {
text-align: center;
color: red;
}
```

## Pseudo Selector

Pseudo-selectors offer dynamic styling based on element states or positions. Explore the versatility of pseudo-classes
and pseudo-elements.

```css
a:hover {
    color: #FF4500;
    text-decoration: underline;
}
```

## Attribute Negation Selector

If you want to select elements that do not have a specific attribute, you can use the attribute negation selector:

```css
/* Selects all images without an "alt" attribute */
img:not([alt]) {
    border: 2px solid red;
}
```

## Conclusion

As we conclude this CSS Selectors MasterClass, you've delved into the intricacies of each selector, gaining a detailed
understanding of their properties and applications. Armed with this knowledge, you are equipped to wield CSS selectors
with precision, elevating your web design skills. Happy coding!