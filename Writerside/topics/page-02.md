# Your First HTML Website

## Configuring GIT

Version control is a crucial aspect of web development, and GIT is a widely-used system for managing project versions.
Let's configure GIT for your project:

1. Install GIT by visiting the [official GIT website](https://git-scm.com/) and following the installation instructions
   for your operating system.

2. Open VS Code and set up GIT integration:
    - Press `Ctrl + Shift + P` to open the command palette.
    - Type "Git: Initialize Repository" and select your project folder.

3. Create a `.gitignore` file in your project folder to specify files and directories you want GIT to ignore. For a
   basic web project, you can include:

   ```
   node_modules/
   .vscode/
   ```

   Customize this based on your project's needs.

4. Stage your changes and commit them using the Source Control view in VS Code.

## Configuring VS Code for Our First Website

Now, let's fine-tune VS Code settings for an optimal web development experience:

1. **Workspace Settings:**
    - Click on the gear icon in the lower-left corner and select "Settings."
    - Configure settings such as font size, theme, and tab size according to your preferences.

2. **Extensions:**
    - Explore and install additional VS Code extensions to enhance your workflow.
    - Some recommended extensions include:
        - "Auto Close Tag" for automatically closing HTML tags.
        - "Prettier" for code formatting.
        - "Live Server" for easy and quick previews of your web pages.

   Install these extensions through the Extensions view (`Ctrl+Shift+X`).

## Useful VS Code Extensions

Let's delve deeper into some extensions that can significantly boost your productivity:

1. **Auto Rename Tag:**
    - Automatically renames paired HTML tags, saving you time and reducing errors.

2. **ESLint and Stylelint:**
    - Linting tools for JavaScript and CSS, respectively, to ensure code quality.

3. **GitLens:**
    - Supercharge your GIT capabilities within VS Code, providing enhanced insights into your code's history and
      contributors.

## Linking CSS and JavaScript

As your website grows in complexity, you'll want to separate your concerns by using separate files for HTML, CSS, and
JavaScript. To link CSS and JavaScript to your HTML file:

1. **Linking CSS:**
    - Create a new file named `styles.css` in your project folder.
    - In your `index.html`, add the following line within the `<head>` tag:

      ```html
      <link rel="stylesheet" href="styles.css">
      ```

2. **Linking JavaScript:**
    - Create a new file named `script.js` in your project folder.
    - At the end of your `index.html` file, just before the closing `</body>` tag, add:

      ```html
      <script src="script.js"></script>
      ```

## Client-Server Interaction Explained

Understanding client-server interaction is fundamental in web development. Let's briefly explore this concept:

- **Client:** The user's device, like an iPhone 15 Pro Max, running a web browser.
- **Server:** A remote computer hosting your website.

When a user interacts with your website:

1. **Request:** The client sends a request (e.g., clicking a link).
2. **Server Processing:** The server processes the request and sends back the necessary resources (HTML, CSS,
   JavaScript).
3. **Rendering:** The client renders the received resources, and the user sees the updated page.

This interaction is the backbone of dynamic and interactive web applications.

Congratulations! You've now configured GIT, optimized VS Code, and learned to link CSS and JavaScript. Understanding
client-server interaction sets the stage for creating dynamic and responsive web applications. Keep coding and
exploring!