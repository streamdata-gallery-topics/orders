---
swagger: "2.0"
x-collection-name: eBay
x-complete: 0
info:
  title: Ebay Get Order
  description: 'Use this call to search for and retrieve one or more orders based
    on their creation date, last modification date, or fulfillment status using the
    filter parameter. You can alternatively specify a list of orders using the orderIds
    parameter. The returned Order objects contain information you can use to create
    and process fulfillments, including: Information about the buyer and seller Information
    about the order''s line items The plans for packaging, addressing and shipping
    the order The status of payment, packaging, addressing, and shipping the order
    A summary of monetary amounts specific to the order such as pricing, payments,
    and shipping costs Important: In this call, the cancelStatus.cancelRequests array
    is returned but is always empty. Use the getOrder call instead, which returns
    this array fully populated with information about any cancellation requests.'
  contact:
    name: eBay Inc.
  version: 1.0.0
host: api.ebay.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /order:
    get:
      summary: Get Order
      description: 'Use this call to search for and retrieve one or more orders based
        on their creation date, last modification date, or fulfillment status using
        the filter parameter. You can alternatively specify a list of orders using
        the orderIds parameter. The returned Order objects contain information you
        can use to create and process fulfillments, including: Information about the
        buyer and seller Information about the order''s line items The plans for packaging,
        addressing and shipping the order The status of payment, packaging, addressing,
        and shipping the order A summary of monetary amounts specific to the order
        such as pricing, payments, and shipping costs Important: In this call, the
        cancelStatus.cancelRequests array is returned but is always empty. Use the
        getOrder call instead, which returns this array fully populated with information
        about any cancellation requests.'
      operationId: getOrders
      x-api-path-slug: order-get
      parameters:
      - in: query
        name: filter
        description: One or more comma-separated criteria for narrowing down the collection
          of orders returned by this call
      - in: query
        name: limit
        description: The number of orders to return in the current result set
      - in: query
        name: offset
        description: The first order to return based on its position in the collection
          of orders
      - in: query
        name: orderIds
        description: A comma-separated list of the unique identifiers of the orders
          to retrieve (maximum 50)
      responses:
        200:
          description: OK
      tags:
      - Auctions
      - Order
  /order/{orderId}:
    get:
      summary: Get Order Order
      description: 'Use this call to retrieve the contents of an order based on its
        unique identifier, orderId. This value was returned in the getOrders call''s
        orders.orderId field when you searched for orders by creation date, modification
        date, or fulfillment status. The returned Order object contains information
        you can use to create and process fulfillments, including: Information about
        the buyer and seller Information about the order''s line items The plans for
        packaging, addressing and shipping the order The status of payment, packaging,
        addressing, and shipping the order A summary of monetary amounts specific
        to the order such as pricing, payments, and shipping costs'
      operationId: getOrder
      x-api-path-slug: orderorderid-get
      parameters:
      - in: path
        name: orderId
        description: The unique identifier of the order
      responses:
        200:
          description: OK
      tags:
      - Auctions
      - Order
      - Order
  /order/{orderId}/shipping_fulfillment:
    get:
      summary: Get Order Order Shipping Fulfillment
      description: Use this call to retrieve the contents of all fulfillments currently
        defined for a specified order based on the order's unique identifier, orderId.
        This value is returned in the getOrders call's members.orderId field when
        you search for orders by creation date or shipment status.
      operationId: getShippingFulfillments
      x-api-path-slug: orderorderidshipping-fulfillment-get
      parameters:
      - in: path
        name: orderId
        description: The unique identifier of the order
      responses:
        200:
          description: OK
      tags:
      - Auctions
      - Order
      - Order
      - Shipping
      - Fulfillment
    post:
      summary: Add Order Order Shipping Fulfillment
      description: 'When you group an order''s line items into one or more packages,
        each package requires a corresponding plan for handling, addressing, and shipping;
        this is a shipping fulfillment. For each package, execute this call once to
        generate a shipping fulfillment associated with that package. Note: A single
        line item in an order can consist of multiple units of a purchased item, and
        one unit can consist of multiple parts or components. Although these components
        might be provided by the manufacturer in separate packaging, the seller must
        include all components of a given line item in the same package.Before using
        this call for a given package, you must determine which line items are in
        the package. If the package has been shipped, you should provide the date
        of shipment in the request. If not provided, it will default to the current
        date and time.'
      operationId: createShippingFulfillment
      x-api-path-slug: orderorderidshipping-fulfillment-post
      parameters:
      - in: body
        name: body
        description: fulfillment payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
        description: The unique identifier of the order
      responses:
        200:
          description: OK
      tags:
      - Auctions
      - Order
      - Order
      - Shipping
      - Fulfillment
  /order/{orderId}/shipping_fulfillment/{fulfillmentId}:
    get:
      summary: Get Order Order Shipping Fulfillment Fulfillment
      description: Use this call to retrieve the contents of a fulfillment based on
        its unique identifier, fulfillmentId (combined with the associated order's
        orderId). The fulfillmentId value was originally generated by the createShippingFulfillment
        call, and is returned by the getShippingFulfillments call in the members.fulfillmentId
        field.
      operationId: getShippingFulfillment
      x-api-path-slug: orderorderidshipping-fulfillmentfulfillmentid-get
      parameters:
      - in: path
        name: fulfillmentId
        description: The unique identifier of the fulfillment
      - in: path
        name: orderId
        description: The unique identifier of the order
      responses:
        200:
          description: OK
      tags:
      - Auctions
      - Order
      - Order
      - Shipping
      - Fulfillment
      - Fulfillment
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