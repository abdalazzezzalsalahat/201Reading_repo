# HTML Images and to maniplate them in CSS
![img](https://repository-images.githubusercontent.com/134285701/635de980-586d-11ea-9220-1a3211239c30)
**We can specify the dimensions of images using CSS.**
**This is very helpful when we use the same sized images on several pages of our site.**
> *Images can be aligned both horizontally and vertically using CSS.*
```
body {
    background: #ffffff url("images/tulip.gif");
    no-repeat top right;
    } 
```
**We can use a background image behind the box created by any element on a page.**
`background-repeat`
`background-attachment`
`repeat`
`repeat-x`
`repeat-y`
`no-repeat`
`fixed`
`scroll`
`background-position: center center;`
> *Background images can appear just once or be repeated across the background of the box.*
**We can create image rollover effects by moving the background position of an image.**
```
#gradient {
    /* fallback color */
    background-color: #66cccc;
    
    /* fallback image */
    background-image: url(images/fallback-image.png);
    
    /* Firefox 3.6+ */
    background-image: -moz-linear-gradient(#336666,#66cccc);

    /* Safari 4+, Chrome 1+ */
    background-image: -webkit-gradient(linear, 0% 0%, 0% 100%, from(#66cccc), to(#336666));
    
    /* Safari 5.1+, Chrome 10+ */
    background-image: -webkit-linear-gradient(#336666,#66cccc);

    /* Opera 11.10+ */
    background-image: -o-linear-gradient(#336666,#66cccc);
    height: 150px;
    width: 300px;
}
```
**To reduce the number of images our browser has to load, we can create image sprites.**



# PRACTICAL INFORMATION
![img](http://www.travelia.uk/wp-content/uploads/2017/10/f6acff6591-e1509374747545-300x192.jpg)

**Search engine optimization helps visitors find our sites when using search engines.**
> *Analytics tools such as Google Analytics allow we to see how many people visit our site, how they find it, and what they do when they get there.*

> **To put our site on the web, we will need to obtain a domain name and web hosting.**
>> *FTP programs allow us to transfer files from our local computer to our web server.*
**Many companies provide platforms for blogging, email newsletters, e-commerce and other popular website tools (to save we writing them from scratch).**

# HTML video and audio
![img](https://disenowebakus.net/en/images/articles/audio-video-web-page-internet.jpg)
> **The `<video>` and `<audio>` elements allow us to embed video and audio into web pages.**
```
<video controls>
    <source src="rabbit320.mp4" type="video/mp4">
    <source src="rabbit320.webm" type="video/webm">
    <p>wer browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>
```
**I think we've taught we enough in this article. The HTMLMediaElement API makes a wealth of functionality available for*creating simple video and audio players, and that's only the tip of the iceberg*. See the "See also" section below for links to more complex and interesting functionality.**

> 1. *The time display currently breaks if the video is an hour long or more (it won't display hours; just minutes and seconds).*

> 2. *Because `<audio>` elements have the same HTMLMediaElement functionality available to them, we could easily get this player to work for an `<audio>` element too.*

> 3. *Can we work out a way to turn the timer inner <div> element into a true seek bar/scrobbler — i.e., when we click somewhere on the bar, it jumps to that relative position in the video playback? As a hint, we can find out the X and Y values of the element's left/right and top/bottom sides via the getBoundingClientRect() method, and we can find the coordinates of a mouse click via the event object of the click event, called on the Document object. For example:*