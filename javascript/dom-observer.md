# Listen to changes in DOM with MutationObserver

Using [MutationObserver] (https://developer.mozilla.org/en/docs/Web/API/MutationObserver), many changes in DOM elements can be captured and processed:


```JavaScript
var observer = new MutationObserver(function(mutations) {
    mutations.forEach(function(mutation) {
        // callback function here
    });
});

// configuration for observer object
var config = { attributes: true, childList: true, characterData: true };

// observe a DOM with configuration
observer.observe(node, config);

// stop watching
observer.disconnect();

```
