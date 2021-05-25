# JavaScript

- [Overview](#Overview)
- [Data Types](#Data-Types)
- [Variables](#Variables)
- [var,let and const](#var,-let-and-const)
- [Function](#Function)
- [Function Declaration And Function Assignment](#Function-Declaration-And-Function-Assignment)
- [Scope Of Function](#Scope-Of-Function)
- [Passing Primitive Parameter To Function](#Passing-Primitive-Parameter-To-Function)
- [Passing Non-Primitive Parameter To Function](#Passing-Non-Primitive-Parameter-To-Function)
- [Function Returning A Function](#Function-Returning-A-Function)
- [Function Passing As Parameter To Another Function](#Function-Passing-As-Parameter-To-Another-Function)
- [Immediately Invoked Function Expression(IIFE)](#Immediately-Invoked-Function-Expression(IIFE))
- [Higher Order Function](#Higher-Order-Function)
- [Pure Function](#Pure-Function)
- [Arrow Function](#Arrow-Function)
- [Objects](#Objects)
- [Prototype Method Of Arrays](#Prototype-Method-Of-Arrays)
- [Prototype Method Of String](#Prototype-Method-Of-String)
- [setTimeout And setInterval Function](#setTimeout-And-setInterval-Function)
- [JSON](#JSON)
- [Spread Operator And Destructuring Feature Of ES6](#Spread-Operator-And-Destructuring-Feature-Of-ES6)

---

## Overview

JavaScript programming language was developed by Brendan Eich in 1995. When JavaScript was created it was known as LiveScript. Netscape changed its name to JavaScript. JavaScript is a high-level, dynamic, lightweight, interpreted computer programming language. It’s designed for creating network-centric apps. JavaScript is a dynamic type language, which means that you don't need to define type of the variable because it is effectively used by the JavaScript engine.
ECMAScript is a standardized version of JavaScript with the goal of unifying the language's specifications and features. As all major browsers and JavaScript-runtimes follow this specification, the term ECMAScript is interchangeable with the term JavaScript.

## Data Types

JavaScript is a dynamic type language, which means that you don't need to define type of the variable because it is effectively used by the JavaScript engine. There are two types of data in JavaScript: primitive data type and non-primitive (reference) data type.

**Primitive Data Types**:
- Number - Stores integer and floating point numbers.  
```JavaScript
    var num=15;
```
- String - Stores text. In JavaScript, strings can’t be changed, and they must be inside of either double or single quotes.  
```JavaScript
    var firstName="Dipankar"; 
    var lastName='Chakraborty';
```
- Boolean - Stores true or false
```JavaScript
    var val=true;
```
- Null - Treated as falsy for boolean operations. In JavaScript null means nothing or empty. It’s something that doesn't exist. But in JavaScript, the data type of null is an object, which you can empty by setting an object to null.
```JavaScript
    var num=null;
```
- Undefined - A variable without a value is called undefined. It’s value and type are undefined, which means that the “value is not assigned”
```JavaScript
    var x;
```
 Symbol - new datatype introduced in ES6, a symbol value represents an unique identifier.
 
 **Non-Primitive Data Types**
 - Arrays - Stores several piece of data in one place
 ```JavaScript
    var sandwich = ["peanut butter", "jelly", "bread"]
 ```
 - Objects - It’s a collection of properties, which can reference any type of data, including objects and/or primitive values.
  ```JavaScript
      var cat = {
      "name": "Tom",
      "eyes": 2,
      "eyeColor": "brown"
      };
 ```
 

## Variables
JavaScript variables are containers for storing data values.
A variable in JavaScript contains any of these data types: number, string, objects.
There are 3 ways to declare variables: **var, let and const**.
```JavaScript
var rollNo = 12;                   // Number
const name= "Dipankar";              // String
let dog = {name:"Bruno", legs:4};  // Object
```

## var,let and const

|Sr No.| var                    | let    |   const  |
|----  | -----------------------| ------ |-------|
|1.   | It was introduced in ES5 |It was introduced in ES6     |  It was introduced in ES6    |
|2.   | It can be redeclared        |  It can't be redeclared    |It can't be redeclared       |
|3.   | It can be reinitialized | It cannot be reinitialized |  It cannot be reinitialized    |
|4.   |  It has functional scope| It has lexical scope |   It has lexical scope   |
|5.   |It get's hoisted|It doesn't get hoisted| It doesn't get hoisted |

- **Variable declaration by using var**
`````JavaScript
var x = 10;
console.log("1", x);  //10
x = 20;
function fun() {
x = 30;                      //only functional scope
console.log("2", x);           //30
var x;                          //gets hoisted on top of the function
}
console.log("3", x);  //30
fun();
``````

- **Variable declaration by using let**
``````JavaScript
let x = 10;
console.log("1", x);  //10
x = 20;
function fun() {
x = 30;                      //only functional scope
console.log("2", x);           //30
let x;                          //error value not assigned
}
console.log("3", x);  //20
fun();
``````

- **Variable declaration by using const**
````````JavaScript
const x = 10;
console.log("1", x);  //10
x = 20; //error invalid assignment to const
function fun() {
const x = 30;                      //only functional scope
console.log("2", x);           //30
const x;                          //error as value is not assigned
}
console.log("3", x);  //10
fun();
`````````

## Function

In JavaScript, we can divide up our code into reusable parts called functions.
```JavaScript
  function fun{
  console.log("Hello World");
  }
  fun();
```

## Function Declaration And Function Assignment
**Function Declaration**
- Function gets hoisted
- Function can be overriden
```JavaScript
  function fun{
  console.log("Hello World");
  }
  fun();
```
**Function Assignment**
- Function is declared without name it's just assigned as a variable
- The function doesn't get hoisted
```JavaScript
var func = function() {
   alert(‘This is anonymous');
}
func();
```

## Scope Of Function

In JavaScript, scope refers to the visibility of variables. Variables which are defined outside of a function block have Global scope. This means, they can be seen everywhere in our JavaScript code.Variables which are defined within a function block have local scope.

```JavaScript
let name='Dipankar'; //global scope
  function fun{
  let val='Hello' + name; //local scope
  console.log(val);
  }
  fun();
```

## Passing Primitive Parameter To Function

```JavaScript
function testFun(param1, param2) {
  console.log(param1, param2);
}
testFun(5,6);
```

## Passing Non-Primitive Parameter To Function
```Javascript
function fun(obj) {
  obj.make = 'Renault';
}
var car = {make: 'Fiat', model: 'Punto', year: 2018};
var x, y;
x = car.make; // x gets the value "Fiat"
fun(car);
y = car.make; // y gets the value "Renault"
```

## Function Returning A Function
```Javascript
function factorial(n) {
  if ((n === 0) || (n === 1))
    return 1;
  else
    return (n * factorial(n - 1));
```

## Function Passing As Parameter To Another Function

```Javascript
function map(f, a) {
  let result = []; // Create a new Array
  let i; // Declare variable
  for (i = 0; i <= a.length; i++)
    result[i] = f(a[i]);
  return result;
}
```

## Immediately Invoked Function Expression(IIFE)

Immediately Invoked Function Expression(IIFE) is a function that runs as soon as it is defined.
```JavaScript
(function () {
  let x;
  let y;
})();     // x and y will be discarded after the function is executed.
```

## Higher Order Function

A higher-order function can be defined as a function that accepts one or more functions as arguments and returns a function as a result.
```JavaScript
const numbers = [1, 2, 3, 4, 5];
const newArray = numbers.map((number) => number + 1);
console.log(numbers);
```

## Pure Function
Pure Function is a function that always returns the same result if the same arguments are passed.
```JavaScript
function calculateBankInterest( totalBalance ) {
    return totalBalance * 0.05;
}
```

## Arrow Function
Arrow functions allow us to write shorter function syntax. It was introduced in ES6. It doesn't get hoisted.
```JavaScript
let multiply = (a, b) => a * b;
console.log(multiply(7, 9));
```

## Objects
Objects are a collection of properties, which can reference any type of data, including objects and/or primitive values.
  ```JavaScript
      var smartphone = {
      "name": "SamsungM1",
      "cameras": 2,
      "color": "blue"
      };
 ```
 
## Prototype Method Of Arrays

- **fill** - Fills the array with given value from start to end index
- **reverse** - Reverses the array
- **push** - Adds the given elements at end of the array
- **pop** - Removes last element from array
- **shift** - Removes first element from array
- **unshift** - Adds the given elements at start of the array
- **map** - Returns a new array of equal length that contains transformed elements
- **forEach** - Iterates an array and calls the given function

## Prototype Method Of String

- **toUpperCase** - Converts string to uppercase
- **toLowerCase** - Converts string to lowercase
- **split** - Divides the string into substrings
- **replace** - Replaces the existing string
- **toString** - Converts to string

## setTimeout And setInterval Function
setTimeout - allows us to run a function once after the interval of time.
setInterval - allows us to run a function repeatedly, starting after the interval of time, then repeating continuously at that interval.
```JavaScript
// repeat with the interval of 2 seconds
let timerId = setInterval(() => alert('tick'), 2000);
// after 5 seconds stop
setTimeout(() => { clearInterval(timerId); alert('stop'); }, 5000);
```
## JSON

JavaScript Object Notation (JSON) is a standard text-based format for representing structured data based on JavaScript object syntax. It is commonly used for transmitting data in web applications (e.g., sending some data from the server to the client, so it can be displayed on a web page, or vice versa).

```JavaScript
{
   "book": [
      {
         "id":"01",
         "language": "Java",
         "edition": "9th",
         "author": "Herbert Schildt"
      },
      {
         "id":"02",
         "language": "C",
         "edition": "3rd",
         "author": "E.Balagurusamy"
      }
   ]
}
```
The **JSON.stringify()** method converts a JavaScript object or value to a JSON string, optionally replacing values if a replacer function is specified or optionally including only the specified properties if a replacer array is specified.
```JavaScript
JSON.stringify(fun, ['week', 'month']);
```

## Spread Operator And Destructuring Feature Of ES6

**Spread Operator** allows an iterable such as an array expression or string to be expanded in places where zero or more arguments (for function calls) or elements (for array literals) are expected, or an object expression to be expanded in places where zero or more key-value pairs (for object literals) are expected.
```JavaScript
function myFunction(x, y, z) { }
let args = [0, 1, 2];
myFunction(...args);
```
ES6 provides a new feature called **destructing assignment** that allows you to destructure properties of an object or elements of an array into individual variables.
```JavaScript
function getPrices() {
   return [170, 380, 900];
}
let [x, y, z] = getPrices();
console.log(x); // 170
console.log(y); // 380
console.log(z); // 900
```
---
