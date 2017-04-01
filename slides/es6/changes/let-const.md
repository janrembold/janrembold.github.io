## var vs. let

fuzzy scope:
```javascript
function varTest(){
  var x = 10;
  if(x > 0) {
    var x = 50;
    console.log(x); // 50
  }
  console.log(x); // 50
}
```

razor blade sharp:
```javascript
function letTest(){
  let x = 10;
  if(x > 0) {
    let x = 50;
    console.log(x); // 50
  }
  console.log(x); // 10
}
```