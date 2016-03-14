# Event Delegation

When you are working with a set of DOM elements and don't want to rebind events each time you remove/add the same type of DOM, you can apply event delegation to make the event binded to the elements' parent:

```html
<ul class="parent">
  <li class="child">Item 1</li>
  <li class="child">Item 2</li>
  <li class="child">Item 3</li>
</ul>
```

```javascript
$('.parent').click(function(ev) {
    if ($(ev.target).hasClass('child')) {
        alert('you click on a child');
    }
});
```
