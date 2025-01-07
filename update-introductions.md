## Meet the Team - Part 2: HTML and CSS

This activity builds upon the previous Git introduction, focusing on HTML structure, basic CSS styling, and further Git branching.

**Recap:** You should already have a local copy of the `meet-the-team` repository with your introduction file.

**Part 1: Upgrading to HTML (lastname-html branch)**

1.  **Create a New Branch:**
    *   In your terminal, ensure you're on the `main` branch: `git checkout main`
    *   Create and switch to a new branch named `lastname-html` (replace `lastname` with your actual last name): `git checkout -b lastname-html`

2.  **Convert to HTML:**
    *   Rename your `introduction-your-name.txt` file to `introduction-your-name.html`.
    *   Open the file in a text editor and add the basic HTML structure:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Introduction - Your Name</title>
</head>
<body>
    </body>
</html>
```

3.  **Add Content with HTML Elements:**
    *   Replace the plain text with structured HTML.
    *   See content contained within demo file, at bare minimum it should include everything there. [Example: introduction-charles-jester.html](https://github.com/2164-ServiceNow/meet-the-team/blob/jester-html/introduction-charles-jester.html)

4.  **Commit and Push:**
    *   Stage your changes: `git add .`
    *   Commit: `git commit -m "Convert introduction to HTML"`
    *   Push: `git push -u origin lastname-html`

**Part 2: Adding CSS (lastname-css branch)**

1.  **Create a New Branch (from the HTML branch):**
    *   Create and switch to a new branch named `lastname-css`: `git checkout -b lastname-css`

2.  **Add CSS Styling:**
    *   Create a new file named `styles.css` in the same directory as your HTML file.
    *   [Example CSS stylings found in this branch on repo](https://github.com/2164-ServiceNow/meet-the-team/tree/jester-css)

    *   **Inline Styles:** Add inline styles directly to HTML elements (use sparingly in real projects, but good for demonstration).

```html
<p style="color: blue; font-size: 16px;">This text is blue.</p>
```

    *   **Internal Styles:** Add a `<style>` tag within the `<head>` of your HTML file:

```html
<head>
    <title>Introduction - Your Name</title>
    <style>
        h1 {
            text-align: center;
        }
    </style>
</head>
```

    *   **External Styles:** Link your `styles.css` file in the `<head>` of your HTML:

```html
<head>
    <title>Introduction - Your Name</title>
    <link rel="stylesheet" href="styles.css">
</head>
```

    *   **CSS Content (in styles.css):** Use a variety of selectors and properties, including box model properties:

```css
/* Element Selector */
body {
    font-family: sans-serif;
    margin: 20px; /* Box Model: Margin */
}

/* Class Selector */
.highlight {
    background-color: yellow;
    padding: 10px; /* Box Model: Padding */
    border: 1px solid black; /* Box Model: Border */
}

/* ID Selector */
#message {
    width: 100%;
    box-sizing: border-box; /* Box Model: Include padding and border in element's total width and height */
}

/* Table styling */
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
    padding: 5px;
}

/* List styling */
ul {
    list-style-type: square;
}

img{
    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 50%;
}
```

3.  **Apply CSS:** Apply classes and IDs to your HTML elements to use the styles you've defined.

4.  **Commit:**
    *   Stage: `git add .`
    *   Commit: `git commit -m "Add traditional CSS styling"`

5. **(Self Study) Implement Grid or Flexbox with a CSS Framework**
    *   Through the use of provided documentation & any other research, implement Grid or Flexbox and include a CSS framework from below. Note: Grid or Flexbox does not require a framework, just trying to kill 2 birds 1 stone.
    *   [Grid Resource Link](https://css-tricks.com/snippets/css/complete-guide-grid/)
    *   [Flexbox Resource Link](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
    *   [Bootstrap CSS Framework Documentation](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
    *   [Tailwind CSS Framework Documentation](https://tailwindcss.com/docs/installation)

4.  **Commit & push:**
    *   Stage: `git add .`
    *   Commit: `git commit -m "Add traditional CSS styling"`
    *   Push: `git push origin lastname-css`
    *   Create a pull request on GitHub from `lastname-css` to `lastname-html`. Request review from a peer.

5. Tomorrow, present these to you groups discussing what it is you implemented. Going over grid or flexbox basics, along with the css frameworks. Include some discussion about what you liked, disliked, or any questions.