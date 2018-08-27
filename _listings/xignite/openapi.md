swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
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