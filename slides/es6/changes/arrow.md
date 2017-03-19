## arrow functions

Old school:
```javascript
function Person(){
  var that = this;
  that.age = 0;

  setInterval(function() {
    that.age++;
  }, 1000);
}
var p = new Person();
```

Shiny new:
```javascript
function Person(){
  this.age = 0;

  setInterval(() => {
    this.age++; // <= this context
  }, 1000);
}
var p = new Person();
```