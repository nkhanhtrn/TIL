# Input with clickable label

Each HTML5 Form input comes with a label that can be used for that input. If the `for` attribute of the label is set to the input's name, clicking on the label with focus the cursor to the input

```html
<label for="input-name">Label here</label>
<input type="text" name="input-name">
```

Another way of doing this is putting the input inside the label itself:

```html
<label for="input-name">Label here
  <input type="text" name="input-name">
</label>
```
