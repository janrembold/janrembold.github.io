## arrow functions demo

ES5:
```javascript
function Person(){
  var that = this;
  that.age = 0;
  setInterval(() => {
    that.age++; // |that| bezieht sich entsprechend auf das person-Objekt
  }, 1000);
}
var p = new Person();
```

ES6:
```javascript
function Person(){
  this.age = 0;
  setInterval(() => {
    this.age++; // |this| bezieht sich entsprechend auf das person-Objekt
  }, 1000);
}
var p = new Person();
```