## spread-operator

Doohhh:
```javascript
var arr1 = [1,2,3];
var arr2 = [4,5];

var arr3 = arr1.slice();
arr3.push(4); // [1,2,3,4]

Array.prototype.push.apply(arr1, arr2); // [1,2,3,4,5]
```

Bazinga:
```javascript
let arr1 = [1,2,3];
let arr2 = [4,5];

let arr3 = [...arr1, 4]; // [1,2,3,4]

arr1.push(...arr2); // [1,2,3,4,5]
```