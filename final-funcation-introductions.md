## Meet the Team - Part 3: Adding JavaScript Functionality 

**Part 1: Setting up JavaScript (lastname-js branch)**

1.  **Create a New Branch:**
    *   Ensure you are on your `lastname-css` branch: `git checkout lastname-css`
    *   Create and switch to a new branch named `lastname-js`: `git checkout -b lastname-js`

2.  **Create a JavaScript File:**
    *   Create a new file named `script.js` in the same directory as your HTML and CSS files.

3.  **Link the JavaScript File:**
    *   Add a `<script>` tag at the end of the `<body>` in your HTML file to link your JavaScript file:

```html
<body>
    ... your HTML content ...
    <script src="script.js"></script>
</body>
```

**Part 2: JavaScript Functionality (Examples and Requirements)**

Implement the following JavaScript functionalities. These are examples, and you can encourage creativity and variations.

1.  **Dynamic Content Update:**
    *   Add an element (e.g., a `<p>` tag with an ID) to your HTML.
    *   Use JavaScript to change the content of this element dynamically (e.g., display a welcome message with the current time).

```html
<p id="dynamic-message"></p>
```

```javascript
// script.js
const messageElement = document.getElementById('dynamic-message');
const currentTime = new Date();
messageElement.textContent = `Welcome! The current time is: ${currentTime.toLocaleTimeString()}`;
```

2.  **Form Validation:**
    *   Improve the form on your page by adding client-side validation using JavaScript. You can validate:
        *   Required fields.
        *   Email format.
        *   Minimum/maximum length of text inputs.

```html
<form id="contact-form">
    <label for="email">Email:</label><br>
    <input type="email" id="email" name="email" required><br><br>
    <span id="email-error" style="color:red; display:none;">Please enter a valid email address.</span>
    <input type="submit" value="Submit">
</form>
```

```javascript
//script.js
const form = document.getElementById('contact-form');
const emailInput = document.getElementById('email');
const emailError = document.getElementById('email-error');

form.addEventListener('submit', (event) => {
  if (!emailInput.checkValidity()) {
    event.preventDefault(); // Prevent form submission
    emailError.style.display = 'block';
  } else {
      emailError.style.display = 'none';
  }
});

```

3.  **Image Manipulation (Optional but Recommended):**
    *   Use JavaScript to change the `src` attribute of your image dynamically (e.g., change the image on mouseover or after a delay).

```html
<img id="my-image" src="your-image.jpg" alt="Your Photo" width="200">
```

```javascript
//script.js
const image = document.getElementById('my-image');
image.addEventListener('mouseover', () => {
    image.src = "another-image.jpg"; // Replace with path to another image
});
image.addEventListener('mouseout', () => {
    image.src = "your-image.jpg"; // Replace with path to original image
});
```

4.  **`onClick` Event with Buttons:**
    *   Add a button to your HTML.
    *   Use the `onClick` attribute directly in the HTML to call a JavaScript function. This function could perform a simple action, like displaying an alert or changing text.

```html
<button onclick="showAlert()">Click Me!</button>
<p id="button-message"></p>

<script>
    function showAlert() {
        alert("Button Clicked with onClick!");
        document.getElementById("button-message").textContent = "Button was clicked";
    }
</script>
```

5.  **Event Handling (Non-Click Example):**
    *   Use a different event listener other than `click`. Good examples include:
        *   `mouseover`/`mouseout`: Change the appearance of an element when the mouse hovers over it.
        *   `focus`/`blur`: Change the appearance of a form input when it gains or loses focus.
        *   `keydown`/`keyup`: Respond to keyboard input.
        *   `load`: Execute code after the page has fully loaded.

Example using `mouseover` and `mouseout`:

```html
<div id="hover-box" style="width: 100px; height: 100px; background-color: lightblue;">Hover Over Me</div>
```

```javascript
//script.js
const hoverBox = document.getElementById('hover-box');

hoverBox.addEventListener('mouseover', () => {
    hoverBox.style.backgroundColor = 'lightgreen';
});

hoverBox.addEventListener('mouseout', () => {
    hoverBox.style.backgroundColor = 'lightblue';
});
```

Example using `focus` and `blur`:

```html
<input type="text" id="my-input" placeholder="Type something">
```

```javascript
//script.js
const myInput = document.getElementById('my-input');

myInput.addEventListener('focus', () => {
    myInput.style.borderColor = 'blue';
});

myInput.addEventListener('blur', () => {
    myInput.style.borderColor = 'gray';
});
```

6. **(Self-Study)Utilize localStorage in some way**
    * [localStorge documentation](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage)

**Part 3: Commit and Push**

1.  Stage your changes: `git add .`
2.  Commit: `git commit -m "Add JavaScript functionality"`
3.  Push: `git push origin lastname-js`
4.  Create a pull request on GitHub from `lastname-js` to `main`. Request review from a peer.

