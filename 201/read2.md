# lists 
HTML provides us with three different types of lists
1. Ordered lists use numbers.

```
<ol>
    <li>     </li>
</ol>
```

2. Unordered lists use bullets

```
<ul>
    <li>     </li>
</ul>
```

3. Definition lists:usually consists of a series of terms and
their definitions.Inside the `<dl>` element you will
usually see pairs of `<dt>` and`<dd>` elements.

# Boxes
1. Control the dimensions of your boxes by height and width 

```
p {
height: 75%;
width: 75%;
background-color: #0088dd;
}
```

and we can limiting the width and height by

> min-width, max-width /min-height, max-height

Overflowing Content:

> hidden: This property simply hides any extra content that does not fit in the box.

> scroll: This property adds a scrollbar to the box so that users can scroll to see the missing content.

```
p {
overflow: hidden;}
p {
overflow: scroll;}
```

2. Create borders around boxes by

   `border-width` , `border-style` ,` border-color`

```
shorthand `border`
p {
width: 250px;
border: 3px dotted #0088dd;}

```

3. Set margins and padding for boxes

   `padding` :allows you to specify how much space should appear between the content of an element and its border.

   `margins` :controls the gap between boxes.

4. Show and hide boxes

   `display` :Change Inline/Block

   `visibility` :Hiding Boxes

   # Javascript
  array is a special type of variable. It doesn't just store one value; it stores a list of values.
  * when you creating an array it possible have var contain different data type (string,numbers,..)
  * we have tow type of array
  1.array literal (using var [])
  2.array constructor (using Array())

    ## switch statement
   A switch statement starts with avariable called the switch value.Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

    ```
   switch (level) {
     case 'O ne ':
     title= 'Level 1 ' ;
         break;
    case 'Two':
    tit 1 e = ' Level 2 ' ;
        break;
    default :
     title= 'Test';
        break;
   }
   ```

   ## datatype

   If you use a data type JavaScript did not expect, it tries to make sense of the operation rather than report an error.
   
DATA TYPE 
string=> Text
number=> Number
Boolean=> true or false
nul => Empty value
undefined =>Variable has been declared but not yet assigned a value
NaN=> is a value that is counted as a number.

   ## types of loop :

 1. while :Loops can execute a block of code as long as a specified condition is true.

 2. for :Loops can execute a block of code a number of times.

 3. do while : The key difference between a whi1e loop and a do whi1e loop is that the statements in the code block    come before the condition. This means that those statements are run once whether or not the condition is met.