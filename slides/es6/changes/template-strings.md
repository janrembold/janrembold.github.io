## template-strings

that sucks:
```javascript
var a = 10;
var b = 20;
console.log('Sum of ' + a + ' and ' + b + ' = ' + (a + b));
```

much cleaner:
```javascript
let a = 10;
let b = 20;
console.log(`Sum of ${a} and ${b} = ${a + b}`);
```