## es6 modules - import and export

lib/math.js
```javascript
export const pi = 3.1415926536;
export function sum (x, y) {
    return x + y;
}
```

echo.js
```javascript
import * as math from "lib/math";
console.log(`2*pi = ${math.sum(math.pi, math.pi)}`);
```