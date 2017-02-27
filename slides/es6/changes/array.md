## arrow functions demo

ES5:
```javascript
function Person(){
  var that = this;
  that.age = 0;
  setInterval(() => {
    that.age++;
  }, 1000);
}
var p = new Person();
```

ES6:
```javascript
function Person(){
  this.age = 0;
  setInterval(() => {
    this.age++;
  }, 1000);
}
var p = new Person();
```