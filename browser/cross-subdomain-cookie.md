# Cross Subdomain Cookie

Cookies can be shared between subdomains if it satisfy these following conditions:
- Domain name must be in format `*.domain.com*`
- Path name must be root `*/*`

If these two conditions are satisfied, the cookie will be accessible across sub domains.

To set the cookie using JavaScript, use the following snippet:

```javascript
    document.cookie = "name=val;path=/;domain=.domain.com";
```
