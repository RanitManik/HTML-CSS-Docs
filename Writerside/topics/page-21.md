# CSS Specificity & Cascade

CSS Specificity plays a pivotal role in determining the styles applied to HTML elements, especially in scenarios with
overlapping CSS rules. It assigns a value or weight to a CSS selector, and the higher the specificity, the greater the
precedence of the selector.

## The Cascade Algorithm:

CSS, which stands for Cascading Style Sheets, employs a cascade algorithm to resolve conflicts when multiple CSS rules
target an HTML element. This algorithm comprises four key stages:

1. **Position and Order of Appearance:** The order in which CSS rules appear influences their application. Styles
   declared later take precedence, overriding previous declarations. For example:

    ```css
    /* Position and order of appearance */
    h1 {
        color: green;
    }

    .header-title {
        color: orange !important;
    }
    ```

2. **Specificity:** The specificity of a selector determines its strength in the cascade. Higher specificity means a
   stronger match. Specificity is calculated based on a point system involving inline styles, IDs, classes, and tag
   names. For instance:

    ```css
    /* Example of CSS specificity */
    .nav-link {
        color: blue; /* Lower specificity */
    }

    #home-link {
        color: red; /* Higher specificity */
    }
    ```

3. **Origin:** The origin of CSS, whether authored by the user, a browser extension, or the browser itself, impacts the
   cascade. Authored CSS takes precedence over other origins.

4. **Importance:** The `!important` rule type grants a CSS rule the highest priority, making it override other rules.
   However, it's advisable to use `!important` sparingly due to potential complexities in maintaining and debugging
   stylesheets.

## Effect of Position: Last One Wins

If two rules have selectors with identical specificity, the last one declared takes precedence. The position can be
influenced by the inclusion of styles through `<link>` tags, `<style>` tags, or inline style attributes.

## Specificity Strength

Specificity is determined by the selector's components, with the following hierarchy:

- Inline Styles (Highest Specificity)
- ID Selectors
- Class or Attribute Selectors
- Element Selectors
- Universal Selectors (Lowest Specificity)

### Inline Styles: The Highest Specificity

Inline styles have the highest specificity and always override other styles. For instance:

```html
<h1 id="title" class="h1" style="color:purple">CodeWithHarry</h1>
```

In this example, the color `purple` will be applied to the `h1` tag.

### ID Selector: High Specificity

ID selectors also possess high specificity, as illustrated in this example:

```css
/* ID Selector example */
#title {
    color: red;
}
```

Here, the color `red` will be applied to the `h1` tag with the `id` of `title`.

### Class and Attribute Selectors: Moderate Specificity

Class and attribute selectors have moderate specificity. Consider this example:

```css
/* Class Selector example */
.h1 {
    color: blue;
}
```

In this case, the color `blue` will be applied to the `h1` tag with the class `h1`.

### Element Selector: Low Specificity

Element selectors, such as `<h1>`, have low specificity. Example:

```css
/* Element Selector example */
h1 {
    color: pink;
}
```

Here, the color `pink` will be applied to all `h1` tags.

### Universal Selector: Lowest Specificity

The universal selector `*` and combining selectors have the lowest specificity. Example:

```css
/* Universal Selector example */
* {
    color: gray;
}
```

In this instance, the color `gray` will be applied to all elements.

## Importance: The !important Rule

The `!important` rule gives a style the highest level of importance, making it override other rules. However,
using `!important` excessively can complicate stylesheet maintenance. Example:

```css
/* Using !important for highest priority */
.important-text {
    color: purple !important;
}
```

In this case, the color `purple` will take precedence.

## Specificity Calculation in CSS

When dealing with conflicting CSS rules, understanding specificity is crucial. Specificity is a value or weight assigned
to a CSS selector, determining which styles take precedence. Here's how you calculate it:

1. **Universal Selector:** 0
2. **Element Selectors and Pseudo-elements:** 1
3. **Class Selectors, Attribute Selectors, and Pseudo-classes:** 10
4. **ID Selectors:** 100
5. **Inline Styles:** 1000

Now, let's break down an example:

```html
<h1 id="title" class="h1">CodeWithHarry</h1>
```

Here, the specificity is calculated as follows:

- ID Selector (`#title`): 100
- Class Selector (`.h

1`): 10

- Element Selector (`h1`): 1

Total Specificity: 111

In case of a tie in specificity, the rule appearing last in the CSS takes precedence.

### Quick Quiz Solution:

Consider the selector:

```css
a.harryclass.rohan-class[href]:hover {
  color: red;
}
```

**Specificity Calculation:**

- Element Selector (`a`): 1
- Class Selectors (`.harryclass` and `.rohan-class`): 20
- Attribute Selector (`[href]`): 10
- Pseudo-class (`:hover`): 10

Total Specificity: 41

So, the specificity value for the selector is 41.

## Conclusion

Understanding CSS specificity, the cascade algorithm, and the impact of position, origin, and importance is crucial for
crafting robust styles. This knowledge empowers developers to create predictable and maintainable stylesheets,
harmonizing structure and aesthetics in web development.