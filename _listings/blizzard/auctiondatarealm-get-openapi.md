---
swagger: "2.0"
x-collection-name: Blizzard
x-complete: 0
info:
  title: World of Warcraft Get Auction Data Realm
  description: Provides a per-realm list of recently generated auction house data
    dumps. The current auctions data is represented as JSON structures containing
    auction data for the tree auctions houses available on each realm.
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