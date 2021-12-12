# `Array.prototype.concat()`

The `concat()` mathod returns an array after appending whatever you would like to add on an existing array.
It can also take in other arrays! 😊

> You cannot produce flat arrays for nested arrays 😔

For example :

```js
var items = [1, 2];
var newItems = items.concat([3, 4], [5, [6, 7], 8]);

console.log(newItems); // [1,2,3,4,5,[6,7],8]
```
