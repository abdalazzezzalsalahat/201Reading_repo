# Lists 

### Ordered lists 
**It's where each item in the list is numbered.**
```
<ol>
    <li></li>
    <li></li>
    <li></li>
</ol>

```
### Unordered lists 
**It's where each item begin with a bullet point**
```
<ul>
    <li></li>
    <li></li>
    <li></li>
</ul>

```
### Definition lists 
**Its made up of a set of terms with its definitions for each of those terms.**
```
<dl>
    <dt></dt>
    <dd></dd>
    <dt></dt>
    <dd></dd>
</dl>
```
## Lists can be nested inside one another.
```
<ul>
    <li>
        <ol>
            <li></li>
            <li></li>
            <li></li>
        </ol>
    </li>
    <li>
        <ul>
            <li></li>
            <li></li>
            <li></li>
        </ul>
    </li>
    <li></li>
</ul>
```
# Boxes
**properties we can manipulate from boxes**
1. *Controling the dimensions of boxes.*
2. *Creating borders around boxes.*
3. *Show and hide boxes.*
4. *margins and padding for boxes.*
- `width`
- `height`
- `min-width`, `max-width`
- `min-height`, `max-hieght`
- `overflow: scroll;`
- `border-width: top, left, bottom, right;`
- `border-style: dotted;`
- `border-color: #l11111;`
- `border: width style color;`
- `padding: 1px;`
- `margin: 1px;`
- `text-align: center;`
- `display: inline-block;`
- `visibility: hidden;`
- `border-image: url() 11 11 11 11 round;`
- `box-shadow: 2px 2px 2px 5px #ffffff;`
- `border-radius: 5px;`
> ### We can control a box how ever we want, make design you want and have fun.
# Arrays
![arrays](http://4.bp.blogspot.com/-OB-Cnc7tUUg/VkSpsp1UsXI/AAAAAAAAJ4Y/zm2EzPX-i8E/s1600/Array%2BIndex.jpg)
> **A special type of variables that can store more than one value of related information.**
```
let arr= ['jordan', 'canada', 'UAE', 'japan'];
```
**The data stored in the array don't have to be the same data-type**
**the values inside an array are accessed only if they are numberd (marked with a specified number)**

to access a value in array using the loops or:
`arr[2] = 'KSA';`
# Decisions
> Conditional statements allow your code to make decisions about what to do next.
## Conditionals
![Comparison-operators](https://www.miltonmarketing.com/wp-content/uploads/2018/04/javascriptcomparisonoperatorsimage041.jpg)
> ### 1. the if family
```
if (true){
    //do somthing
}else {
    false;
}


if (condition 1){
    //do somthing
}else if (condition 2){
    //do somthing else
}
else {
    false;
}
```
> ### 2. The switch
**Used to compare a value with possible outcomes**
```
switch (switch-value){
    case 1:
        //do somthing;
        break;
    case 2:
        //do somthing;
        break;
    case 3:
        //do somthing;
        break;
    case 4:
        //do somthing;
        break;
    default:
        //do somthing;
        break;
}
```
## Truthy Values 
![truthyValues](https://xavierchow.github.io/images/js-coercion-table.png)
> All values evaluate to either *true* or *false*.
# Loops 
![loops](https://excelmate.files.wordpress.com/2014/09/shutterstock_173122277.jpg)
> they **_check repeatedly_** a condition if _true_ a **code block** will run.
### for 
```
for(var x = 0; x < 10; x++){
    //do something
}
```
### while
```
var x = 0;
while(x < 10){
    //do something
    x++;
}
```
### do while
```
var x = 0;
do{
    //do something
    x++;
}while(x < 10);
```

> ## loops are the best when dealing with arrays, but the performance is not ideal