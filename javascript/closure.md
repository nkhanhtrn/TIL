# Closure in JavaScript

Closure in JavaScript closely related to Lexical Scope. Basically, closure makes local variable accessible from out side of the function, thus protect the availability of the variable but still make it usable outside scope.

```javascript
var hello = function() {
    var person = { age: 99, name: 'Voldermort'};
    return function() {
        return person;
    }
};

hello()();    // => return person
```
