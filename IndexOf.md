# `Array.prototyoe.indexOf()`

If the item does not exist then it returns `-1`.

```js
let family = ['Shane', 'Sally', 'Isaac', 'Kittie']
let kittieExists = family.indexOf('Kittie') > -1

if(!kittieExists) {
    family.push('Kittie)
}

```

Providing a second argumnt specifies from which index to start looking for the first argument.

Making a filter with `indexOf()` method:

```js
let whitelist = ['.css', '.js']

let events = [
    {
        file: 'css/core.css';
    },
    {
        file: 'js/app.js'
    },
    {
        file: 'index.html'
    }
]

let filtered = events.filter(event => {
    let ext = require('path').extname(event.file)
    return whitelist.indexOF(ext) > -1
})


```

### `Array.prototype.filter()`

The `filter() `method **creates a new array** with all elements that pass the test implemented by the provided function.
