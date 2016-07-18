# Create delay between Requests to prevent flooding the server

```javascript
var allow_request = false;
const DELAY_TIME = 500;

if (!allow_request) {
  allow_request = true;

  setTimeout(function() {
    allow_request == false;
    }, DELAY_TIME);
    
  request();
}
```

The blocks script above will delay the request to 500ms.
