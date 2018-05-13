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
- name: Ebay Get Item Get Item By Legacy
  description: This call is a bridge between the eBay legacy APIs, such as Trading,
    Shopping, and Finding and the eBay Buy APIs. There are differences between how
    legacy APIs and RESTful APIs return the identifier of an &quot;item&quot;. There
    is also a difference in what the item Id represents and in the format of the item
    Id value returned. This call lets you use the legacy item Ids retrieve the details
    of a specific item, such as description, price, and other information the buyer
    needs to make a purchasing decision. It also returns the RESTful item Id, which
    you can use with all the Buy API calls. For more information about how to use
    legacy Ids with the Buy APIs, see Legacy API compatibility in the Buying Integration
    guide. This call returns the item details and requires you to pass in either the
    item Id of a non-variation item or the item Ids of both the parent and child of
    a item group. An item group is an item that has various aspect differences, such
    as color, size, storage capacity, etc. When an item group is created, one of the
    item variations, such as the red shirt size L, is chosen as the &quot;parent&quot;.
    All the other items in the group are the children, such as the blue shirt size
    L, red shirt size M, etc. The fieldgroups URI parameter lets you control what
    is returned in the response. Setting fieldgroups to PRODUCT, adds additional fields
    to the default response that return information about the product of the item.
    For more information, see fieldgroups. Request headers You will want to use the
    X-EBAY-C-ENDUSERCTX request header with this call. If you are an eBay Network
    Partner you must use affiliateCampaignId=ePNCampaignId,affiliateReferenceId=referenceId
    in the header in order to be paid for selling eBay items on your site and it is
    strongly recommended you use contextualLocation to improved the estimated delivery
    window information. For details see, Request headers in the Buy APIs Overview.
    Restrictions For a list of supported sites and other restrictions, see API Restrictions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/138_logo.png
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Auctions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/auctions/master/_listings/ebay/item-get-item-by-legacy-id-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/auctions/master/_listings/ebay/item-get-item-by-legacy-id-get-postman.md
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