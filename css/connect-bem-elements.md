# Connect parents and children with BEM

BEM is mostly used for self-contain elements, so in order to connect two BEM elements, there is a nice way to do it:

```html
<div class="parent">
    <div class="parent__child child child--modifier">
        <div class="child__smaller-child">Here are some texts</div>
    </div>
</div>
```
