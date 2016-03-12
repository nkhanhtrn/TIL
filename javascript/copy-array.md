# Copy array in JavaScript

To copy an array in JavaScript, simple assign new array to the old one won't work since JavaScript behaviours base on reference

```javascript
var arr = {1, 2, 3};
var brr = arr;        // it won't work here because `arr` and `brr` points to the same array
```

So how to copy it? Simply using the `slice()` function without any argument will do the job:

```javascript
var arr = [1, 2, 3];
var brr = arr.slice();
```

Simple and beautiful!
