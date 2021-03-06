# Quiz #2

## Instructions

1. Fork this repo
2. Clone your fork
3. Fill in your answers by writing in the appropriate area, or placing an 'x' in
the square brackets (for multiple-choice questions).
4. Add/Commit/Push your changes to Github.
5. Open a pull request.

## JavaScript

### Question #1

**What of the following are JavaScript Data Types?**

Select all that apply:
```
[x] String
[x] Boolean
[x] Undefined
[] NaN
[x] Number
[x] Array
[x] Null
```

## Question #2

Explain what is a REPL, and why is it important for us as developers and help with debugging?

```text
I don't remember talking about REPL
```
### Question #3

**Given the Following Array**

var foods = [ ["apple","banana","strawberry"], ["pizza","fries","hamburger"] ];

Create a For Loop that outputs the following string for each piece of fruit in the console. "I want to eat a [fruit]"

```js
// write code here
for (i=0; i <= food.length; i++){
  for (m=0; m <= food[i].length; m++){
    console.log("I want to eat a" + food[i][m]);
  }
}
```
### Question #4

**Given the Following Array**

var foods = [ ["apple","banana","strawberry"], ["pizza","fries","hamburger"] ];

How would I go about accessing the string "pizza" in the above array?

```js
// write code here
food[1][0];
```

## Scope/Context/Closures

### Question #5

Describe the rules of scope in JavaScript.

Your Answer:
```text
the rules of scope relate to the areas in code which have access to certain variables or functions based on where they are defined and how they are defined.For example, function
declarations can be hoisted, whereas function expressions cannot. new variables declared
within functions can only be used in that function (unless they are defined without
using 'var variableName', but this is not best practice). Global functions should be
used only when needed since they slow down processing of the code.

```

### Question #6

Define an object and store it in a variable `pizza`. The object should have 2
properties: a temperature (set to 70), and a method called `bake`. When called,
this method should set the pizza's temperature to be 300. Note: you may not use
the variable pizza inside your method.

Your Answer:
```js
// write code here
var pizza= {
  temperature: 70,
  bake: function(){
    temperature = 300;
    return temperature;
  }
}
```

### Question #7

Using a 'for' loop, iterate over an array of numbers in JavaScript, printing each to the console.

Your Answer:
```js
// write code here
var numbers = [1,2,3,4,5,6]
for (i=0; i <= numbers.length; i++){
  console.log(numbers[i]);
}
```

### Question #8

Write the vanilla JS equivalent of the following jQuery code:

```js
$("button").on("click", function(event){
  $(event.target).css('color', 'red')
})

```

Your Answer:
```js
// write code here
document.querySelector("button").addEventListener("click", function(event){
  querySelector(event.target).style("color", "red")
})
```

## Objects and Functions

### Question #9

What are the differences between calling and referencing a function? Please provide examples of each.

```text
calling a function is executing it.
  eg: "function();"
referencing a function is when you want a function to execute when a piece of code executes.
  eg: "$("button").on("click," function);" - function here is being referenced
```
### Question #10

Using the object literal notation, Define an object called student and give it the properties (your attributes) of name, age, and a method sayHello, that outputs "Hi, my name is [your_name]".

Your Answer:
```js
// write code here
var student = {
  name: Julia,
  age: 23;
  sayhello: function(){
    console.log("Hi, my name is " + name);
  }
}
```

## Callbacks

### Question #11

**What is the difference between synchronous and asynchronous program execution?**

Select all that apply:
```
[] Synchronous code runs at an even pace, asynchronous code runs with uneven pacing.
[] Synchronous code runs all at the same time, asynchronous code runs completely randomly
[x] Synchronous code runs in order (as appears in the source), asynchronous code may run at a later time.
```
