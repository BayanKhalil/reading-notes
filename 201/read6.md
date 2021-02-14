# Domain Modeling
Domain model is a structured visual representation of interconnected concepts or real-world objects that incorporates vocabulary, key concepts, behavior, and relationships of all of its entities

Most of the time a domain model is illustrated with a set of class diagrams which may show:
* domain objects or conceptual classes
* associations between conceptual classes
* attributes of conceptual classes


we can Generate random numbers by 
> Math.floor(Math.random() * (max - min + 1)) + min
> Math.floor(): function returns the largest integer less than or equal to a given number.
> Math.random(): function returns a floating-point, pseudo-random number in the range 0 to less than 1 (inclusive of 0, but not 1) with     approximately uniform distribution over that range



# Tables 
Basic Table Structure
 1. The `<table>` element is used to create a table.
 2. You indicate the start of each row using the opening `<tr>` tag.
 3. Each cell of a table is represented using a `<td>` element.The `<th>` element put heading for either a column or a row

 * You can make cells of a table span more than one row or column using the rowspan and colspan attributes.

 Long Tables
 1. The headings of the table should sit inside the `<thead>` element.
 2. The body should sit inside the `<tbody>` element.
 3. The footer belongs inside the `<tfoot>` element.


# objects
accessing an objects in tow way
1. objectName.propertyName
2. objectName["propertyName"]
* A method is a function stored as a property.

types of objects:
1. LITERAL NOTATION
2. constructor notation

* creat objects in literal notation
```
var hotel = {
name: 'Quay',
rooms : 40,
booked: 25,
checkAvailability: function() {
return this.rooms - this.booked;
}
} 
```

* creat objects in constructor notation
```
var hotel = new Object();
hotel.name= 'Park';
hotel.rooms = 120;
hotel .booked = 77;
hotel .checkAvailability = function()
return this . rooms - this.booked;
}
```

 * MULTIPLE OBJECTS
When you need to create multiple objects within the
same page, you should use an object constructor to
provide a template for the objects.

```
function Hotel (name, rooms)
this .name = name;
this.rooms = rooms;
```
You then create instances of the object using the **new** keyword and then a call to the constructor function.
```
var hotell =new Hotel ( ' Quay', 40);
var hotel2 = new Hotel ( ' Park ' , 120);
```

**The this Keyword**
 In a function definition, this refers to the "owner" of the function.
 >In other words, `this.firstName` means the firstName property of this object.

## BUILT-IN OBJECTS
the new toolkit has three compartments
1. BROWSER OBJECT MODEL :creat model of the browser window or tab.
2. DOCUMENT OBJECT MODEL :creat model of the current web page.
3. GLOBAL JAVASCRIPT OBJECTS :agrouped of individual object that relate to different parts of js language


 