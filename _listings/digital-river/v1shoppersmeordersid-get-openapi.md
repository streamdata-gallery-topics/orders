---
swagger: "2.0"
x-collection-name: Digital River
x-complete: 0
info:
  title: Digital River Shopper API Get Shoppers Me Orders
  description: Get shoppers me orders.
  version: v1
host: store.digitalriver.com
basePath: /store/{mysite}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/shoppers/me/orders:
    get:
      summary: Get Shoppers Me Orders
      description: Get shoppers me orders.
      operationId: getV1ShoppersMeOrders
      x-api-path-slug: v1shoppersmeorders-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Orders
    post:
      summary: Post Shoppers Me Orders
      description: Post shoppers me orders.
      operationId: postV1ShoppersMeOrders
      x-api-path-slug: v1shoppersmeorders-post
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Orders
  /v1/shoppers/me/orders/{id}:
    get:
      summary: Get Shoppers Me Orders
      description: Get shoppers me orders.
      operationId: getV1ShoppersMeOrders
      x-api-path-slug: v1shoppersmeordersid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Orders
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---