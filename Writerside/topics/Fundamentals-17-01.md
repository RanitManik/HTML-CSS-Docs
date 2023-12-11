# Combinator Selectors

Combinator selectors in CSS allow you to target elements based on their relationship with other elements. Understanding
these selectors is crucial for creating precise and efficient stylesheets. Let's explore the various combinator
selectors and how they can be used.

## Descendant Selector

The descendant selector (whitespace) selects all elements that are descendants of a specified element, regardless of how
deep the hierarchy goes.

```css
/* Selects all <p> elements inside a <div> */
div p {
    color: blue;
}
```

In this example, all `<p>` elements that are descendants of a `<div>` will have a blue text color.

## Child Selector

The child selector (`>`) selects all direct children of a specified element.

```css
/* Selects all <li> elements that are direct children of <ul> */
ul > li {
    list-style-type: square;
}
```

Here, only `<li>` elements that are direct children of `<ul>` will have a square list style.

## Adjacent Sibling Selector

The adjacent sibling selector (`+`) selects an element that is immediately preceded by a specified element.

```css
/* Selects all <p> elements that are immediately preceded by an <h2> */
h2 + p {
    font-style: italic;
}
```

This rule applies italic style to all `<p>` elements that are immediately preceded by an `<h2>`.

## General Sibling Selector

The general sibling selector (`~`) selects all elements that are siblings of a specified element and share the same
parent.

```css
/* Selects all <span> elements that are siblings of <h2> */
h2 ~ span {
    color: red;
}
```

This example styles all `<span>` elements that are siblings of an `<h2>` with a red text color.

## Conclusion

Combinator selectors in CSS provide a powerful way to navigate the document structure and target specific elements based
on their relationships. Whether you're styling descendants, direct children, adjacent siblings, or general siblings,
these selectors offer flexibility and precision in your styling approach. By mastering combinator selectors, you can
create well-organized and visually appealing web designs.