1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
}

let percentage = function(marks, total) {
  return (marks * 100) / total;
}
let percentage = function(marks, total) => {
  return (marks * 100) / total;
}

let percentage = (marks, total) => {
  return (marks * 100) / total;
}

// Your code goes here
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// function declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
// function expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
// function expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
// function expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;
// function expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
Function definition of a function inside variable of an expressionso that how we can use the fucntion expression.
```js
let percentage = (marks, total) => (marks * 100) / total;
// function expression
```
4. Why is a function call an expression in JavaScript?
while calling an function in javascript it will always return any kind of value.
```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
```
5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Valid output will be undefined because code will pass two parameters value.
five = add; // valid
five = five(10, 11); // valid
five = function () {
  return 'Hello';
}; // valid
```

6. What is the difference between function definition and function call? Explain with an example.
function definition can process that function but function call will call the function.
Example:- function add() {} // definition add() // call a function
7. What is the similarities between function definition and function call?
we can use the parameters to execute the code in function definition we can use the parameters with the assign but when we call the function with function call we have to pass any value in the paramter.
8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid 
```

9. What is higher order function explain with an example.
function that takes a function as an argument or return a function.
10. Explain what is callback function. Why you can pass a function inside a function?
function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action