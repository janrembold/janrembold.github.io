## function default parameter

dusty way:
```javascript
function pow(base, exp){
  if( typeof exp === 'undefined' ) {
    exp = 2;
  }
  return Math.pow(base, exp);
}
pow(4); // 16
```

bling bling way:
```javascript
function pow(base, exp=2){
  return Math.pow(base, exp);
}
pow(4); // 16
```