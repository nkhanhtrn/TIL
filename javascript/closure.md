# Closure in JavaScript

Closure in JavaScript closely related to Lexical Scope. Basically, closure makes local variable viewable from out side of the function, but still protect the accessibility of that variable.

```javascript
var hello = function() {
    var person = { age: 99, name: 'Voldermort'};
    return function() {
        return person;
    }
};

hello()();    // => return person
```
