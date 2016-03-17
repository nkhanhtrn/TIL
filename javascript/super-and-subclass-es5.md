# Create Superclass and Subclass in ES5

Prior to ES6, there is no offical syntax for super and subclass. Thus, to make Object Oriented works with JavaScript, you need to take care of the `prototype` and `constructor`:

```javascript
// Superclass
var Car = function(loc) {
    this.loc = loc;
};
Car.prototype.move = function() {
    this.loc++;
};

var Van = function(loc) {
    Car.call(this, loc);
};
Van.prototype = Object.create(Car.prototype);
Van.prototype.constructor = Van;
```

`call` function is used to set properties of subclass, while `subclass.prototype` is a new Object that links to `superclass.prototype`. The `constructor` method that come free with `prototype` is also needed to be linked with `subclass`, or else it is linked to the `superclass`.
