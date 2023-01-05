# Contact-From
This is a simple contact form that allows website visitors to send messages and inquiries to the website owner or administrator. It is created using HTML and CSS, and the submitted data is stored in a Google Sheets spreadsheet for easy access and organization.

# Getting Started
1. Create a new form in Google Sheets using the Forms tool.
2. Create a new HTML file and link it to a CSS stylesheet (optional).
3. Use the following code to create the form:
<form id="contact-form" method="post" action="">
  <label for="name">Name:</label><br>
  <input type="text" id="name" name="name"><br>
  <label for="email">Email:</label><br>
  <input type="email" id="email" name="email"><br>
  <label for="subject">Subject:</label><br>
  <input type="text" id="subject" name="subject"><br>
  <label for="message">Message:</label><br>
  <textarea id="message" name="message"></textarea><br><br>
  <input type="submit" value="Submit">
</form> 


5. Use the Google Sheets API or a third-party service like JotForm or Wufoo to send the submitted form data to your Google Sheets spreadsheet.
#Customization
You can customize the form by adding or removing fields, changing the layout and styling, and adjusting the form behavior. For example, you can use JavaScript to validate the form data before it is submitted or to show a message after the form is submitted.

# Contact Form Example
Here is an example of how the contact form might look: [Visit Now](https://contact-from.vercel.app/)


# Support
If you have any questions or need help with the contact form, please don't hesitate to ask.
