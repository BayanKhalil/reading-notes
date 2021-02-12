# objects
object :Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,variables and functions take on new names.
which *VARIABLES BECOME KNOWN AS PROPERTIES, and FUNCTIONS BECOME KNOWN AS METHODS*

* there are several way to creat objects letiral notation is the most popular way to creat it 
   we called it with a var and put the property and methods into curly brace and seperate between them by comma
   we access it by dot notation or squer brackets


   # DOM
   The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.
   The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules. It is implemented by all major browser makers, and covers two primary areas:
   1. MAKING A MODEL OF THE HTML PAGE :The DOM specifies the way in which the browser should structure this model using a DOM tree. The DOM is called an object model because is made of objects.
   2. ACCESSING AND CHANGING THE HTML PAGE

   * The DOM tree is  a model of a web page It consists of four main types of nodes.
   1. THE DOCUMENT NODE
   2. ELEMENT NODES
   3. ATTRIBUTE NODES
   4. TEXT NODES

   * ACCESSING ELEMENTS
* METHODS THAT RETURN A SINGLE ELEMENT NODE

`getElementByld('id')`

* METHODS THAT RETURN ONE OR MORE ELEMENTS (AS A NODELIST)

`getElementsByClassName('class')`

* SELECTING ELEMENTS USING CLASS ATTRIBUTES
```
var elements = document .getElementsByClassName('hot');       // Find hot items
if (elements.length> 2) {                                     // If 3 or more are found
var el = elements[2];                                         // Select the th i rd one from the Nodelist
el.className = 'cool';}                                       // Change the value of its class attribute
}
```
* SELECTING ELEMENTS BY TAG NAME
```
var elements = document.getElementsByTagName('li '); 
if (elements.length> O) {
var el = elements[O];
el.className = 'cool';
}
```
* SELECTING ELEMENTS USING CSS SELECTORS
```
// querySel ector() only retur ns the fi rst match
var el = document .querySel ector('li .hot ' };
el.className = ' cool' ;
// querySel ectorAll returns a Nodeli st
// The second matching element (the t hird list item) is selected and changed
var el s = document.querySelectorAll('li .hot') ;
els[l] .className = ' cool' ;
```
* LOOPING THROUGH A NODELIST
```
var hotltems = document.querySelectorAll('li. hot') ;       // Store Nodel i st in array
if (hot ltems.length > O) {                                      // If it contains items
for (var i=O; i<hotl tems.length; i++) {                         // Loop through each item
hotltems[i].className = 'cool';                                // Change value of class attribute
}
}
```
* ACCESSING & CHANGING A TEXT NODE
```
var itemTwo document.getElementByld('two');                        // Get second l ist item
var elText itemTwo.firstChild .nodeValue;                          // Get its text content
elText = elText.replace( ' pine nuts', ' kal e ' );                // Change pine nuts to ka le
itemTwo . firstChi ld.nodeValue = elText;                          // Update the li st item
                                                                   
```
* From an element node, you can access and update its content using properties such as textContent and
innerHTML or using DOM manipulation techniques.   
* An element node can contain multiple text nodes and child elements that are siblings of each other.                                                                
                                                                   
