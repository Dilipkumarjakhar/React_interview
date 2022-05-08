

![LCO Mascot](https://learncodeonline.in/mascot.png)
## What is javaScript.? ##
 Javascript is used by programmers across the 
 **world to create dynamic and interactive 
 web content like applications and browsers.** 
 JavaScript is so popular that it's the most 
 used programming language in the world, used 
 as a **client-side programming language by 97.0% of all websites.**


## What is node.js ##
**Node.js is an open-source, cross-platform**, back-end JavaScript runtime environment that runs on the V8 engine 
and executes JavaScript code outside a web browser.**

## What is express JS used for? ##
**Express. js is a free and open-source web 
application framework for Node. js.** 
It is used for designing and building web 
applications and API 's quickly and easily.
-  It has been called the de facto standard server framework 
   for Node.js
- **Initial release:** 16 November 2010; 11 years ago

**1.Anonymous Function**
- A function without name it is called Anonymous function.
```
function (){
}
```
**2.Function Statment and function Declaration**
- Function statment is nothing but writting the normal function.
- Function Statment and function Declaration both are same.
```
function a(){
    console.log("a called")
}
a()
o/p:- a called
```
**3.Function Expression**
- In this function we are assigning the function into b variable.
```
var b=function (){
    console.log("b called")
}
b()
o/p:- b called
```
**4.Named Function Expression**
- In this function we are assigning the function into b variable.
```
var b=function xyz(){
    <!-- console.log(xyz) here it will give function or you access -->
    console.log("b called")
}
b()
o/p:- b called
xyz()
o/p:- refrence error
```
**5.Diffrence Between Parameter & Arguments**
- In this function we are assigning the function into b variable.
```
var b=function (para1,para2){
//these lebels and identifiers are getting the values
 is called parameters.
    console.log(para1,para2)
}
b(1,2)
//here we are passing the values inside the function is called Arguments
o/p:- 1 2 

```
**6.First Class Functions or First Class Citizens**
- function inside function .
- we can pass the value as argument and we can use that values as parameters in another function .
- Ability to Used like values.

```
var b=function (){
  return function (){

  }

}
    console.log(b())

o/p:- function (){
}

```
**7.Arrow Functions**
- An Arrow Function is used to write an expression in React.
- It allows users to manually bind components easily.
- The functionality of arrow functions is very useful when you are working with higher-order function particularly.


```
Example:
//the usual way
render(){
    <Myinput onChange={this.handleChange.bind(this)}>
}
//Making use of arrow function 
render(){
    return(
    <Myinput onChange={(e)=>this.handleOnChange(e)}>
    )}
```

```
Normal Example:-
var b=function ()=>{
 console.log("Arrow function")
}
b()
o/p:- Arrow function
```
**8.Closure Functions**
- closer in action that is inner function can have access to the outer function variables as well as all the global variables.
- A closure is the combination of a function and lexical
environment within which that function was declared.

- [the return statment does not execute the inner function - function is execute only when followed by (),
but rather then return statment return the entire body of the function.] 
```
let sum=(a)=>{
    let z=10
    function y(a){
        console.log('dilip',a+z)
        
    }
    y(a)
}
sum(1)

o/p:-->dilip 11

let outer=(a)=>{
    let x=a;
    function inner(y){
        console.log('sum',x+y)
        
    }
    // inner(a)
   return inner
}

outer(1);
let store=outer(1);

store(1)
o/p:->sum 2
```

**9.function Hoisting**
- for each function(function declarations) a property is created in the variable object.which is pointing to function
- for each function(variable declarations) a property is created in the variable object.which is set undefined.
- Argument object are created that were passed into the function.
- lin1 and lin2 is called **Hoisting** in js.
- hoisting is js mechanism where variable and function declaration are moved to the top of there scope before code execution.

``` 
this is normale:
const sum=(a,b)=>{
    let c=10;
    console.log(a+b+c);
}
sum(3,4);
o/p:->17
```

```
- This is Hoisting :--------|>
sum(3,4);              |const sum=(a,b)=>{
const sum=(a,b)=>{     | let c=10;
    let c=10;          |  console.log(a+b+c);
    console.log(a+b+c);|  }
}                      |sum(3,4);
                       |
o/p:->17               |o/p:->17  
```

**10.Use Strict**
- It's a new feature of ECMAScript 5.
- The statment 'use strict'; instructs the browser the browser to use the strict mode which is a reduced and safer feature set of js.
```
normale example
function sum(a,b){
    add=a+b;
    console.log(add)
}
sum(10,12)
o/p:-22;
```
```
strict example:-
'use strict'
function sum(a,b){
    add=a+b;
    console.log(add)
}
sum(10,12)
o/p:-add is undefined
```
**11.Let,var and const** 
- **let and const** is a block scope variable.
```
let a=1;

if(a){
    let x=2;
    console.log('x:', x)
    }
console.log('x:', x)
console.log('a:', a)
o/p:-
x:2
x:undefined;
a:1;
```
- var is a function scope variable.
```
var sum=100;
function d(a,b){
    if(sum>99){
        var sum=a+b;
    }
    console.log(sum);

}
console.log(d(10,20));
o/p:-30
```
**12.This Keyword**
- **“This”** keyword refers to an object that is executing the current piece of code
- console.log(this)//window object 
- It references the object that is executing the current function. 
- If the function being referenced is a regular function, “this” references the global object.
**13.What is this inside function?**
- “this” inside Functions
- The value of this inside a function is usually defined by the **function's call**. 
- this can have **different values inside it for each execution of the function.** 
- In your index. js file, write a very simple function that simply checks if this is equal to the global object.

**14.What is $() in JavaScript?**
- The $() function
- The dollar function, **$()**, can be used as shorthand for the **getElementById function**. 
- To refer to an element in the Document Object Model **(DOM)** of an HTML page, the usual function identifying an element is: document.

**15.What is this in jQuery?**
- this is a reference to the html DOM element that is the **source of the event.** 
- $(this) is a jQuery wrapper around that element that enables usage of jQuery methods. 
- jQuery calls the callback using apply() to bind this.

**13.Promises**
- Promises are used to handle asynchronous operations in javascript.
- They are easy to manage when dealing with multiple asynchronous operations where callbacks can create hell
leading to unmanageable code.

- A Promise is an object that keeps track about whether
a creation event has happened already or not.

```
```

**13.Event Loop**
- javaScript is single synchronous thread langauge.
- It has one CallStack it can do one thing at a time this callstack persent inside javaScript Engine.
- All The js code executed inside callstack.
- WhenEver any Javascript code run that time Global
  Execution context will be created.
- The GEC will be pushed inside callstack.
- Inside GEC code run line by line|    -------   |
                                  |    -------   |
                                  | ----GEC----- | 
                                  |______________|
- (Line no 243 to 245)Function a(){console.log('a')} allocated the memory.
- whenever function invocations(line no 246) happen that time GEC will created.
- This function invocations pushed inside callstack.
- so a() in inside the callstack so the code of a() function will executed line by line.
- when the end of function a() the function a() pops out of the callstack.
```
 __________________
|                  |   function a(){
|   |          |   |     console.log("a);
|   |          |   |     }
|   |          |   |     a();
|   |          |   |     console.log('end)
|   |          |   |
|   |call stack|   |
|   |__________|   |
| js Engine        | 
|__________________|
```
```
 ________________________
|      Browser           |
|   __________________   |
|  |                  |  |
|  |                  |  |  
|  |   |          |   |  |  
|  |   |          |   |  | 
|  |   |          |   |  |
|  |   |call stack|   |  |
|  |   |__________|   |  |
|  |    js Engine     |  |
|  |__________________|  |
|                        |
|________________________|
```

**14. What's the difference between == and === ?**
- The difference between **==(abstract equality)** and **===(strict equality)** is that the == compares by value after coercion and === compares by value and type without coercion.
- Let's dig deeper on the ==. So first let's talk about coercion.

**coercion is the process of converting a value 
to another type. As in this case, the == does 
implicit coercion. The == has some conditions
 to perform before comparing the two values.**

Suppose we have to compare x == y values.

- If x and y have same type. Then compare them with the === operator.
- If x is null and y is undefined then return true.
- If x is undefined and y is null then return true.
- If x is type number and y is type string Then return x == toNumber(y).
- If x is type string and y is type number Then return toNumber(x) == y.
- If x is type boolean Then return toNumber(x) == y.
- If y is type boolean Then return x == toNumber(y).
- If x is either string,symbol or number and y is type object Then return x == toPrimitive(y).
- If x is either object and x is either string,symbol Then return toPrimitive(x) == y.
- Return false.
Note: toPrimitive uses first the valueOf method then the toString method in objects to get the primitive value of that object.

**Let's have examples.**

| x | y	| x == y |
|---|---|--------|
|5	|5	|  ```true``` |
|1	|'1'|	```true```    |
|null	|undefined|	```true```|
|0	|false|	```true```|
|'1,2'	|[1,2]|	```true```|
|'[object Object]'|	{}|	```true```|

These examples all return true.

- The first example goes to condition one because x and y have the same type and value.

- The second example goes to condition four y is converted to a number before comparing.

- The third example goes to condition two.

- The fourth example goes to condition seven because y is boolean.

- The fifth example goes to condition eight. The array is converted to a string using the toString() method which returns 1,2.

- The last example goes to condition ten. The object is converted to a string using the toString() method which returns [object Object].

|x  | y  |x === y|
|---|----|-------|
|5  |	5|	```true```|
|1  |	'1'|	```false```|
|null|	undefined|	```false```|
|0	|false	|```false```|
|'1,2'|	[1,2]|	```false```|
|'[object Object]'|	{}|	```false```|

If we use the === operator all the comparisons 
except for the first example will return false because they don't have the same type while the first example will return true because the two have the same type and value.


**15.What is Difference between object (o) with 
lowercase and Object (O) with upper case.?**
```
function Game(){
this.name=“cricket”;
}
var object=new Game();
console.log(Object);
console.log(object);

output 1-ƒ Object() { [native code] }
output 2- Game {name: “cricket”}`
```
**what is output .???**

- Javascript is case sensitive "object" is essentially a variable that can hold anything. 
- "Object" is an actual javascript Data-type.
- While in your case **object is an instance of the constructor function**, 
  without storing the **reference** of new Game in the variable object, object is nothing in JavaScript.


















**14.Equal(==)**
- It Have **Operate** as well as **Operands**.
- **operater ==,<,>,<=,>=,!**
- operands variables name like let x=10,let y=11 **x and y**;
- It is comparsion operator which is used to check the vlues of the operands
```
Example:-
let x=1;
let y="1";
if(x==y){
    console.log("equal")
}
else{
    console.log("not equal")
}
o/p:-equail
why because both the value are equal (1=="1") the check only values.
```
**15.Equal(===)**
- It Have **Operate** as well as **Operands**.
- **operater ==,<,>,<=,>=,!**
- operands variables name like let x=10,let y=11 **x and y**;
- It is comparsion operator which is used to check the vlue and type of the operands

```
Example:-
let x=1;
let y="1";
if(x===y){
    console.log("equal")
}
else{
    console.log("not equal")
}
o/p:-equail
why because both the values equal but type is number and string (10==11)
```

**16.What is the Output.?** 
- **Null and Undefined.**
```
console.log(null==undefined)
```
- The == comparison operator doesn't check the types. 
- null and undefined both return false. 
- That's why your code is actually checking if false is equal to false.

- > null == undefined;
- > true
- > false == false
- > true
**Output:-true**
```
console.log(null===undefined)
```
- > typeof undefined;
-  "undefined"
- > typeof null;
-  "object"
- Because of that, the next statement will return false, as the === comparison operator checks both the types and their value.
- why true because null has falsy and undefined also falsy.
**Output:-false**
## object ##
```
console.log({}=={})
```
**Output**:-false
- Because both of having different **Address**.

```
console.log({}==={})
```
**Output**:-false
```
console.log({}===[])
```
**Output**:-false

## Array ##
```
console.log([]==[])

```
**Output**:-false

```
console.log([]===[])
```

**Output**:-false
```
console.log([]=={})

```
**Output:-false**



-----------------------------------------------

-----------------------------------------------
## React Interview ##
**7. Must-Know JavaScript Tricks & Tips** 

**1. Use object instead of “switch”**

- We often use switch to handle different things, 
- but have you ever thought of using an object to greatly simplify
- your code?(It works in some simple scenarios)
```
❌
const n = 1
let result
switch (n) {
  case 1:
    result = 'res-1'
    break
  case 2:
    result = 'res-2'
    break
  case 3:
    result = 'res-3'
    break  
  // ...There are a lot more
}
```
**You only need to use an object to achieve your goal.**
```
✅
const n = 1
const nMap = {
  1: 'res-1',
  2: 'res-2',
  3: 'res-3'
}
const result = nMap[ n ]
```
**Strong/Bold**

~~10~~ **999**

Links
[visit website](https://dilipkumarjakhar.netlify.app)


Images

Use `for` loop

---
Dropdown
--
Tables
| S.no | Name | Level | links |
| ---   | ---  | ---   | ---  |
| 1     | Array Reverse    | 3     | [4]("https://dilipkumarjakhar.netlify.app/")    |
| 1     | 2    | 3     | 4    |
| 1     | 2    | 3     | 4    |




