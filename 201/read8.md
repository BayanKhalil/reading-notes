# forms
An HTML form is used to collect user input. The user input is most often sent to a server for processing and tore
the information in a
database. then the server creats new page to send back to the browser


### form structure
we have `action` attribute into `form` element and it's value is URL for information page 

the input element 
An `<input>` element can be displayed in many ways, depending on the type attribute

`text` Displays a single-line text input field
`radio` Displays a radio button (for selecting one of many choices)
`checkbox`Displays a checkbox (for selecting zero or more of many choices)
`submit`Displays a submit button (for submitting the form )
`button`Displays a clickable button


`<label>` tag defines a label for many form elements inside it `for` attribute which The value of the for attribute
matches that of the id attribute on the of the `<input>` 

* HTML5 introduces new form elements which make it easier for visitors to fill in forms like:
`type="date"` 
`type="email"` 
`type="url"`
`type="search"`


# lists and tables
The CSS list properties allow you to:

Set different list item markers for ordered lists
Set different list item markers for unordered lists
Set an image as the list item marker

*different List style Item
`list-style-type`
`list-style-image`
`list-style-position`

The CSS list give tips  to style your table like give cells padding, distinguish heading , shade alternative row and align numbers and theres a prperties can help you in different things like `empty-cells` to border it  with `show ` value or not with `hide ` value and you can control the distance between cells `border-scacing`or `border-collaps`
and you can style every element in your page ,styling the text, styling submit button, and the fieldsets etc...



# events
JavaScript's interaction with HTML is handled through events that occur when the user or the browser manipulates a page.
When the page loads, it is called an event. When the user clicks a button, that click too is an event.mouseover an element .
* Events are said to trigger a function or script. When the click event fires on any element it could trigger a script that enlarges the selected item. and thers a steps involved in getting it to trigger some JavaScript code Together known as event handling.first select the element then spicify event then  call the code.

* Binding is the process of stating which event you are waiting to happen, and which element you are waiting
for that event to happen upon. and there three way to bind elements we will work with traditional dom event handlers which
All modern browsers understand this way of creating an event handler, but you can only attach one function to each event handler. and event listeners can deal with more than one function at a time

* event object : tells you information about the event, and the element it happened upon

* You can use event delegation to monitor for events
that happen on all of the children of an element.
* The most commonly used events are W3C DOM
events,






