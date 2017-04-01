## modules aka namespaces

lib/math.js
```javascript
LibMath = {}; // just wasted the global namespace
LibMath.pi = 3.1415926536;
LibMath.sum = function (x, y) {
    return x + y
};
```

echo.js // load after lib/math.js
```javascript
console.log("2*pi = " + LibMath.sum(LibMath.pi, LibMath.pi));
```