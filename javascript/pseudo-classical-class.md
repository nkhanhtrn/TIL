# Pseudo Classical Class

Before ES6, creating class in JavaScript is a little bit tricky. The language doesn't support proper Object Oriented, thus you need to do a little hack to make it work:

```javascript

var Car = function(location) {
    // this = Object.create(Car.prototype);
    this.location = location;
    // return this;
};

Car.prototype.move = function() {
    this.location++;
};
```

```javascript
var bmw = new Car(10);
```

if keyword `new` is used, the commented lines on block 1 will be automatically inserted at runtime (You cannot assign `this` to something else in JavaScript). This is call Pseudo Classical Pattern and it adds a thin syntactical layer to the Prototypcal Pattern.
