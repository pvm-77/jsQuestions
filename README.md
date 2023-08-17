## Variable Declarations(let,const)
1. what is the difference between `let` and const in js?
2. How does let differ from `var` in term of block scope?
3. why is using  `const` recommended for variables that wont change their value?
4. can you reassign a value to a variable declared with `const`?
5. what happens if you try to declare a variable with the same name using `let` within the same scope?
6. how does the `temporal dead zone` relate to `let ` and  `const` declarations?

## scope and closure
7. explain what `scope` means in js?
8. how does js handle variable scope in comparison to other programming languages?
9. describe the difference between `global scope` and `local(function) scope`?
10. can u access variables defined in a higher scope from lower scope?
11. explain what a closure is and why its useful?
12. how does a closure retain access to its outer function's variables even after the outer function has finished executing?

## Block scope and Hoisting
13. how does `let` differ from `var` regarding hoisting?




14. in which cases will a variable declared with `var` be function-scoped rather than block-scoped?
15. whats the significance of the`TDZ` with regard to block-scoped ?
16. how do block scoped variables declared with `let` behave within loops and conditional statements?


## Closure
17. provide an example of a closure in js?
18. how can u create closure intentionally?
19. explain how closure can lead memory leaks if not handled properly?
20. how can u use closure to create private varibles and encapsulation?
21. whats the differnce between a closure and a function that returns a function?

## practice with closure?

22. write a function that increaments a counter each time its called?
23. create a function that generates a sequence of unique IDs?
24. build a simple module pattern using closures to create private methods and variables
NOTE:important apllication of closure is module pattern
## Advanced Closure Concepts:

25. What is the "module pattern," and how does it relate to closures?
26. Describe the "IIFE" (Immediately Invoked Function Expression) pattern and its purpose.
    
27. Explain the "this" context within a closure and how it can change based on how the closure is invoked.


## Practical Applications:

How can closures be useful in handling asynchronous operations, like callbacks?

Describe how closures are employed in event handling, such as with addEventListener.

Explain how closures can assist in creating iterators and generators.


## Garbage Collection and Memory:

Does a closure prevent its outer function's variables from being garbage-collected?

How can you release memory associated with a closure?

Explain the concept of "circular references" and how they might relate to closures.


## Debugging and Best Practices:

What challenges might closures pose when debugging code?

How can you avoid unintended closures or memory leaks in your code?

What's the best practice for naming variables that are part of a closure to avoid naming conflicts?

## Arrow Functions and Closures:

How do arrow functions handle the "this" context compared to regular functions?

What's the difference between the way arrow functions and regular functions handle closures?



## Common Interview Questions:

Can you explain the concept of hoisting and how it applies to variables and functions?

Describe the difference between a function declaration and a function expression in terms of hoisting.

How would you create a private variable in JavaScript?

Explain how you can avoid the "callback hell" problem using closures and named functions.


## Testing Your Knowledge:

Write a function that uses closure to create a countdown timer.
Implement a function that checks if a number is prime using closures.
Create a simple counter using the module pattern to demonstrate closures.
Miscellaneous:

Can closures only be created with functions, or are there other ways?

What's the relationship between lexical scoping and closures?

Explain how closures can help manage state in functional programming.

How does the use of closures affect the performance of your code?





## Basic Multiple-Choice Questions:

1. In JavaScript, what is the scope of a variable declared with var?

    a) Global scope
  
    b) Function scope
  
    c) Block scope
  
    d) Module scope
  

2. What happens if you declare a variable with var inside a block statement (e.g., if, for, while)?

    a) The variable has block scope.
    
    
    b) The variable has function scope.
    
    
    c) The variable has global scope.
    
    
    d) The variable is not affected by the block statement.



3. What is the behavior of hoisting for variables declared with var?

    a) Variables are hoisted and can be accessed anywhere within the function or global scope.
    
    
    b) Variables are hoisted only within the block where they are declared.
    
    
    c) Variables are not hoisted, and referencing them before declaration results in an error.
    
    
    d) Variables are hoisted, but they retain their value at the time of declaration.



4. In a function, if a variable is declared with var inside the function and is not explicitly returned, what is the scope of that variable?

    a) Global scope
    
    
    b) Function scope
    
    
    c) Module scope
    
    
    d) Block scope



5. When using var to declare a variable with the same name inside a function and in the global scope, what happens?

    a) The variable inside the function shadows the global variable.
    
    b) An error is thrown because the variable name is already used in the global scope.
    
    c) Both variables coexist, and the function will use the local variable first.
    
    d) The global variable gets reassigned with the value of the local variable.


6. In JavaScript, what is the behavior of re-declaring a variable with var within the same scope?

    a) The variable is re-initialized to its original value.
    
    b) A new variable is created with the same name, shadowing the original variable.
    
    c) An error is thrown because you cannot re-declare a variable with var.
    
    d) The new declaration has no effect; it continues to reference the original variable.

7. What happens if a variable is declared inside a function and also declared with var in the global scope?

    a) Both variables are accessible globally but hold different values.
    
    b) An error is thrown because you cannot have the same variable name declared multiple times.
    
    c) The global declaration is ignored, and the variable inside the function is used.
    
    d) The global declaration overrides the local declaration inside the function.

