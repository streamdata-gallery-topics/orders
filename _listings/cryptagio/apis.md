---
name: Cryptagio
x-slug: cryptagio
description: Cryptagio is a global crypto exchange, providing a simple, fast and secure
  way to buy, sell or trade the world&rsquo;s most eminent digital assets.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
x-kinRank: "7"
x-alexaRank: "892881"
tags: Orders
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/cryptagio/apis.md
specificationVersion: "0.14"
apis:
- name: Cryptagio API - GetMy  Orders
  x-api-slug: ordersmy-get
  description: Trades are sorted in reverse creation order.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/cryptagio/ordersmy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/cryptagio/ordersmy-get-openapi.md
- name: Cryptagio API - Post Orders
  x-api-slug: orders-post
  description: Accepts an array of JSON objects.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/cryptagio/orders-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/cryptagio/orders-post-openapi.md
- name: Cryptagio API - Post Orders Cancel
  x-api-slug: orderscancel-post
  description: Accepts JSON object. Cancels all orders if no parameters are passed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/cryptagio/orderscancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/cryptagio/orderscancel-post-openapi.md
- name: Cryptagio API - Delete Orders
  x-api-slug: ordersuuid-delete
  description: Cancel order by uuid..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/cryptagio/ordersuuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/cryptagio/ordersuuid-delete-openapi.md
x-common:
- type: x-blog
  url: https://medium.com/@cryptagio
- type: x-blog-rss
  url: view-source:https://medium.com/feed/@cryptagio
- type: x-openapi
  url: https://api.cryptagio.com/docs/CryptagioAPI.json
- type: x-website
  url: http://www.cryptagio.com
- type: x-api-gallery
  url: http://coutts.api.gallery.streamdata.io
- type: x-api-stack
  url: http://cryptagio.stack.network
- type: x-documentation
  url: https://api.cryptagio.com/docs/
- type: x-security
  url: https://cryptagio.com/about
- type: x-support
  url: https://support.cryptagio.com/hc/en-us
- type: x-twitter
  url: https://twitter.com/cryptagio
- type: x-website
  url: https://api.cryptagio.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---