# Draw a triangle in CSS

CSS only supports box model; but a hack with the border setting can be used to create the triangle.

```css
.triangle {
    width: 0;
    height: 0;
    border-top: 50px solid black;
    border-left: 50px solid transparent;
    border-right: 50px solid transparent;
}
```

The trick is to use transparent color to remove the side borders.