8. What is the value of y after the following code is executed?
  ```js
  var x = 5;
  function foo() {
    var x = 10;
  }
  foo();
  var y = x;
  ```
    a) 5
    
    b) 10
    
    c) undefined
    
    d) ReferenceError

9. What is the output of the following code?
  ```js# JS-Questions
  console.log(x);
  var x = 10;
  
  ```
    a) ReferenceError: x is not defined
    
    b) undefined
    
    c) null
    
    d) 10

10. What will the code output?
  ```js
  var x = 5;
  if (true) {
    var x = 10;
  }
  console.log(x);
  
  ```
    a) 5
    b) 10
    c) undefined
    d) ReferenceError


## Predict the output type questions?

  1. 
    ```js  const pi=3.14
      console.log(pi)
      pi=3;
    function foo() {
      console.log(x);
      var x = 5;
    }
    foo();
    
    ```
  
  2. 
    ```js
    
    for (var i = 0; i < 3; i++) {
      setTimeout(function () {
        console.log(i);
      }, 100);
    }
    
    ```

  3.
    ```js
    var x = 10;
    if (true) {
      var x = 20;
    }
    console.log(x);
    ```

  4.
    ```js
    
    var x = 5;
    function foo() {
      console.log(x);
      var x = 10;
    }
    foo();
    
    ```

  5.
    ```js
    var x = 5;
    function foo() {
      console.log(x);
    }
    foo();
    
    ```
  
  6.
    ```js
    
    var x = 1;
    if (true) {
      var x = 2;
      console.log(x);
    }
    console.log(x);
  
    ```

  7.
    ```js
    
    var x = 10;
    function foo() {
      console.log(x);
    }
    foo();
    
    ```

  8.
    ```js
    var x = 5;
    if (true) {
      var x = 10;
      console.log(x);
    }
    console.log(x);
    
    ```
  
  9.
    ```js
    for (var i = 0; i < 5; i++) {
      setTimeout(function () {
        console.log(i);
      }, 100);
    }
    
    ```
  
  10. 
    ```js# JS-Questions
    function foo() {
      var x = 5;
    }
    foo();
    console.log(x);
    
    ```


## ADVANCE Theory questions

1. What is the temporal dead zone in relation to let?

2. How does let differ from var in terms of hoisting and scope?

3. Explain how let variables are affected by closures in JavaScript.

4. Compare and contrast the behavior of let and const when used in loops and conditional statements.

5. What are the best practices for using let in modern JavaScript development?

6. How does the usage of let impact garbage collection and memory management in JavaScript?

7. Describe the lexical scoping rules that apply to let variables in arrow functions.

8. Explain the behavior of let when used inside async functions and how it handles asyn# Node.js template



# * * * Md Mohib Khan * * *

## Group-A (Write output:)

### 1) 
  ```
  const pi=3.14
  console.log(pi)
  pi=3;

  ```

# Aasif Iqbal
## (Guess the output)
01. var 
```
var fruit = 'apple'
{
  var fruit = 'orange'
  console.log(fruit) // ??
}

console.log(fruit) // ??
```
02. var
```
var fruit = 'apple'

function gimmeFruit() {
  var fruit = 'orange'
  console.log(fruit) // ??
}

console.log(fruit) // ??
gimmeFruit()
```
03. let
```
let fruit = 'apple'

{
  let fruit = 'orange'
  console.log(fruit) // ??
}

console.log(fruit) // ??
```
04. let
```
function foo(n) {
    if (n == 6) {
        let num = 2;
    }
    console.log(num);
}

var n = 6;
console.log(n);
foo(6);
```
05. let
```
for(var i=0;i<3;i++){
  console.log(i)
}
console.log("i outside the loop: ", i);

for(let j=0;j<3;j++){
  console.log(j);
}

console.log("j oustide the loop :", j);
```
06. const
```
{
  const fruit = 'apple'
  fruit = 'orange'
  console.log(fruit)
}
```
07. const
```
if (true) const a = 1;
```
08. const
```
const MY_FAV = 7;

if (MY_FAV === 7) {
   
  const MY_FAV = 20;
  console.log(MY_FAV);  
  
  var MY_FAV = 20;  
}

console.log(MY_FAV); 
```
09. let and var
```
{  
  console.log(bar);  
  console.log(foo);  
  var bar = 1;
  let foo = 2;  
}
hint:TDZ
```
10. let and var
```
{

  const func = () => console.log(letVar);

  let letVar = 3; 
  func(); 
}

```
11. let and var
```
function test() {
  var foo = 33;
  if (foo) {
    let foo = foo + 55; 
  }
}
test();

```
12. let and var
```
function go(n) {
  
  console.log(n); 

  for (let n of n.a) {
  
    console.log(n);
  }
}

go({ a: [1, 2, 3] });

```
13. let and var
```
let x = 1;

{
  var x = 2; 
}

```
14. var
```
"use strict";
var x = 1;
Object.hasOwn(globalThis, "x"); // ??
delete globalThis.x; // ??
delete x; // ??

```
15. var
```
try {
  throw 1;
} catch (e) {
  var e = 2; 
}
console.log(e); // ??

```
16. var
```
"use strict";

var x = 0;
function f() {
  var x = y = 1;
}
f();

console.log(x, y);

```
17. var
```
function foo(a) {
  var a = 1;
  console.log(a);
}

foo(2); 
 ```     




