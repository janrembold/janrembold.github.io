## function default parameter

Dusty way:
```javascript
function pow(base, exp){
  if( isNaN(exp) ) {
    exp = 2;
  }
  return Math.pow(base, exp);
}
pow(4); // 16
```

Bling bling way:
```javascript
function pow(base, exp=2){
  return Math.pow(base, exp);
}
pow(4); // 16
```