1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```

Answer : first function returns the sum so has return type as 'number' but second function just prints the sum in console and hence has a return value of type 'undefined'

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
   Answer : values of `first` will be 'number' and value of `second` will be 'undefined'.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
   Answer : value returned will be 35 ( 12 + 24) , 35 will be ignored because function does not require it.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
   Answer : yes we can store it in a variable because functions are expressions in JS.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
   Answer :

```js
function sayHello(name) {
  return `Hello ${name}`;
}
```

6. What will be the output of the function below and why?

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

showMessage();
```

Answer : there will be no output as the function is just returning the `message` and not printing anything. The value it returns is 'Hello John'.

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

alert(userName); // Output 1

showMessage(); // Output 2

alert(userName); // Output 3
```

Answer : Output1 - 'Hello John'
Output2 - message will be 'Hello John'
Output 3 - 'Hello John'

8. What is a Anonymous Function give example of three functions.
   Answer : anonymous function is a function without a name. It is used in function expressions.
   Example - let sum = function (a, b) {
   return a + b;
   }

9. Can function declaration be a Anonymous Function? Explain
   Answer : no function declaration can not be anonymous as we need to name of function to call it. In case of IIFE we can have an anonymous function but then again it is a function expression.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```

Answer : getDimension()
calcArea()
getSquare()
showDescription()
checkShape()
