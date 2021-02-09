# links 
we writing links by  `<a> `tags
 1. Linking to Other Sites
 ` <a href="http://www.empireonline.com">Empire</a>` 
 2. Linking to Other Pages on the Same Site
  `<a href="index.html">Home</a>`
3. Email Links :To create a link that starts up the user's email program and addresses an email to a specified
email address, by `mailto`
`<a href="mailto:jon@example.org">Email Jon</a>`
4. Opening Links in a New Window:
If you want a link to open in anew window, you can use the` target `attribute on the opening
`<a> `tag. The value of this attribute should be `_blank`.
`<a href="http://www.imdb.com" target="_blank">Internet Movie Database</a>`

# Layout
Key Concepts in Positioning Elements
1. Building Blocks :CSS treats each HTML element as if it is in its own box.
This box will either be a block-level which start in anew line` <h1> <p> <ul> <li>`
box or an inline box. flow in between surrounding text`<img> <b> <i>`
2. Containing Elements: If one block-level element sits inside another
block-level element then the outer box is known as the containing or parent element.

* CSS has the three positioning schemes that allow you to control the layout of a page:
 `normal flow, relative positioning, and absolute positioning.`

 * To indicate where a box should be positioned, you may also need to use box offset properties
  if it  `Fixed Positioning ` or  `Floating Elements `

# javascript

  functions and method and objects :
  **function**: consist of a series of statements that have been grouped together because they perform aspecific tak 
  **method**: is the same as function ,except methods are created inside and part of object

  **objects**: we use it create models of the world using data and it made up of properties and methods 

types of function
  1. declaring function
```
function sayHello(){
   return document.write('hello'); 
}
sayHello();
```
2. expresstion function
```
var showImage = function() {
    code...code
}
showImage();
```

*variable scope* :

The location where you declare a variable will affect where it can be used
within your code. If you declare it within a function, it can only be used
within that function. This is known as the variable's scope.
1. When a variable is created inside a function using the var keyword, it can only be used in that function. its called 
**local var**

2. If you create a variable outside of a function, then it can be used anywhere within the script.its called **global var**


 # the article about pair programming 

 pair programming is the practice of two developers sharing a single workstation to interactively tackle a coding task togethe.
 theres a tow roles when we writing the code 

 1. the Driver: Driver manages the text editor, switching files, version control, and code
 2. The Navigator: thinks about the big picture.

 Pair programming touches on all four skills listening ,reading, writing ,speaking, developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves and it will give alot of benefites that will improve all our skills that we need during the work even skills on personal level
