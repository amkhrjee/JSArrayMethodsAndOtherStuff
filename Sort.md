# `Array.prototype.sort()`

It sorts the array and returns the same array.

> The default sort order is ascending, built upon converting the elements into strings, then comparing their sequences of UTF-16 code units values.

This, however doesn't exactly work for numbers as it by default converts everything to string and compares them.

## Performing a Numeric Sort

To perform a numeric sort we need to provide a _comparator function_.

```js
let items = [10, 30, 2, 20];
items.sort((a, b) => a - b);
```

Here is a practical example:

```js
let lessons = [
  {
    title: "A",
    views: 100,
  },
  {
    title: "B",
    views: 200,
  },
  {
    title: "C",
    views: 300,
  },
];

let list = lessons
  .sort((a, b) => b.views - a.views)
  .map((x) => `  <li>${x.title} has ${x.views} views</li>`)
  .join("\n");

let output = `<ul>\n${list}\n</ul>`;
```
