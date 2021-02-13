
# JavaScript HTML DOM

### When a web page is loaded, the browser creates a Document Object Model of the page.
> **The HTML DOM model is constructed as a tree of Objects:**
![image](https://i.stack.imgur.com/JatOa.png)

### Objects are grouped together in a set of variables and functions to create a model of somthing.

# Creating objects

## Literal  notation:
> **This is the easiest and most popular way of creating objects**

```
let rental = {
    // properties
    name: 'azooz',
    price: '400$',
    months: '4',

    // method
    payment: function(){
        return this.months * this.price;
    }
}
```

### Accessing an object
> **Using the dot notation we can access any thing inside of an object** 
```
let rentalName = rental.name;
let rentalPayment = rental.payment();
```


## Constructor notation 
> **The *new* keyword and the *object()* constructor creats a blank object, then we add parameters and methods.**

```
let rental = new object();
rental.name = 'azooz';
rental.price = '400$';
rental.months = '10';
rental.payment = function (){
    return this.months * this.price;
};
```

## Updating objects
> **We use the *dot* or *[]* to update value of properties, but to delete properties we use *delete* keyword**
`rental.name ='anan';`
`rental['name'] = 'anan';`
`delete rental.months;`

## The "this" keyword
> **It's commonly used inside functions and objects.**
> **It always refers to *one* object, usually the object in which the function operates.**
`this.name;`

## Arrays of objects & objects in arrays
> **To create a complex data structurs we can compine arrays and objects.**
> *As arrays can stor series of objects, objects hold arrays too.*

### Arrays in objects
```
rental.items = ['chair', 'table', 'closet', 'carpets', 'plates'];
```
`
rental.items[0];
`
### objects in array 
`rental[5].name;`

# Built-in objects
> **Such as String, Number, Math, and Date.**
> **Their properties and methods offer functionality that help you write scripts.**

## Browser object model
> **It contains objects that represent the current browser window or tab.**
> **It contains objects that model things like *browser history* and the *device's screen*.**
`window.innerHeight`
`window.innerWidth`
`window.pageXOffset`
`window.pageYOffset` 
`window.screenX`
`window.screenY`
`window.location`
`window.document`
`window.history`
`window.history.length`
`window.screen`
`window.screen.width`
`window.screen.height`
`window.alert()`
`window.open()`
`window.print()`
![Browser object model](https://static.javatpoint.com/images/javascript/bom.jpg)


## Document object model
> **It uses objects to create a representation of the current page.**
> **It creates a new object for each element within the page.**
`document.title`
`document.lastModified`
`document.URL`
`document.domain`
`document.write()`
`document.getElementByld()`
`document.querySe1ectorA11()`
`document.createElement()`
`document.createTextNode()`
![Document object model](https://www.w3schools.com/js/pic_htmltree.gif)

## Global JS objects
> **It represents things that the JS needs to create a model of.**
![Global JS objects](https://res.cloudinary.com/practicaldev/image/fetch/s--jRLu_Z5j--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/q6pyi9z2qpt9iai9foqx.png)
### String objects
`length`
`toUpperCase()`
`tolowerCase()`
`charAt()`
`indexOf()`
`lastlndexOf()`
`substring()`
`split()`
`trim()`
`replace()`
### Numarical objects
`isNaN()`
`toFixed()`
`toPrecision()`
`toExponential()`
### Math objects 
`Math.PI`
`Math.round()`
`Math.sqrt(n)`
`Math.ceil()`
`Math.floor()`
`Math.random()`
### Date and Time objects
`getDate()`
`setDate()`
`getDay()`
`getFullYear()`
`setFullYear()`
`getHours()`
`setHours()`
`getMilliseconds()`
`setMilliseconds()`
`getMinutes()`
`setMinutes()`
`getMonth()`
`setMonth()`
`getSeconds()`
`setSeconds()`
`getTime()`
`setTime()` *00:00:00 UTC*
`getTimezoneOffset()`
`toDateString()`
`toTimeString()`
`toString()`
