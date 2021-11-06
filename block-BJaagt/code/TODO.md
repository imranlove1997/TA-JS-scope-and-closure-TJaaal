Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(username); // ReferenceError: username is not defined
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(username); // ReferenceError: username is not defined
```

In above code variable username is defined inside the block because of that when we are logging it will give us error.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // ReferenceError: username is not defined
```

In above code variable is declared with if block global scope thats why username is not defined.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(username); // Arya
```

In above code variable we are using var to define the variable so because of tht we get the value of username.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); // Identifier 'username' has already been declared
```

In above code we cant declare an variable with var again so thats why we will get an error.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // John
```

In above code we have be declared variable so we will not get an error.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // John
```

In above code FEC will update the value of username in its memory.


8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0 'First'
                           /* 1 'First'
                            2 'First'
                            3 'First'
                            4 'First'
                            5 'First'
                            6 'First'
                            7 'First'
                            8 'First'
                            9 'First' */
}
console.log(i, 'Second'); // 10 'Second'
```

In above code we are using var and var can store the value in the box so when we execute our code outside of loop we will get the value with the output of 10 second 

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0 'First'
                            /* 1 'First'
                            2 'First'
                            3 'First'
                            4 'First'
                            5 'First'
                            6 'First'
                            7 'First'
                            8 'First'
                            9 'First' */
}
console.log(i, 'Second'); // ReferenceError: i is not defined
```
In above code let is an block level scope so thats why we will get an error outside of loop