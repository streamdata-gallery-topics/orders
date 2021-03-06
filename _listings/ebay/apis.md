---
name: eBay
x-slug: ebay
description: Buy and sell electronics, cars, fashion apparel, collectibles, sporting
  goods, digital cameras, baby items, coupons, and everything else on eBay, the worlds
  online marketplace
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
x-kinRank: "8"
x-alexaRank: "42"
tags: Orders
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/apis.md
specificationVersion: "0.14"
apis:
- name: Ebay - Get Order
  x-api-slug: order-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/order-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/order-get-openapi.md
- name: Ebay - Get Order Order
  x-api-slug: orderorderid-get
  description: 'Use this call to retrieve the contents of an order based on its unique
    identifier, orderId. This value was returned in the getOrders call''s orders.orderId
    field when you searched for orders by creation date, modification date, or fulfillment
    status. The returned Order object contains information you can use to create and
    process fulfillments, including: Information about the buyer and seller Information
    about the order''s line items The plans for packaging, addressing and shipping
    the order The status of payment, packaging, addressing, and shipping the order
    A summary of monetary amounts specific to the order such as pricing, payments,
    and shipping costs'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderid-get-openapi.md
- name: Ebay - Get Order Order Shipping Fulfillment
  x-api-slug: orderorderidshipping-fulfillment-get
  description: Use this call to retrieve the contents of all fulfillments currently
    defined for a specified order based on the order's unique identifier, orderId.
    This value is returned in the getOrders call's members.orderId field when you
    search for orders by creation date or shipment status.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillment-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillment-get-openapi.md
- name: Ebay - Add Order Order Shipping Fulfillment
  x-api-slug: orderorderidshipping-fulfillment-post
  description: 'When you group an order''s line items into one or more packages, each
    package requires a corresponding plan for handling, addressing, and shipping;
    this is a shipping fulfillment. For each package, execute this call once to generate
    a shipping fulfillment associated with that package. Note: A single line item
    in an order can consist of multiple units of a purchased item, and one unit can
    consist of multiple parts or components. Although these components might be provided
    by the manufacturer in separate packaging, the seller must include all components
    of a given line item in the same package.Before using this call for a given package,
    you must determine which line items are in the package. If the package has been
    shipped, you should provide the date of shipment in the request. If not provided,
    it will default to the current date and time.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillment-post-openapi.md
