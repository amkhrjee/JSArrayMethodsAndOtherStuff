# `Array.prototype.join()`

The `join()` method produces an array that is the result of adding together all items of an array.
In the argument you provide what you want the separator to be in-between the array items.

For example:

```js
let names = ["Peter", "Parker", "Mary", "Jane"];

console.log(names.join(" 🕸️ ")); //'Peter 🕸️ Parker 🕸️ Mary 🕸️ Jane'
```

### `String.prototype.split()`

The `split()` method divides a `String` into an ordered list of substrings, puts these substrings into an array, and _returns the array_. The division is done by searching for a pattern; where the pattern is provided as the first parameter in the method's call.

### `Array.prototype.map()`

Creates a new `Array` by calling a function on the elements of a different `Array`

```js
const users = [{ name: "🐼" }, { name: "🐨" }, { name: "🦥" }];

const differentArray = users.map((user) => user.name); //["🐼", "🐨", "🦥"]
```
