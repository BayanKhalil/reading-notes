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


* `z-index` When you use relative, fixed, orabsolute positioning, boxes can overlap. If boxes do overlap, the
elements that appear later in the HTML code sit on top of those that are earlier in the page.

`float `  allows you to take an element in normal flow and place it as far to the left or right of the containing
element as possible.

 `clear` allows youto say that no element (withinthe same containing element) should touch the left or righthand
sides of a box. It can take the following values:

 `Screen Sizes`
Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.

`Screen Resolution` Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.


Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide(since most users will be able to see designs this wide on their screens).

`Fixed Width Layouts`Fixed width layout designs do not change size as the user increases or decreases
the size of their browser window. Measurements tend to be given in pixels.

`Liquid Layouts` Liquid layout designs stretch and contract as the user increases or decreases the size of their browser
window. They tend to use percentages.


* Composition in any visual art (such as design, painting, or photography) is the placement or arrangement of visual elements — how they are organized on a page. Many designers use a grid structure to help them
position items on a page, and the same is true for web designers.

* CSS Frameworks provide rules for common tasks and You can include multiple CSS files in one page.