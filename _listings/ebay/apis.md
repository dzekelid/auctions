---
name: eBay
description: Buy and sell electronics, cars, fashion apparel, collectibles, sporting
  goods, digital cameras, baby items, coupons, and everything else on eBay, the worlds
  online marketplace.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/138_logo.png
x-kinRank: "8"
x-alexaRank: ""
tags:
- Stack
- Partners
- Commerce
- Auction
created: "2018-03-27"
modified: "2018-03-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/auctions/master/_listings/ebay/apis.yaml
specificationVersion: "0.14"
apis:
- name: Ebay
  description: Buy and sell electronics, cars, fashion apparel, collectibles, sporting
    goods, digital cameras, baby items, coupons, and everything else on eBay, the
    worlds online marketplace
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/138_logo.png
  humanURL: ""
  baseURL: https://api.ebay.com//
  tags: Auctions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/auctions/master/_listings/ebay/order-orderid-shipping-fulfillment-fulfillmentid-get.md
- name: Ebay Get Order Order
  description: 'Use this call to retrieve the contents of an order based on its unique
    identifier, orderId. This value was returned in the getOrders call''s orders.orderId
    field when you searched for orders by creation date, modification date, or fulfillment
    status. The returned Order object contains information you can use to create and
    process fulfillments, including: Information about the buyer and seller Information
    about the order''s line items The plans for packaging, addressing and shipping
    the order The status of payment, packaging, addressing, and shipping the order
    A summary of monetary amounts specific to the order such as pricing, payments,
    and shipping costs'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/138_logo.png
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Auctions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/auctions/master/_listings/ebay/order-orderid-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/auctions/master/_listings/ebay/order-orderid-get-postman.md
x-common:
- type: x-blog
  url: https://go.developer.ebay.com/dev-program-blog
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ebay
- type: x-developer
  url: https://go.developer.ebay.com/
- type: x-github
  url: https://github.com/eBayDeveloper
- type: x-twitter
  url: https://twitter.com/ebaydev
- type: x-website
  url: https://ebay.com
- type: x-blog
  url: https://go.developer.ebay.com/dev-program-blog
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ebay
- type: x-developer
  url: https://go.developer.ebay.com/
- type: x-github
  url: https://github.com/eBayDeveloper
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