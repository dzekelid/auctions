swagger: "2.0"
x-collection-name: Blizzard
x-complete: 1
info:
  title: World of Warcraft
  description: welcome-to-the-restful-apis-exposed-through-the-world-of-warcraft-community-site-as-a-service-to-the-world-of-warcraft-community-
  version: 1.0.0
host: us.battle.net
basePath: /api/wow/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /auction/data/{realm}:
    get:
      summary: Get Auction Data Realm
      description: Provides a per-realm list of recently generated auction house data
        dumps. The current auctions data is represented as JSON structures containing
        auction data for the tree auctions houses available on each realm.
      operationId: getAuctionDataRealm
      x-api-path-slug: auctiondatarealm-get
      parameters:
      - in: path
        name: realm
        description: The realm name
      responses:
        200:
          description: OK
      tags:
      - Auction
      - Data
      - Realm