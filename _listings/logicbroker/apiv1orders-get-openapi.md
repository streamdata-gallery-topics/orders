---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Search orders
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Orders/PickList:
    get:
      summary: Get pick lists for multiple orders
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetOrderPickListToken
      x-api-path-slug: apiv1orderspicklist-get
      parameters:
      - in: query
        name: FileType
        description: 'Valid types: jpg, png, pdf, ps, zpl'
      - in: query
        name: LogicbrokerKeys
        description: The logicbroker Keys
      - in: query
        name: ViewInBrowser
        description: Set to true to view the resulting link in the browser
      responses:
        200:
          description: OK
      tags:
      - Pick
      - Listsmultiple
      - Orders
  /api/v1/Orders:
    get:
      summary: Search orders
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_SearchSalesOrders
      x-api-path-slug: apiv1orders-get
      parameters:
      - in: query
        name: Filters.advanced
        description: Advanced query options
      - in: query
        name: Filters.from
        description: Beginning of time search window
      - in: query
        name: Filters.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: Filters.page
        description: Page number
      - in: query
        name: Filters.pageSize
        description: Page size
      - in: query
        name: Filters.partnerPO
        description: The partners purchase order number
      - in: query
        name: Filters.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: Filters.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: Filters.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: Filters.status
        description: The status of the document
      - in: query
        name: Filters.to
        description: End of time search window
      responses:
        200:
          description: OK
      tags:
      - Search
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