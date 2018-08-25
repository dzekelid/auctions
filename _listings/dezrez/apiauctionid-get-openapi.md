---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get an auction by its id.
  version: 1.0.0
  description: Get an auction by its id..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/auction/{id}:
    get:
      summary: Get an auction by its id.
      description: Get an auction by its id..
      operationId: Auction_GetByid
      x-api-path-slug: apiauctionid-get
      parameters:
      - in: path
        name: id
        description: The id of the auction to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Auction
      - By
      - Its
      - Id
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