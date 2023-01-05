# Contact-From
This is a simple contact form that allows website visitors to send messages and inquiries to the website owner or administrator. It is created using HTML and CSS, and the submitted data is stored in a Google Sheets spreadsheet for easy access and organization.

# Getting Started
1. Create a new form in Google Sheets using the Forms tool.
2. Create a new HTML file and link it to a CSS stylesheet (optional).
3. Use the following code to create the form:

```html
    <div class="form-container">
        <form name="submit-to-google-sheet">
            <input name="email" type="email" placeholder="Email" required>
            <input name="text" type="text" placeholder="Phone" required>
            <input name="firstName" type="text" placeholder="First Name">
            <input name="lastName" type="text" placeholder="Last Name">
            <textarea name="message" id="" cols="40" rows="3" placeholder="Your Message"></textarea>
            <button type="submit">Send</button>
            <span id="msg"></span>
        </form>
    </div>
</form>
```
```css
:root {
    --accent: #F18260;
    --purple: #252431;
  }

  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body {
    background: #eee;
    color: var(--purple);
    padding: 10% 5%;
    font-family: system, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
    line-height: 1.4;
  }

  .form-container {
    position: relative;
    background: #fff;
    padding: 2rem;
    border-radius: 6px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    width: 350px;
    min-height: 300px;
    margin: 0 auto;
    box-shadow: 0 10px 50px 0 #ccc;
    margin-bottom: 2rem;
  }

  input,textarea, button {
    appearance: none;
    border: none;
    font-size: inherit;
    background: #eee;
    border-radius: 3px;
    padding: 1rem;
    width: 100%;
  }

  input {
    margin-bottom: 1rem;
  }

  input:focus {
    outline: 1px solid var(--accent);
  }

  button {
    color: #fff;
    cursor: pointer;
    background-color: var(--purple);
  }

  button:hover {
    background-color: var(--accent);
  }

  .is-hidden {
    display: none !important;
  }

  a {
    display: block;
    width: max-content;
    margin: 0 auto;
    color: var(--accent);
    text-decoration: none;
    margin-bottom: 0.5rem;
  }

  @keyframes rotate {
   100% { transform: rotate(360deg); }
  }

  @keyframes dash {
   0% { stroke-dasharray: 1,200; stroke-dashoffset: 0; }
   50% { stroke-dasharray: 89,200; stroke-dashoffset: -35; }
   100% { stroke-dasharray: 89,200; stroke-dashoffset: -124; }
  }

  .loading {
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .loading-spinner {
    width: 50px;
    height: 50px;
  }

  .loading-spinner svg {
    position: relative;
    animation: rotate 2s linear infinite;
    height: 50px;
    width: 50px;
  }

  .loading-spinner circle {
    stroke: var(--accent);
    stroke-dasharray: 1,200;
    stroke-dashoffset: 0;
    stroke-linecap: round;
    animation: dash 1.5s ease-in-out infinite;
  }
```

5. Use the Google Sheets API or a third-party service like JotForm or Wufoo to send the submitted form data to your Google Sheets spreadsheet.
#Customization
You can customize the form by adding or removing fields, changing the layout and styling, and adjusting the form behavior. For example, you can use JavaScript to validate the form data before it is submitted or to show a message after the form is submitted.

# Contact Form Example
Here is an example of how the contact form might look: [Visit Now](https://contact-from.vercel.app/)


# Support
If you have any questions or need help with the contact form, please don't hesitate to ask.
