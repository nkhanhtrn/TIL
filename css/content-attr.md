# Get value from attribute in CSS

value from attribute in CSS can be obtained by attr(). However, it only support `content` for now, and other CSS attributes are experimental

```css
.el::after {
    content: attr('data-content');
}
```
