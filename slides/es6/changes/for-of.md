# for...of

We all know that one:
```javascript
var list = [8, 3, 11];

for (var i = 0; i < list.length; i++) {
  console.log(list[i]);
}

// or since IE9+
list.forEach(function(value, index) {
  console.log(value);
});
```

Mighty and short:
```javascript
let list = [8, 3, 11];

for (let value of list) {
   console.log(value);
}

// works for all `iterable` objects:
// like Array, Map, Set, Strings, arguments...
```