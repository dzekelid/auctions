---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Delete a custom auction milestone
  version: 1.0.0
  description: Delete a custom auction milestone.
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
  /api/auction/saveauction:
    put:
      summary: Save or update an auction.
      description: Save or update an auction..
      operationId: Auction_SaveAuctionByauction
      x-api-path-slug: apiauctionsaveauction-put
      parameters:
      - in: body
        name: auction
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Update
      - Auction
  /api/auction/{id}/confirmlots:
    post:
      summary: To confirm or unconfirm a list of lots for the auction
      description: To confirm or unconfirm a list of lots for the auction.
      operationId: Auction_ConfirmLotsByidByconfirmLotsDataContract
      x-api-path-slug: apiauctionidconfirmlots-post
      parameters:
      - in: body
        name: confirmLotsDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - To
      - Confirm
      - Unconfirm
      - List
      - Of
      - Lotsthe
      - Auction
  /api/auction/{id}/withdrawlots:
    post:
      summary: To withdraw a list of properties from the auction
      description: To withdraw a list of properties from the auction.
      operationId: Auction_WithdrawLotsByidBywithdrawLotsDataContract
      x-api-path-slug: apiauctionidwithdrawlots-post
      parameters:
      - in: path
        name: id
        description: The auction ID
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: withdrawLotsDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Withdraw
      - List
      - Of
      - Properties
      - From
      - Auction
  /api/auction/{id}/postponelots:
    post:
      summary: To postpone a list of lots for the auction
      description: To postpone a list of lots for the auction.
      operationId: Auction_PostponeLotsByidBypostponeLotsDataContract
      x-api-path-slug: apiauctionidpostponelots-post
      parameters:
      - in: path
        name: id
        description: The auction ID
      - in: body
        name: postponeLotsDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - To
      - Postpone
      - List
      - Of
      - Lotsthe
      - Auction
  /api/auction/savecontact:
    post:
      summary: Add a new contact to the given auction Role or edit an existing contact
      description: Add a new contact to the given auction role or edit an existing
        contact.
      operationId: Auction_SaveAuctionContactBysaveContactDataContract
      x-api-path-slug: apiauctionsavecontact-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: saveContactDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Contact
      - To
      - Given
      - Auction
      - Role
      - Edit
      - Existing
      - Contact
  /api/auction/removecontact:
    post:
      summary: Remove an existing auction contact from the auction role
      description: Remove an existing auction contact from the auction role.
      operationId: Auction_RemoveAuctionContactByremoveContactDataContract
      x-api-path-slug: apiauctionremovecontact-post
      parameters:
      - in: body
        name: removeContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Existing
      - Auction
      - Contact
      - From
      - Auction
      - Role
  /api/auction/{id}/recordbid:
    post:
      summary: Record auction bid details
      description: Record auction bid details.
      operationId: Auction_ReccordAuctionBidByidBydataContactDataContract
      x-api-path-slug: apiauctionidrecordbid-post
      parameters:
      - in: body
        name: dataContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Auction
      - Bid
      - Details
  /api/role/auction/{id}/setrequestedlotnumber:
    post:
      summary: Set the requested lot number for a property auction role.
      description: Set the requested lot number for a property auction role..
      operationId: AuctionRole_SetRequestedLotNumberByidBylotNumber
      x-api-path-slug: apiroleauctionidsetrequestedlotnumber-post
      parameters:
      - in: path
        name: id
        description: the id of the role
      - in: query
        name: lotNumber
        description: the requested lot number
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Requested
      - Lot
      - Numbera
      - Property
      - Auction
      - Role
  /api/role/auction/{id}/setlotnumber:
    post:
      summary: Set the lot number for a property auction role.
      description: Set the lot number for a property auction role..
      operationId: AuctionRole_SetLotNumberByidByauctionIdBylotNumber
      x-api-path-slug: apiroleauctionidsetlotnumber-post
      parameters:
      - in: query
        name: auctionId
        description: the id of the auction to set the lot number for
      - in: path
        name: id
        description: the id of the role
      - in: query
        name: lotNumber
        description: the lot number
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Lot
      - Numbera
      - Property
      - Auction
      - Role
  /api/role/auction/{id}/addtoauction:
    post:
      summary: Add a property auction role to an existing auction
      description: Add a property auction role to an existing auction.
      operationId: AuctionRole_AddToAuctionByidByauctionIdBylotNumber
      x-api-path-slug: apiroleauctionidaddtoauction-post
      parameters:
      - in: query
        name: auctionId
        description: the id of the auction to add the role to
      - in: path
        name: id
        description: the id of the role
      - in: query
        name: lotNumber
        description: the lot number
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Property
      - Auction
      - Role
      - To
      - Existing
      - Auction
  /api/role/auction/{id}/removefromauction:
    post:
      summary: Add a property auction role to an existing auction
      description: Add a property auction role to an existing auction.
      operationId: AuctionRole_RemoveFromAuctionByidByremoveFromAuctionDataContract
      x-api-path-slug: apiroleauctionidremovefromauction-post
      parameters:
      - in: path
        name: id
        description: the id of the role
      - in: body
        name: removeFromAuctionDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Property
      - Auction
      - Role
      - To
      - Existing
      - Auction
  /api/role/auction/{id}/setreserve:
    post:
      summary: Set the reserve for a property auction role.
      description: Set the reserve for a property auction role..
      operationId: AuctionRole_SetReserveByidBysetReserveDataContract
      x-api-path-slug: apiroleauctionidsetreserve-post
      parameters:
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setReserveDataContract
        description: SetReserveDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Reservea
      - Property
      - Auction
      - Role
  /api/role/auction/{id}/settype:
    post:
      summary: Set the type of auction role (Commercial or Residential)
      description: Set the type of auction role (commercial or residential).
      operationId: AuctionRole_SetTypeByidByauctionRoleTypeSystemName
      x-api-path-slug: apiroleauctionidsettype-post
      parameters:
      - in: query
        name: auctionRoleTypeSystemName
        description: The auction role type
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Type
      - Of
      - Auction
      - Role
      - (Commercial
      - Residential)
  /api/role/auction/milestone/{roleId}:
    get:
      summary: Get auction role milestones
      description: Get auction role milestones.
      operationId: AuctionRole_GetRoleMilestonesByroleId
      x-api-path-slug: apiroleauctionmilestoneroleid-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Auction
      - Role
      - Milestones
    put:
      summary: Update an auction role milestone
      description: Update an auction role milestone.
      operationId: AuctionRole_SaveAuctionMilestoneByroleIdBydataContract
      x-api-path-slug: apiroleauctionmilestoneroleid-put
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Auction
      - Role
      - Milestone
    post:
      summary: Add a new auction role milestone
      description: Add a new auction role milestone.
      operationId: AuctionRole_AddAuctionMilestoneByroleIdBydataContract
      x-api-path-slug: apiroleauctionmilestoneroleid-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - New
      - Auction
      - Role
      - Milestone
  /api/role/auction/milestone/{roleId}/{milestoneId}:
    delete:
      summary: Delete a custom auction milestone
      description: Delete a custom auction milestone.
      operationId: AuctionRole_DeleteAuctionMilestoneByroleIdBymilestoneId
      x-api-path-slug: apiroleauctionmilestoneroleidmilestoneid-delete
      parameters:
      - in: path
        name: milestoneId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Auction
      - Milestone
  /api/offer/recordofferresponse:
    post:
      summary: Record a sale/auction offer response
      description: Record a sale/auction offer response.
      operationId: Offer_RecordOfferResponseByrecordOfferResponseCommand
      x-api-path-slug: apiofferrecordofferresponse-post
      parameters:
      - in: body
        name: recordOfferResponseCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Sale
      - Auction
      - Offer
      - Response
  /api/offer/recordauctionofferresponse:
    post:
      summary: Record a auction offer Response
      description: Record a auction offer response.
      operationId: Offer_RecordAuctionOfferResponseByrecordOfferResponseCommand
      x-api-path-slug: apiofferrecordauctionofferresponse-post
      parameters:
      - in: body
        name: recordOfferResponseCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Auction
      - Offer
      - Response
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