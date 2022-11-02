# Spree Commerce Storefront API v2 JavaScript / TypeScript SDK

Node module to easily integrate your JavaScript or TypeScript application with [Spree API](https://api.spreecommerce.org). You can create an entirely custom Storefront in JS/TS with this package including one page checkout, Single Page Apps, PWAs and so on.

Developed and maintained by:

[![Vendo](https://assets-global.website-files.com/6230c485f2c32ea1b0daa438/623372f40a8c54ca9aea34e8_vendo%202.svg)][vendo]

> All-in-one platform for all your Marketplace and B2B eCommerce needs. [Start your 30-day free trial](https://e98esoirr8c.typeform.com/contactvendo?typeform-source=spree_sdk_github)

## About Vendo

<a href="https://getvendo.com?utm_source=spree_sdk_github">
  <img src="https://uploads-ssl.webflow.com/6230c485f2c32ea1b0daa438/62386b96518cdcbe111f134a_OG%20Image%20(2).png" style="max-height:400px" />
</a>

> [Vendo][vendo] is a great fit for marketplaces of all sizes - either with own fulfillment and multiple warehouses or in a dropshipping model. Vendo **automates everything** from **vendor onboarding**, accepting buyer **payments in over 135 currencies**, to supplier **payouts in 50 countries**. 

> Vendo ensures excellent buyer experience with smooth product discovery and search, a multitude of payment methods and optimal shipping cost calculation. Vendo keeps suppliers happy with easy onboarding, automated products sync using their preferred method and easy payouts.

> [Start your 30-day free trial](https://e98esoirr8c.typeform.com/contactvendo?typeform-source=spree_sdk_github)

[1]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error
[3]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/instanceof
[4]: https://jsonapi.org/format/
[5]: https://unpkg.com/@spree/storefront-api-v2-sdk@5.0.0/dist/client/index.js
[6]: https://unpkg.com/@spree/storefront-api-v2-sdk/dist/client/index.js
[7]: https://unpkg.com/
[vendo]: http://getvendo.com?utm_source=spree_sdk_github
[8]: https://github.com/axios/axios
[9]: https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API
[10]: https://github.com/node-fetch/node-fetch
[11]: https://developer.mozilla.org/en-US/docs/Web/API/ReadableStream
[12]: https://api.spreecommerce.org/docs/api-v2/YXBpOjMxMjQ5NjA-storefront-api
[13]: https://api.spreecommerce.org/docs/api-v2/YXBpOjMxMjQ5NTg-authentication
[14]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0MjczNQ-create-an-account
[15]: https://github.com/spree/spree_auth_devise/blob/db4ccf202f42cdb713931e9915b213ab9c9b2062/config/routes.rb
[16]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0MjczNg-update-an-account
[17]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0MjczNA-retrieve-an-account
[18]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0NTE5OQ-list-all-credit-cards
[19]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc0MQ-retrieve-the-default-credit-card
[20]: https://api.spreecommerce.org/docs/api-v2/b3A6MTc1NjU3NDM-remove-a-credit-card
[21]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc0Mg-list-all-orders
[22]: https://api.spreecommerce.org/docs/api-v2/b3A6MTgwNTI4NjA-retrieve-an-order
[23]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0NTE5Ng-list-all-addresses
[24]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0NTE5Nw-create-an-address
[25]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0NTE5OA-update-an-address
[26]: https://api.spreecommerce.org/docs/api-v2/b3A6MTAwNjA3Njg-remove-an-address
[27]: https://api.spreecommerce.org/docs/api-v2/b3A6MTgwNTI4NjE-retrieve-an-order-status
[28]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc0NQ-create-a-cart
[29]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc0Ng-retrieve-a-cart
[30]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc0Nw-add-an-item-to-cart
[31]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc0OA-set-line-item-quantity
[32]: https://api.spreecommerce.org/docs/api-v2/b3A6MTg1MTUyNTg-remove-a-line-item
[33]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc1MA-empty-the-cart
[34]: https://api.spreecommerce.org/docs/api-v2/b3A6MTcyNTA0NDc-delete-a-cart
[35]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc1MQ-apply-a-coupon-code
[36]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc1Mg-remove-a-coupon
[37]: https://api.spreecommerce.org/docs/api-v2/b3A6MjM5NTU3NTg-remove-all-coupons
[38]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc1Mw-list-estimated-shipping-rates
[39]: https://api.spreecommerce.org/docs/api-v2/b3A6MjAxMTAyMzM-associate-a-cart-with-a-user
[40]: https://api.spreecommerce.org/docs/api-v2/b3A6MjA2OTMwMDM-change-cart-currency
[41]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc1NA-update-checkout
[42]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc1NQ-next-checkout-step
[43]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc1Ng-advance-checkout
[44]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc1Nw-complete-checkout
[45]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc1OA-add-store-credit
[46]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc1OQ-remove-store-credit
[47]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc2MA-list-payment-methods
[48]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc2MQ-list-shipping-rates
[49]: https://api.spreecommerce.org/docs/api-v2/b3A6MjY1NTc1NzY-selects-shipping-method-for-shipment-s
[50]: https://api.spreecommerce.org/docs/api-v2/b3A6MjYyODA2NTY-create-new-payment
[51]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc2Mg-list-all-products
[52]: https://api.spreecommerce.org/docs/api-v2/b3A6MTgwNTI4ODE-retrieve-a-product
[53]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc2NA-list-all-taxons
[54]: https://api.spreecommerce.org/docs/api-v2/b3A6MTgwNTI4ODM-retrieve-a-taxon
[55]: https://api.spreecommerce.org/docs/api-v2/b3A6MjE0NTY5Mzg-list-all-wishlists
[56]: https://api.spreecommerce.org/docs/api-v2/b3A6MjE0NTY5NDA-retrieve-a-wishlist
[57]: https://api.spreecommerce.org/docs/api-v2/b3A6MjE0NTY5NDM-retrieve-the-default-wishlist
[58]: https://api.spreecommerce.org/docs/api-v2/b3A6MjE0NTY5Mzk-create-a-wishlist
[59]: https://api.spreecommerce.org/docs/api-v2/b3A6MjM5NTU3ODQ-update-a-wishlist
[60]: https://api.spreecommerce.org/docs/api-v2/b3A6MjE0NTY5NDI-delete-a-wishlist
[61]: https://api.spreecommerce.org/docs/api-v2/b3A6MjE0NTY5NDQ-add-item-to-wishlist
[62]: https://api.spreecommerce.org/docs/api-v2/b3A6MjE0NTY5NDU-set-wished-item-quantity
[63]: https://api.spreecommerce.org/docs/api-v2/b3A6MjE0NTY5NDY-delete-item-from-wishlist
[64]: https://api.spreecommerce.org/docs/api-v2/b3A6MTc3MzEwMzM-list-all-cms-pages
[65]: https://api.spreecommerce.org/docs/api-v2/b3A6MTg4MDA4OTk-retrieve-a-cms-page
[66]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc2Ng-list-all-countries
[67]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc2Nw-retrieve-a-country
[68]: https://api.spreecommerce.org/docs/api-v2/b3A6MzE0Mjc2OA-get-default-country
[69]: https://api.spreecommerce.org/docs/api-v2/b3A6MjQxNjA3ODY-download-a-digital-asset
[70]: https://api.spreecommerce.org/docs/api-v2/b3A6MTc2NjI3MTM-list-all-menus
[71]: https://api.spreecommerce.org/docs/api-v2/b3A6MTc3MzEwMzI-retrieve-a-menu
