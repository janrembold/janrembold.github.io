## arrow functions

ES5:
```javascript
this.counter = 0;
var _this = this;
$('a.link').on('click', function() {
    _this.counter++;
});
```

ES6:
```javascript
this.counter = 0;
$('a.link').on('click', () => {
    this.counter++;
});
```