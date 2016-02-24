# Align content vertically inside a DIV

To align content vertically, simuate the DIV as a table cell:

```html
<div class="container">
    <div class="cell">
        content
    </div>
</div>
```

```css
.container {
    display: table;
}

.container .cell {
    display: table-cell;
    vertical-align: middle;
    text-align: center;
}
```
