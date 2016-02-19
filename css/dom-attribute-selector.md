# CSS select element using attribute

select an element using that element's attribute:

```css
tag[attribute="val"]    // select "tag" that has "attribute" with value = val
```

```css
tag[attribute|="val"]   // attribute starts with "val"
```

```css
tag[attribute$="val"]   // attribute ends with "val"

```css
tag[attribute*="val"]   // attribute contains "val", which is a part of the word "value"
```

```css
tag[attribute~="value"]   // attribute contains full word "value"
```