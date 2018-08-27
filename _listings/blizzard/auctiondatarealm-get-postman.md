{
  "info": {
    "name": "World of Warcraft Get Auction Data Realm",
    "_postman_id": "953e9f9a-d8a2-410e-a092-4b87a68f6674",
    "description": "Provides a per-realm list of recently generated auction house data dumps. The current auctions data is represented as JSON structures containing auction data for the tree auctions houses available on each realm.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auction",
      "item": [
        {
          "id": "c4dfeaab-bc1d-4774-8f7e-b6608dafebb5",
          "name": "getAuctionDataRealm",
          "request": {
            "url": {
              "protocol": "http",
              "host": "us.battle.net",
              "path": [
                "api",
                "wow",
                "auction/data/:realm"
              ],
              "variable": [
                {
                  "id": "realm",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides a per-realm list of recently generated auction house data dumps. The current auctions data is represented as JSON structures containing auction data for the tree auctions houses available on each realm."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8378c879-0915-4c43-ab87-c2f1b2952b9c"
            }
          ]
        }
      ]
    }
  ]
}