# Force keeping two or more words on same line

There are two way to keep two or more words inside a box element from breaking into lines when resizing the element:

```HTML
word1&nbsp;word2&nbsp;word3
```
OR

```HTML
word1<span class="transparent-color">_</span>word2<span class="transparent-color">_</span>word3
```
```CSS
.transparent-color {
  color: transparent;
  &:select {
    color: transparent;
  }
}
```
