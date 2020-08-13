# Readings: Form and JS Events

## Duckett HTML Book

### Forms (144-175)
<br>
How to collect information from visitors, different kinds of form controls, and new HTML5 for controls. You can make a few different types of forms that control information your users store on your site. When adding text, you can use a text input like a single line for an email, a password input that masks the characters put inside, or a text area for longer messages like comments or messages. When addign buttons you can make radio buttons, checkboxes, or drop-down boxes. When submitting forms you can have a subscribe/submit button, or an image button, that lets you use a picture as the submit option. 
<br>

**HOW FORMS WORK**
1. A user fills in a form and then presses a button
to submit the information to the server.
2. The name of each form control is sent to the server along with the value the user enters or selects.
3. The server processes the information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information in a database.
4. The server creates a new page to send back to the browser based on the information received.
<br>

A form may have several different form controls, each gathering different information. The server needs to know which piece of inputted data corresponds with which form element. i.e. username=Ivy vote=Herbie. syntax pages (151-168)
<br>

**SUMMARY**
1. Whenever you want to collect information from visitors you will need a form, which lives inside a <form> element.
2. Information from a form is sent in name/value pairs.
3. Each form control is given a name, and the text the user types in or the values of the options they select are sent to the server. 
4. HTML5 introduces new form elements which make it easier for visitors to fill in forms.



### Lists, Tables, & Forms (330-357)
<br>

<ul>
  <li>Specifying bullet point styles</li>
  <li>Adding borders and backgrounds to tables</li>
  <li>Changing the appearance of form elements</li>
</ul>

<br>

You can change the styles of bullet points, to something like roman numerals or stars in css. ex. 
<br>
ul {
  list-style-image: url("images/star.png";
}
<br>
or
<br>
ol {
  list-style-type: lower-roman;
}
<br>

Here are some table elements we already know; width, padding, text-transform, letter-spacing, font-size, border-top, border-bottom, text-align, background-color, :hover. Give cells of tables some padding, make headings bold to distinguish them, shade alternating rows for readability, align numerals to the large numbers are clearly distinguished form the smaller ones. TIP if you  have an empty cell you can specify it and make its borders invisible. you can also collapse gaps between cells if you need, with border-collapse: collapse; 
<br>

Fieldsets help distinguish the contents of a form and can be styled. You can also style submit buttons, to help readability. You can change the cursor style when hovering a form.
<br>

Examples (351-354)
<br>

**SUMMARY**
1. In addition to the CSS properties covered in other chapters which work with the contents of all elements, there are several others that are specifically used to control the appearance of lists, tables and forms.
2. List markers can be given different appearances using the list-style-type and list-style image properties.
3. Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent.
4. Forms are easier to use if the form controls are vertically aligned using CSS.
5. Forms benefit from styles that make them feel more interactive.
<br>

## Duckett JS Book

### Events (243-292)
<br>

Event breakdown- its the browsers way of saying 'hey this happened' so your script can then respond to these events. Interactions create events, events trigger code, code responds to user. There is a compendium of event types on pg (246). Note, events 'fire' or 'are raised'.
<br>

**HOW EVENTS TRIGGER JAVASCRIPT CODE**
<br>

1. Select element node(s) you want the script to respond to.
2. Indicate which event on the selected node(s) will trigger the response.
3. State the **code** you want to run when the event occurs.
<br>

Event Listeners
<br>
Event listeners are a more recent approach to handling events. They can deal with more than one function at a time but they are not supported in older browsers. how to add an event listener to the DOM:
<br>

element.addEventListener('event', functionName [,Boolean]);

function checkUsername(){
  //code to check the length of username
}

var el = document.getElementById('username');
el.addEventListener('blur', checkUserName, false);
<br>

Event Flow
<br>

HTML elements nest inside other elements. If you hover or click on a link, you will also be hovering or clicking on its parent elements. The event object has methods that change: the default behavior of an element and how the element's ancestors respond to the event. you need to use preventDefault ().
<br>

Mouse Events:
<br>

There are many types of mouse events. These include but are not limited to; click, dbclick, mousedown, mouseup, mouseover, mouseout, mousemove.
<br>

KeyBoard Events:
<br>

Here are a few keyboard events: input, keydown, keypress, keyup.
<br>

Example Events: pg (288-291)
<br>

**SUMMARY**
<br>

1. Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked).
2. Binding is the process of stating which event you are waiting to happen, and which element you are waiting fot that even to happen upon.
3. When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user.
4. You can use event delegation to monitor for events that happen on all of the children of an element.
5. The most commonly used events are W3C DOM events, although there are others in the HTML5 specification as well as browser-specific events.






[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)