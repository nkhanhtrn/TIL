# will-change CSS
Tell browsers before hand that these attributes will be changed in the future so browsers can do optimization ahead of time. This is still in working-draft so it may change in the future. This attribute is not intended for gaining optimization but only as the last resort to gain speed when an application is troubling with optimization issue.

```css
.element {
  will-change: transform;
}
```
