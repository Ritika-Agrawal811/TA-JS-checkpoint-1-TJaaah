1. Using loops take 10 inputs from user and find the average of all the numbers.

```js
let sum = 0;
for (let i = 0; i < 10; i++) {
  let num = prompt("Enter a number");
  sum = sum + num;
}

let average = sum / 10;
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println("hi");
  i++;
}
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

```js
function getEvenSum(max = 10) {
  let sum = 0;
  for (let i = 0; i < max; i++) {
    let num = prompt("Enter a number");
    if (num % 2 == 0) {
      sum = sum + num;
    }
  }

  return sum;
}
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

```js
function getOddSum(max = 10) {
  let sum = 0;
  for (let i = 0; i < max; i++) {
    let num = prompt("Enter a number");
    if (num % 2 != 0) {
      sum = sum + num;
    }
  }

  return sum;
}
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

```js
function getProductOfDigits(num) {
  let product = 1;

  if (num < 0) {
    return `not a valid input`;
  } else {
    while (num > 0) {
      let digit = num % 10;
      num = Math.floor(num / 10);
      product = product * digit;
    }
  }

  return product;
}
```

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return "Bigger than 5";
  }

  if (num < 5) {
    return "Smaller than 5";
  }

  return num;
}

check(10); // output - "Bigger than 5"
check(1); // output - "Smaller than 5"
check(5); // output - 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") return "You are arya";
  if (name === "John") return "You are john";
  return "Who are you";
}

getOutput("Arya"); // what will be the output - "You are arya"
getOutput("John"); // what will be the output - "You are john"
getOutput(); // what will be the output - "Who are you"
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") console.log("You are arya");
  if (name === "John") console.log("You are john");
  return "Who are you";
}

getOutput("Arya"); // what will be the output - "You are arya" here "Who are you" is also returned
getOutput("John"); // what will be the output - "You are john" here "Who are you" is also returned
getOutput(); // what will be the output - "Who are you"
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
   yes a function can have multiple return statements.

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
