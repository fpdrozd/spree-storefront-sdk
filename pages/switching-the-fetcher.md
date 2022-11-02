Spree SDK does not come bundled with a HTTP client. A HTTP client may have to be installed before using the library. Out of the box, Spree SDK supports using [Axios](https://github.com/axios/axios) and [fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) HTTP clients to communicate with Spree.

**Option A - RECOMMENDED: Spree SDK in NodeJS using Axios**

To use Spree SDK with Axios in NodeJS, install Axios using NPM:

```
npm install axios
```

Set the fetcher to axios when creating the Spree SDK client:

```js
const createAxiosFetcher = require('@spree/storefront-api-v2-sdk/dist/server/createAxiosFetcher').default
const { makeClient } = require('@spree/storefront-api-v2-sdk')

const client = makeClient({
  host: 'http://localhost:3000',
  createFetcher: createAxiosFetcher
})
```

**Option B - Spree SDK in the browser using Axios**

To use Spree SDK with Axios in the browser, include axios as a `<script>` tag before using the SDK:

```html
<script src="https://unpkg.com/@spree/storefront-api-v2-sdk@5.0.0/dist/client/index.js"></script>
<script src="https://unpkg.com/axios@0.24.0/dist/axios.min.js"></script>
<script src="https://unpkg.com/@spree/storefront-api-v2-sdk@5.0.0/dist/client/createAxiosFetcher.js"></script>

<script>
  const client = SpreeSDK.makeClient({
    host: 'http://localhost:3000',
    createFetcher: SpreeSDK.createAxiosFetcher.default
  })
</script>
```

Again, Spree SDK will automatically detect that Axios is available and use it to make requests to Spree.

**Option C - Spree SDK in NodeJS using fetch**

Another supported HTTP client is [fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API). It can be setup in NodeJS as follows:

```
npm install node-fetch
```

Set the fetcher to fetch:

```js
const createFetchFetcher = require('@spree/storefront-api-v2-sdk/dist/server/createFetchFetcher').default
const { makeClient } = require('@spree/storefront-api-v2-sdk')

const client = makeClient({
  host: 'http://localhost:3000',
  createFetcher: createFetchFetcher
})
```

**Option D - Spree SDK in the browser using fetch**

Modern web browsers include fetch natively. To use Spree SDK with native fetch, it's enough to set `fetcherType` to `'fetch'` when creating the Spree SDK Client:

```html
<script src="https://unpkg.com/@spree/storefront-api-v2-sdk@5.0.0/dist/client/index.js"></script>
<script src="https://unpkg.com/@spree/storefront-api-v2-sdk@5.0.0/dist/client/createFetchFetcher.js"></script>

<script>
  const client = SpreeSDK.makeClient({
    host: 'http://localhost:3000',
    createFetcher: SpreeSDK.createFetchFetcher.default
  })
</script>
```

**Option E - ADVANCED: Supply a custom HTTP client.**

To have full control over requests and responses, a custom fetcher can be supplied during the creation of the Spree SDK client:

```js
makeClient({ createFetcher: ... })
```

If you want to use a fetch-compatible interface, use the `createCustomizedFetchFetcher` function.