## destructuring

Really unamazing:
```javascript
function f(){
  var args = Array.prototype.slice.call(arguments, f.length);
  return args[0] + args[1] + args[2];
}
f(1);         // NaN
f(1, 2, 3);   // 6
f(1, 2, 3, 4) // 6
```

Fabulous:
```javascript
function f(...[a, b, c]) {
  return a + b + c;
}
function f(...args) {
  return args[0] + args[1] + args[2];
}
f(1);         // NaN
f(1, 2, 3);   // 6
f(1, 2, 3, 4) // 6
```