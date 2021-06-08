Forms and JS Events
 (Links to an external site.)HTML Forms :
 (Links to an external site.)An HTML form is used to collect user input. The user input is most often sent to a server for processing.
 (Links to an external site.)Form Controls:
There are several types of form controls that you can use to collect information from visitors to your site.

 (Links to an external site.)ADDING TEXT:
Text input (single-line):

Used for a single line of text such as email addresses and names.

Password input:

Like a single line text box but it masks the characters entered.

Text area (multi-line):

For longer areas of text, such as messages and comments.

 (Links to an external site.)Making Choices:
Radio buttons:

For use when a user must select one of a number of options.

Checkboxes:

When a user can select and unselect one or more options.

Drop-down boxes:

When a user must pick one of a number of options from a list.

 (Links to an external site.)Submitting Forms:
Submit buttons:

To submit data from your form to another web page.

Image buttons:

Similar to submit buttons but they allow you to use an image.

 (Links to an external site.)How Forms Work:
A user fills in a form and then presses a button to submit the information to the server.
The name of each form control is sent to the server along with the value the user enters or selects.
The server processes the information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information in a database.
The server creates a new page to send back to the browser based on the information received.
form

 (Links to an external site.)Styling Forms:
font-size sets the size of the text entered by the user.

color sets the text color, and background-color sets the background color of the input.

border adds a border around the edge of the input box, and border-radius can be used to create rounded corners (for browsers that support this property).

The :focus pseudo-class is used to change the background color of the text input when it is being used, and the :hover psuedo-class applies the same styles when the user hovers over them.

background-image adds a background image to the box. Because there is a different image for each input, we are using an attribute selector looking for the value of the id attribute on each input.

 (Links to an external site.)What is an Event ?
 (Links to an external site.)JavaScript's interaction with HTML is handled through events that occur when the user or the browser manipulates a page.When the page loads, it is called an event. When the user clicks a button, that click too is an event. Other examples include events like pressing any key, closing a window, resizing a window, etc.
 (Links to an external site.)Developers can use these events to execute JavaScript coded responses, which cause buttons to close windows, messages to be displayed to users, data to be validated, and virtually any other type of response imaginable.
 (Links to an external site.)Events are a part of the Document Object Model (DOM) Level 3 and every HTML element contains a set of events which can trigger JavaScript Code.
 (Links to an external site.)HOW EVENTS TRIGGER JAVASCRIPT CODE
 (Links to an external site.)When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as event handling.
Select t he element node(s) you want the script to respond to.

Indicate which event on the selected node(s) will trigger the response.

State the code you want to run when the event occurs.

< button onclick="document.getElementById('demo').innerHTML = Date()">The time is?

The time is?
