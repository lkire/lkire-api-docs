# Authorization

> To obtain access to protected demos, please fill out the request form on the Contact page. If you would like to embed protected resources or access protected APIs please indicate so on the request form.



```python
import lkire-api

api = lkire-api.authorize('youraccesstocken')
```

```javascript
const lkire-api = require('lkire-api');

let api = lkire-api.authorize('youraccesstoken');
```

> Make sure to replace `youraccesstoken` with your API key.

lkire.com uses API keys to allow access to restricted APIs. You can register a new lkire.com API key at the [Contact Page](http://lkire.com/contact).

lkire.com expects for the API key to be included in all restricted API requests to the server in a header that looks like the following:

`Authorization: youraccesstoken`

<aside class="notice">
You must replace <code>youraccesstoken</code> with your personal API key.
</aside>

