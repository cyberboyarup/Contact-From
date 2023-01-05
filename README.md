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
