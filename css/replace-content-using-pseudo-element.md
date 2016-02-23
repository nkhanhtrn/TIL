# Replace content using pseudo elements

Sometime when you don't have access to the markup file of a website, but want to replace the content of an element. For this case you can hide the old element and use the pseudo element to show the new content:

Assuming we have this element:

```html
<span class="content">I like you</span>
```

With the correct CSS, you can replace the `I like you` text to something else:

```css
.content {
    opacity: 0;
    visibility: hidden;
}

.content::before {
    content: 'Just kidding!';
    opacity: 1;
    visibility: visible;
}
```

