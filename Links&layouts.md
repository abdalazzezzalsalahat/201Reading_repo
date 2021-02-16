# Links
> *`<a href="Link goes here">'any text to show in the page'</a>`*
**- *Using the <a> element.***
**- *It uses the href attribute to indicate the page you are linking to.***
**- *To link a page within your own site, it is best to use relative links rather than qualified URLs.***
**- *We can create links to open email programs with an email address in the "to" field.***
**- *Also we can use the id attribute to target elements within a page that can be linked to.***

# Layouts
> **There are tons of different layout designs to choose from. However, the structure above, is one of the most common, and we will take a closer look at it in this tutorial.**

## Elements Positioning
> **To specify the positioning scheme use the *position* property in CSS.** 
> **We can also float elements using the *float* property.**

## Normal Positioning
> *Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.*
**`position:static`**
## Relative Positioning
> *This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed.*
**`position:relative`**
## Absolute Positioning
> *This positions the element in relation to its containing element.*
**`position:absolute`**
## Fixed Positioning
> *This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element.*
**`position:fixed`**
## Overlapping Elements
> *It allows you to control which box appears on top.*
**`z-index`**
## Floating Elements
> *Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box.*
**`float: direction`'left, right'**
**We can use the float to place elements side-by-side**
### Clearing floats
> **The clear property allows you to say that no element should touch the left or righthand sides of a box.**
*`clear: values`'left, right, both, none'.*
## Screen Resolution
> **Resolution refers to the number of dots a screen shows per inch.**
> *Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.*
### Fixed width layouts
> **Advantages**
*1. Pixel values are accurate at controlling size and positioning of elements.*
*2. We have far greater control over the appearance and position of items on the page than with liquid layouts.*
*3. We can control the lengths of lines of text regardless of the size of the user's window.*
*4. The size of an image will always remain the same relative to the rest of the page.*
> **Disadvantages**
*1. We can end up with big gaps around the edge of a page.*
*2. the page can look smaller and text can be harder to read.* 
*3. If a user increases font sizes, text might not fit into the allotted spaces.*
*4. The design works best on devices that have a site or resolution similar to that of desktop or laptop computers.*
*5. The page will often take up more vertical space than a liquid layout with the same content.*
## Liquid Layouts
> **The liquid layout uses percentages to specify the width of each box so that the design will stretch to fit the size of the screen.**
![Liquid Layout](http://maxdesign.com.au/maxdesign/wp-content/uploads/2015/04/grid.gif)
## Grid Layouts 
![Grid Layouts](https://i.ytimg.com/vi/v5KzBPUEgGQ/maxresdefault.jpg)
## CSS Frameworks
![CSS Frameworks](https://cdn.tutsplus.com/net/uploads/legacy/178_960Framework/20090114-154700.png)
> **Advantages**
*- They save you from repeatedly writing code for the same tasks.*
*- They will have been tested across different browser versions.*
> **Disadvantages**
*- They often require that you use class names in your HTML code that only control the presentation of the page.*
*- In order to satisfy a wide variety of needs, they often contain more code than you need for your particular web page.*
## Using multiple Style files
