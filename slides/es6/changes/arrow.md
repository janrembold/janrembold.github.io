## arrow functions

old school:
```javascript
function Person(){
  var that = this;
  that.age = 0;

  setInterval(function() {
    that.age++; // <= that context
  }, 1000);
}
var p = new Person();
```

shiny new:
```javascript
function Person(){
  this.age = 0;

  setInterval(() => {
    this.age++; // <= this context
  }, 1000);
}
var p = new Person();
```