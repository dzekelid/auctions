swagger: "2.0"
x-collection-name: IEX
x-complete: 1
info:
  title: IEX
  description: the-iex-api-is-a-set-of-services-designed-for-developers-and-engineers--it-can-be-used-to-build-highquality-apps-and-services--were-always-working-to-improve-the-iex-api--please-check-back-for-enhancements-and-improvements-
  termsOfService: https://iextrading.com/api-terms/
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: api.iextrading.com
basePath: /1.0
paths:
  /deep/auction:
    get:
      summary: Auction
      description: For an example of an app that&rsquo;s using stats, see our IEX
        mobile app.
      operationId: auction
      x-api-path-slug: deepauction-get
      parameters:
      - in: query
        name: symbols
        description: Parameter is required Value needs to be a comma-separated list
          of symbols (i
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Auctions