- name: Ebay - Get Order Order Shipping Fulfillment Fulfillment
  x-api-slug: orderorderidshipping-fulfillmentfulfillmentid-get
  description: Use this call to retrieve the contents of a fulfillment based on its
    unique identifier, fulfillmentId (combined with the associated order's orderId).
    The fulfillmentId value was originally generated by the createShippingFulfillment
    call, and is returned by the getShippingFulfillments call in the members.fulfillmentId
    field.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillmentfulfillmentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillmentfulfillmentid-get-openapi.md
- name: Ebay - Get Order
  x-api-slug: order-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/order-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/order-get-openapi.md
- name: Ebay - Get Order Order
  x-api-slug: orderorderid-get
  description: 'Use this call to retrieve the contents of an order based on its unique
    identifier, orderId. This value was returned in the getOrders call''s orders.orderId
    field when you searched for orders by creation date, modification date, or fulfillment
    status. The returned Order object contains information you can use to create and
    process fulfillments, including: Information about the buyer and seller Information
    about the order''s line items The plans for packaging, addressing and shipping
    the order The status of payment, packaging, addressing, and shipping the order
    A summary of monetary amounts specific to the order such as pricing, payments,
    and shipping costs'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderid-get-openapi.md
- name: Ebay - Get Order Order Shipping Fulfillment
  x-api-slug: orderorderidshipping-fulfillment-get
  description: Use this call to retrieve the contents of all fulfillments currently
    defined for a specified order based on the order's unique identifier, orderId.
    This value is returned in the getOrders call's members.orderId field when you
    search for orders by creation date or shipment status.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillment-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillment-get-openapi.md
- name: Ebay - Add Order Order Shipping Fulfillment
  x-api-slug: orderorderidshipping-fulfillment-post
  description: 'When you group an order''s line items into one or more packages, each
    package requires a corresponding plan for handling, addressing, and shipping;
    this is a shipping fulfillment. For each package, execute this call once to generate
    a shipping fulfillment associated with that package. Note: A single line item
    in an order can consist of multiple units of a purchased item, and one unit can
    consist of multiple parts or components. Although these components might be provided
    by the manufacturer in separate packaging, the seller must include all components
    of a given line item in the same package.Before using this call for a given package,
    you must determine which line items are in the package. If the package has been
    shipped, you should provide the date of shipment in the request. If not provided,
    it will default to the current date and time.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillment-post-openapi.md
- name: Ebay - Get Order Order Shipping Fulfillment Fulfillment
  x-api-slug: orderorderidshipping-fulfillmentfulfillmentid-get
  description: Use this call to retrieve the contents of a fulfillment based on its
    unique identifier, fulfillmentId (combined with the associated order's orderId).
    The fulfillmentId value was originally generated by the createShippingFulfillment
    call, and is returned by the getShippingFulfillments call in the members.fulfillmentId
    field.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillmentfulfillmentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillmentfulfillmentid-get-openapi.md
- name: Ebay - Get Order Order Shipping Fulfillment Fulfillment
  x-api-slug: orderorderidshipping-fulfillmentfulfillmentid-get
  description: Use this call to retrieve the contents of a fulfillment based on its
    unique identifier, fulfillmentId (combined with the associated order's orderId).
    The fulfillmentId value was originally generated by the createShippingFulfillment
    call, and is returned by the getShippingFulfillments call in the members.fulfillmentId
    field.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillmentfulfillmentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillmentfulfillmentid-get-openapi.md
- name: Ebay - Add Order Order Shipping Fulfillment
  x-api-slug: orderorderidshipping-fulfillment-post
  description: 'When you group an order''s line items into one or more packages, each
    package requires a corresponding plan for handling, addressing, and shipping;
    this is a shipping fulfillment. For each package, execute this call once to generate
    a shipping fulfillment associated with that package. Note: A single line item
    in an order can consist of multiple units of a purchased item, and one unit can
    consist of multiple parts or components. Although these components might be provided
    by the manufacturer in separate packaging, the seller must include all components
    of a given line item in the same package.Before using this call for a given package,
    you must determine which line items are in the package. If the package has been
    shipped, you should provide the date of shipment in the request. If not provided,
    it will default to the current date and time.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillment-post-openapi.md
- name: Ebay - Get Order Order Shipping Fulfillment
  x-api-slug: orderorderidshipping-fulfillment-get
  description: Use this call to retrieve the contents of all fulfillments currently
    defined for a specified order based on the order's unique identifier, orderId.
    This value is returned in the getOrders call's members.orderId field when you
    search for orders by creation date or shipment status.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillment-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderidshipping-fulfillment-get-openapi.md
- name: Ebay - Get Order Order
  x-api-slug: orderorderid-get
  description: 'Use this call to retrieve the contents of an order based on its unique
    identifier, orderId. This value was returned in the getOrders call''s orders.orderId
    field when you searched for orders by creation date, modification date, or fulfillment
    status. The returned Order object contains information you can use to create and
    process fulfillments, including: Information about the buyer and seller Information
    about the order''s line items The plans for packaging, addressing and shipping
    the order The status of payment, packaging, addressing, and shipping the order
    A summary of monetary amounts specific to the order such as pricing, payments,
    and shipping costs'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/orderorderid-get-openapi.md
- name: Ebay - Get Order
  x-api-slug: order-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/order-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ebay/order-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://easycron.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ebay.stack.network
- type: x-blog
  url: https://go.developer.ebay.com/dev-program-blog
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ebay
- type: x-crunchbase
  url: https://crunchbase.com/organization/leah
- type: x-developer
  url: https://go.developer.ebay.com/
- type: x-email
  url: spam@ebay.com
- type: x-email
  url: spoof@ebay.com
- type: x-github
  url: https://github.com/eBayDeveloper
- type: x-twitter
  url: https://twitter.com/eBay
- type: x-twitter
  url: https://twitter.com/ebaydev
- type: x-website
  url: https://ebay.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---