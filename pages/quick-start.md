Install the NPM package:

```
npm install --save @spree/storefront-api-v2-sdk
```

Install the [Axios](https://github.com/axios/axios) HTTP client:

```
npm install --save axios
```

Create a client and use it to call Spree:

```js
const createAxiosFetcher = require('@spree/storefront-api-v2-sdk/dist/server/createAxiosFetcher').default
const { makeClient } = require('@spree/storefront-api-v2-sdk')

const client = makeClient({
  host: 'http://localhost:3000',
  createFetcher: createAxiosFetcher
})

client.products
  .list({
    include: 'default_variant',
    page: 1
  })
  .then((spreeResponse) => {
    console.log(spreeResponse.success())
  })
```

_Spree SDK can also be imported using `import` and `<script>` tags in the browser. Check the {@page alternative-setups.md} section for examples._

_For details about HTTP clients, read the {@page switching-the-fetcher.md} section._