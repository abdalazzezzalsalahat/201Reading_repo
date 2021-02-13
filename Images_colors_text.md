# Images 
### Using the "<img src="">" to add images to a web page. 
## Three Rules for Creating Images
> **1. Save images in the right *format*.**
> **2. Save images at the right *size*.**
> **3. Use the correct *resolution*.**
## Image Dimensions
> **The images you use on your website should be saved at the same width and height that you want them to appear on the page.**
![Image Dimensions](https://zomasleep.com/blog/wp-content/uploads/2020/02/Artboard-Copy.jpg)
## Image Resolution 
> **Images created for the web should be saved at a resolution of *72 ppi*. The higher the resolution of the image, the larger the size of the file.**
![Image Resolution](https://upload.wikimedia.org/wikipedia/commons/f/f2/Resolution_illustration.png)
## Vector Images
> **they differ from bitmap images and are resolution-independent.**
![Vector Images](https://www.vectorizer.io/img/intro_raster_to_vector.svg?v4)
## Animated GIFs
> **Animated GIFs show several frames of an image in sequence and therefore can be used to create simple animations.**
> **Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.**
![Animated GIFs](http://msurguy.github.io/gifloopcoder.com/example3.gif)

# Colors 
> **The color property allows you to specify the color of text inside an element.**
![Colors](https://www.sessions.edu/wp-content/themes/divi-child/color-calculator/wheel-3-rgb.png)
> *Every color on a computer screen is created by mixing amounts of red, green, and blue.*
**we can specify colors as HSL values, with an optional opacity value. It is known as HSLA.**
### RGB values
**Express colors in terms of how much red, green and blue are used to make it up.**
*the numbers are valued **between 0 and 255**.*
**extra value for RGB colors to indicate opacity. It is known as RGBA.**
`color: rgb(100,100,90, 0);`
### Hex codes
**Six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash #**
*the numbers goes from '0' to '9' and from 'a' to 'f'.*
`color: #e2e2e2;`
### color names
**There are 147 predefined color names that are recognized by browsers.**
`color: red;`
### Hue
**Hue is near to the colloquial idea of color**
![Hue](https://i.stack.imgur.com/YOBFy.png)
### Saturation 
**Saturation refers to the amount of gray in a color.**
**At maximum saturation, there would be no gray in the color.**
**At minimum saturation, the color would be mostly gray.**
![Saturation](https://drawpaintacademy.com/wp-content/uploads/2019/10/Color-Saturation-Scale.jpg)
### Brightness
**Brightness (or "value") refers to how much black is in a color.**
**At maximum brightness, there would be no black in the color.**
**At minimum brightness, the color would be very dark.**
![Brightness](https://i.stack.imgur.com/QWEFy.png)

# Texts
> 
![Texts](https://s3.gomedia.us/wp-content/uploads/2008/10/font-structure.jpg)
### Font Weight
> **The font weight not only adds emphasis but can also affect the amount of white space and contrast on a page.**
***Light*, *Medium*, *Bold*, *Black*.**
![Font Weight](https://docs.microsoft.com/en-us/typography/opentype/otspec181/images/otvo_fig26d.png)

### Font Style
**Normal**
_Italic_
*Oblique*
**Italic fonts have a cursive aspect to some of the lettering.**
**Oblique font styles take the normal style and put it on an angle.**
![Font Style](https://next3-assets.s3.amazonaws.com/journeys/29/description_backgrounds-1423860873-font_intro.png)
### Font Stretch
**In condensed (or narrow) versions of the font, letters are thinner and closer together.**
**In expanded versions they are thicker and further apart.**
![Font Stretch](https://spiderinfomedia.files.wordpress.com/2014/03/font-stretch.gif)


### Choosing Typeface
> **It is important to understand that a browser will usually only display it if it's installed on that user's computer.**
![Typeface](https://newenglandrepro.com/wp-content/uploads/2016/08/BP-Serif-SansSerif-Graphic1-862x518.jpg)
```
@font-face{
    font-family: 'ChunkFiveRegular';
    src: url('fonts/chunkfive.eot');
} 
```
**The font-family property allows you to specify the typeface that**
**should be used for any text inside the element(s) to which a CSS rule applies.**
**The value of this property is the name of the typeface you want to use.**
**We can specify a list of fonts separated by commas so that, if the user does not have your first choice of typeface installed, the browser can try to use an alternative font from the list.**
`font-family: Georgia, Times, serif;`


### Font Size
> **The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font.**
**Pixels**
> The number of pixels is followed by the letters px.
`font-size: 30px;`
**percentages**
> *The default size of text in browsers is 16px. So a size of 75% would be the equivalent of 12px, and 200% would be 32px.*
`font-size: 200%;`
**EMS**
> **An em is equivalent to the width of a letter *m*.**
`font-size: 10em;`

### Type Scales
> *The default size of text in a browser is 16 pixels.*
> **So if you use percentages or ems, you calculate the size of text you want based on the default size of the text used in browsers.**
> **For example, you could scale down to 12 pixels for body copy and scale up to 24 pixels for headings.**
![Type Scales](https://i1.wp.com/www.layoutgridcalculator.com/wp-content/uploads/2019/03/modular_scale_Formula2.png?fit=585%2C351&ssl=1)

### Text decoration 
*none* *underline* *overline* *line-through* *blink*
`text-decoration: none;`
`line-height: 10px;`
`letter-spacing: 10px;`
`word-spacing: 10px;`
`text-align: left;`
`text-align: center;`
`text-align: right;`
`text-align: justify;`
`vertical-align: text-top;`
`vertical-align: baseline;`
`vertical-align: text-bottom;`
`text-indent: -9999px;`
`text-shadow: 1px 1px 0px #000000;`
`:first-letter`
`:first-line`
`:link`
`:visited`
`:hover`
`:active`
`:focus`
![Attribute Selectors](https://qph.fs.quoracdn.net/main-qimg-10d23bc1f01574213ebd806123fa024d)
