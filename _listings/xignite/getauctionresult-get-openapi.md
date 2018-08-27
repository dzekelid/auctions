---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Rates Get Auction Result
  description: Returns an auction result by cusip.
  version: 1.0.0
host: www.xignite.com
basePath: xRates.json/XigniteRates
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetAuctionResult:
    get:
      summary: Get Auction Result
      description: Returns an auction result by cusip.
      operationId: postGetauctionresult
      x-api-path-slug: getauctionresult-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Auction
      - Result
  /GetAuctionResults:
    get:
      summary: Get Auction Results
      description: Returns auction results by date.
      operationId: postGetauctionresults
      x-api-path-slug: getauctionresults-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Auction
      - Results
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