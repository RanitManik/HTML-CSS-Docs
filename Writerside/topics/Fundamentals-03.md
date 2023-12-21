# HTML Fundamentals: Building the Web

HTML, or HyperText Markup Language, forms the backbone of the World Wide Web. It serves as the standard markup language
for creating web pages, employing key components such as elements and attributes.

## Elements: The Foundation of HTML

At its essence, HTML relies on elements as the fundamental building blocks of a web page. Each HTML element comprises a
start tag, content, and an end tag. The start tag initiates the element, the end tag concludes it, and the content lies
between them.

To illustrate, crafting a paragraph involves the `<p>` element:

```html
<p>This is a paragraph.</p>
```

In this example, `<p>` marks the start, `</p>` denotes the end, and "This is a paragraph." constitutes the content.

Certain elements, like line breaks, dispense with an end tag:

```html
<br>
```

## HTML Tags: Structuring Content

HTML utilizes tags, enclosed in angle brackets ("<" and ">"), in pairs with opening and closing counterparts. Here are
examples of HTML tags:

1. **Paragraph Tag:**
   ```html
   <p>This is a paragraph.</p>
   ```

2. **Heading Tags:**
   ```html
   <h1>This is a heading level 1</h1>
   <h2>This is a heading level 2</h2>
   <!-- ... up to h6 -->
   ```

3. **Anchor Tag (Link):**
   ```html
   <a href="https://www.example.com">Visit Example.com</a>
   ```

4. **Image Tag:**
   ```html
   <img src="image.jpg" alt="Description of the image">
   ```

5. **List Tags:**
   ```html
   <ul>
       <li>Item 1</li>
       <li>Item 2</li>
   </ul>

   <ol>
       <li>Item 1</li>
       <li>Item 2</li>
   </ol>
   ```

6. **Div Tag (Division/Container):**
   ```html
   <div>This is a container</div>
   ```

7. **Form Tags:**
   ```html
   <form action="/submit" method="post">
       <!-- Form elements go here -->
   </form>
   ```

8. **Input Tag:**
   ```html
   <input type="text" name="username" placeholder="Enter your username">
   ```

9. **Button Tag:**
   ```html
   <button type="submit">Submit</button>
   ```

10. **Table Tags:**
    ```html
    <table>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
    </table>
    ```

These examples showcase the versatility of HTML tags for diverse purposes.

## Attributes: Enhancing Elements

Attributes furnish additional information about HTML elements, residing in the opening tag. Comprising a name and a
value, attributes modify an element's behavior or appearance.

Consider the image element (`<img>`):

```html
<img src="image.jpg" alt="An example image">
```

Here, `src` is an attribute with the value "image.jpg," and `alt` provides alternative text for the image.

### Common HTML Elements

1. **Headings (`<h1>` to `<h6>`):**
   ```html
   <h1>This is a Heading 1</h1>
   ```

2. **Paragraph (`<p>`):**
   ```html
   <p>This is a paragraph.</p>
   ```

3. **Links (`<a>`):**
   ```html
   <a href="https://www.example.com">Visit Example.com</a>
   ```

4. **Lists (`<ul>`, `<ol>`, `<li>`):**
   ```html
   <ul>
     <li>Item 1</li>
     <li>Item 2</li>
   </ul>
   ```

5. **Images (`<img>`):**
   ```html
   <img src="image.jpg" alt="An example image">
   ```

## Nesting Elements

HTML elements can nest within each other, forming a hierarchical structure:

```html

<div>
    <h2>Heading inside a Div</h2>
    <p>Paragraph inside the Div.</p>
</div>
```

Here, `<h2>` and `<p>` nest within `<div>` (division).

## HTML Document Structure

A standard HTML document comprises a doctype declaration (`<!DOCTYPE html>`), opening and closing HTML tags (`<html>`),
head and body sections, and metadata.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Page Title</title>
</head>
<body>

<h1>This is a Heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

## Conclusion

Mastery of HTML, encompassing elements and attributes, is crucial for aspiring web developers. These foundational
components provide the structure and content for dynamic web pages. As you delve deeper into web development,
encountering a plethora of elements and attributes, you embark on a journey towards creating immersive online
experiences. Proficiency in HTML is the cornerstone for mastering other web technologies.