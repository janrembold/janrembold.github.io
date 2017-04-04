## es6 classes

```javascript
class Hello {
  constructor(name) { this.name = name; }

  hello() {
    return 'Hello ' + this.name + '!';
  }
}

class HelloWorld extends Hello {
  constructor() { super('World'); }

  echo() {
    console.log(super.hello());
  }
}
```