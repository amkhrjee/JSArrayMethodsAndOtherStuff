# `Array.prototype.reduce()`

The reduce() method executes a user-supplied “reducer” callback function on each element of the array, in order, passing in the return value from the calculation on the preceding element. The final result of running the reducer across all elements of the array is a single value.

Say we want to sum all of the elements of an array:

```js
let arr = [1, 2, 3, 4, 5];

const sum = arr.reduce((prev, item) => prev + item);

console.log(sum); //15
```

Here the process actually takes four steps to complete, which is a bit counter-intuitive as there are 5 array items.

Here as we have not explicitly supplied any `prev` for the first first iteration of the method, it takes the first item of the array as `prev`.

So here are the following steps:

```js
fn(1, 2); //3
fn(3, 3); //6
fn(6, 4); //10
fn(10, 5); //15
```

We can explicitly provide a `prev` value throgh a second argument in addition to the callback function.

```js
let arr = [1, 2, 3, 4, 5];

const sum = arr.reduce((prev, item) => prev + item, 0);

console.log(sum); //15
```

Here the preocess completes in 5 steps.
