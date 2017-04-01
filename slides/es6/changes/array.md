## array functions

old style:
```javascript
[ 1, 3, 4, 2 ].filter(function (x) { return x > 3; })[0]; // 4
```

shiny new:
```javascript
[ 1, 3, 4, 2 ].find(x => x > 3); // 4
```