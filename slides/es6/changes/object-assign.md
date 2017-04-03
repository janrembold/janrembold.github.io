## Object.assign

what a fake:
```javascript
let defaults = {prop1: 1}, options {prop2: 2};
let settings = _.extend({}, defaults, options);
// settings = {prop1: 1, prop2: 2}
```

yours truly:
```javascript
let defaults = {prop1: 1}, options {prop2: 2};
let settings = Object.assign({}, defaults, options);
// settings = {prop1: 1, prop2: 2}
```