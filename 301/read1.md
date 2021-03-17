# Responsive Web Design

this term coined by Ethan Marcotte and it's mean how to building a website suitable to work on every device and every screen size

**Responsive web design is have three main components**
1. **including flexible layouts**: is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. Flexible grids are built using relative length .
```
The formula is based around taking the target width of an element and dividing it by the width of it’s parent element. The result is the relative width of the target element

> target ÷ context = result

section,
aside {
  margin: 10px;
}
section,
aside {
  margin: 1.858736059%; /*  10px ÷ 538px = .018587361 */
}
where 538px is the width of parent div
```

2. **media queries**

recommend to use the `@media` rule inside of an existing style sheet
```
 @media Rule 
@media all and (max-width: 1024px) {...}

@import Rule 
@import url(styles.css) all and (max-width: 1024px) {...}
```
#### There are three different logical operators available for use within media queries
- and : allows an extra condition to be added
> @media all and (min-width: 800px) and (max-width: 1024px) {...}
- not : specifying any query but the one identified
> @media not screen and (color) {...}
- only: hiding the styles from devices or browsers that don’t support media queries
> @media only screen and (orientation: portrait) {...}

### Media Features
- Height & Width 
- Orientation  :determines if a device is in the landscape or portrait orientation
> @media all and (orientation: landscape) {...}
- Aspect Ratio :The value for the aspect ratio feature consist of two positive integers separated by a forward slash. The first integer identifies the width in pixels while the second integer identifies the height in pixels
>@media all and (min-device-aspect-ratio: 16/9) {...}
- Resolution 
> @media print and (min-resolution: 300dpi) {...}

* **Mobile First** : it's most popular technique with using media queries,which approach includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows
```
/* Default styles first then media queries */
@media screen and (min-width: 400px)  {...}
```
### Viewport
- Height & Width 
> <meta name="viewport" content="width=device-width">
- scale :use the `minimum-scale`, `maximum-scale`, `initial-scale`, and `user-scalable` properties
  initial, minimum,maximum-scale should always be a positive integer between 0 and 10
  setting the `user-scalable value` to yes will turn on zooming
- Resolution
> <meta name="viewport" content="target-densitydpi=device-dpi">
* Combining Viewport Values :The viewport meta tag will accept individual values as well as multiple values
> <meta name="viewport" content="width=device-width, initial-scale=1">
```
viewport in css most recommended
@viewport {
  width: device-width;
  zoom: 1;
}
```

3. **flexible media**
One quick way to make media scalable is by using the max-width property =100%,
To get embedded media to be fully responsive,by this steps
* parent element needs to have a width of 100% 
* parent element also needs to have a height of 0
* Padding-bottom of the parent element, the value of which is set in the same aspect ratio of the video
the code 
```
HTML
<figure>
  <iframe src="https://www.youtube.com/embed/4Fqg43ozz7A"></iframe>
</figure>
CSS
figure {
  height: 0;
  padding-bottom: 56.25%; /* 16:9 */
  position: relative;
  width: 100%;
}
iframe {
  height: 100%;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
}
```


# All About Floats
when we distribution the element during the website design we asked what is the best way to put the element beside each other In an orderly way without `absolute position ` command cause it bad way , the way was by `Float` which the elemnt can flow in appropriate way .
* float used for entire web layouts
* ` clear:both` will not move up adjacent to the float like the float desires, but will move itself down past the float
*   We fix the Collapsing by clearing the float after the floated elements in the container but before the close of the container

*Techniques for Clearing Floats*

* The Empty Div Method :` <div style="clear: both;"></div>`
* The Overflow Method : If this property is set to auto or hidden on the parent element, the parent will expand to contain the floats
* The Easy Clearing Method
```
.clearfix:after { 
   content: "."; 
   visibility: hidden; 
   display: block; 
   height: 0; 
   clear: both;
}
```




              