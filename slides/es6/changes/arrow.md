#arrow

ES5:
```javascript
this.counter = 0;
// ...
var _this = this;
$('a.link').on('click', function(e) {
    _this.counter++;
});
```

ES6:
```javascript
this.counter = 0;
// ...
$('a.link').on('click', (e) => {
    this.counter++;
});
```