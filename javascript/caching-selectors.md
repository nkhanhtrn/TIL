# Caching selectors to improve performance

Each selector query will travel throughout the DOM to find the element. This is counter-productive and can harm your application performance.

To avoid this issue, it's a good practice to cache the query with either using variables or through automatic caching. 

```javascript
function cachingEls(query) {
    this.cache = this.cache || {};
    
    if (!this.cache[query]) {
        this.cache[query] = $(query);      
    }
    
    return this.cache[query];
}
```

To use the function:
```javascript
cachingEls('#id').val();
```
