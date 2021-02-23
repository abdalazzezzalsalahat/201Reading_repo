# Transforms
![img](https://miro.medium.com/max/900/1*_6MfwckxNfQTca9SiG8MdQ.png)
> *With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the `transform` property.*

```
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```
### 2D Rotate
*The `transform` property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element `clockwise`, and using a negative value will rotate the element `counterclockwise`. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically. Later we will discuss how you can change this default point of rotation.*
```
.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}
```
![img](https://cloud.netlifyusercontent.com/assets/344dbf88-fdf9-42bb-adb4-46f01eedd629/d8ec8964-0bd6-4256-8d9d-d5dcc8d29b27/transform-rotate.png)
### 2D Skew
*The last `transfor`m value in the group, `skew`, is used to distort elements on the horizontal `axis`, vertical `axis`, or both. The syntax is very similar to that of the `scale` and translate values. Using the `skewX` value distorts an element on the horizontal `axis` while the `skewY` value distorts an element on the vertical `axis`. To distort an element on both axes the `skew` value is used, declaring the x `axis` value first, followed by a comma, and then the `y axis` value.*
```
.box-1 {
  transform: skewX(5deg);
}
.box-2 {
  transform: skewY(-20deg);
}
.box-3 {
  transform: skew(5deg, -20deg);
}
```
![img](https://cdn.educba.com/academy/wp-content/uploads/2020/06/CSS-skew.jpg)
### Transform Origin
*As previously mentioned, the default `transform` origin is the dead center of an element, both 50% horizontally and 50% vertically. To change this default origin position the `transform-origin` property may be used.*
```
.box-1 {
  transform: rotate(15deg);
  transform-origin: 0 0;
}
```
![img](https://i7x7p5b7.stackpathcdn.com/codrops/wp-content/uploads/2014/12/transform-origin-examples.png)
### Perspective
*The `perspective` of an element can be set in two different ways. One way includes using the `perspective` value within the `transform` property on individual elements, while the other includes using the `perspective` property on the parent element residing over child elements being transformed.*

```
.box {
  transform: perspective(200px) rotateX(45deg);
}
```
![img](https://www.includehelp.com/code-snippets/Images/perspective-of-an-element-in-css.jpg)
### 3D Transforms

- **3D Rotate**
*So far we’ve discussed how to rotate an object either clockwise or counterclockwise on a flat plane. With three-dimensional transforms we can rotate an element around any axes. To do so, we use three new transform values, including `rotateX`, `rotateY`, and `rotateZ`.*
```
.box-1 {
  transform: perspective(200px) rotateX(45deg);
}
```
![img](https://www.tutorialrepublic.com/lib/images/css3-3d-rotation-illustration.png)
- **3D Scale**
*By using the scaleZ three-dimensional transform elements may be scaled on the z axis. This isn’t extremely exciting when no other three-dimensional transforms are in place, as there is nothing in particular to scale. In the demonstration below the elements are being scaled up and down on the z axis, however the rotateX value is added in order to see the behavior of the scaleZ value. When removing the rotateX in this case, the elements will appear to be unchanged.*
```
.box-1 {
  transform: perspective(200px) scaleZ(1.75) rotateX(45deg);
}
```
![img](https://i2.wp.com/cdn-images-1.medium.com/max/1600/1*9b-zGEjNmyi1fAuwsbX7Zg.png?ssl=1)
### Transform Style 
*On occasion three-dimensional transforms will be applied on an element that is nested within a parent element which is also being transformed. In this event, the nested, transformed elements will not appear in their own three-dimensional space. To allow nested elements to transform in their own three-dimensional plane use the transform-style property with the preserve-3d value.*
```
.three-d {
  transform-style: preserve-3d;
}
```
![img](https://miro.medium.com/max/1102/1*AX-ojZx301J9_BU4lan5WQ.gif)
### Backface Visibility
*When working with three-dimensional transforms, elements will occasionally be transformed in a way that causes them to face away from the screen. This may be caused by setting the rotateY(180deg) value for example. By default these elements are shown from the back. So if you prefer not to see these elements at all, set the backface-visibility property to hidden, and you will hide the element whenever it is facing away from the screen.*
```
.box-2 {
  backface-visibility: hidden;
  transform: rotateY(180deg);
}
```
![img](https://i2.wp.com/css-tricks.com/wp-content/uploads/2019/07/animations.gif?fit=900%2C450&ssl=1)
# Transitions
![img](https://res.cloudinary.com/practicaldev/image/fetch/s--OKcvSx-w--/c_imagga_scale,f_auto,fl_progressive,h_420,q_66,w_1000/https://thepracticaldev.s3.amazonaws.com/i/9sjvqruqixbvsg3mon9y.gif)
*As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.*
**Animations**
*Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.*
`transition-property: background, border-radius;`
`transition-duration: .2s, 1s;`
`transition-timing-function: linear, ease-in;`
`transition-delay: 0s, 1s;`
`animation-iteration-count: infinite;`
`animation-direction: alternate;`
`animation-fill-mode: forwards;`
`animation: slide 2s ease-in-out .5s infinite alternate;`
![img](https://codemyui.com/wp-content/uploads/2016/09/a-set-of-animated-css-spinners.gif)
### @-webkit-keyframes

```
@-webkit-keyframes bouncing {
  40%, 70%, 90% {
    bottom: 0;
    -webkit-animation-timing-function: ease-out;
  }
  0% {
    bottom: 200px;
    left: 0;
    -webkit-animation-timing-function: ease-in;
  }
  55% {
    bottom: 50px;
    -webkit-animation-timing-function: ease-in;
  }
  80% {
    bottom: 25px;
    -webkit-animation-timing-function: ease-in;
  }
  95% {
    bottom: 10px;
    -webkit-animation-timing-function: ease-out;
  }
  100% {
    left: 110px;
    bottom: 0;
    -webkit-animation-timing-function: ease-out;
  }
```
![img](https://cdn.dribbble.com/users/97870/screenshots/2071726/pause-push-2.gif)
