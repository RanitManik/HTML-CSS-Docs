# text-wrap: balance

`text-wrap: balance` is a relatively new CSS property that can be used to distribute text evenly across multiple lines,
aiming for a more balanced and visually appealing layout. Here's what you need to know about it:

## What it does

* It analyzes the text within an element and tries to break it into lines so that each line has roughly the same number
  of characters.
* This can improve the readability and aesthetics of text, especially for headings, titles, and short paragraphs.

## Example: Balancing a heading

```html
<h1 style="max-width: 500px; text-wrap: balance;">This Is a Long Heading That Needs Balancing</h1>
```

This code applies `text-wrap: balance` to a heading with a maximum width of 500px. The browser will try to distribute
the text across multiple lines, aiming for roughly equal character counts on each line.

## Things to consider

* **Limited browser support:** Currently, only Chrome and Firefox support `text-wrap: balance` natively. For other
  browsers, you may need polyfills or alternative solutions.
* **Potential word breaking:** To achieve even lines, the property may break words in unexpected places. It's important
  to consider the context and adjust if needed.
* **Layout constraints:** Balancing lines might not always be possible, especially with short text or limited container
  width.

> Overall, `text-wrap: balance` is a promising new property for enhancing text layout. It's worth experimenting with to
> see if it can improve the visual appeal and readability of your content.**

Here are some additional resources you may find helpful:

* **MDN Web Docs:
  ** [https://developer.mozilla.org/en-US/docs/Web/CSS/text-wrap](https://developer.mozilla.org/en-US/docs/Web/CSS/text-wrap)
* **Can I Use:** [https://caniuse.com/css-text-wrap-balance](https://caniuse.com/css-text-wrap-balance)
* **Chrome Developers Blog:
  ** [https://developer.chrome.com/blog/css-text-wrap-balance](https://developer.chrome.com/blog/css-text-wrap-balance)


