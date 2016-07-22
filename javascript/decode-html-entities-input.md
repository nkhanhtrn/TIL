# Decode HTML Entities inside Input

Sometime HTML Entities cannot be decoded. This trick will ensure they are decoded inside the input

```javascript
$('input[type=text]').val(function() {
  if (this.value.indexOf('&') != -1) {
    var txt = document.createElement('textarea');
    txt.innerHTML = this.value;
    return xt.value;
  }
});
```

  
