## prototypal inheritance

```javascript
function Hello(name) {
  this.name = name;
}

Hello.prototype.hello = function hello() {
  return 'Hello ' + this.name + '!';
};

function HelloWorld() {
  Hello.call(this, 'World');
}

HelloWorld.prototype = Object.create(Hello.prototype);
HelloWorld.prototype.constructor = HelloWorld;

HelloWorld.prototype.echo = function echo() {
  console.log(Hello.prototype.hello.call(this));
};

var hw = new HelloWorld();
hw.echo(); // "Hello World!"
```