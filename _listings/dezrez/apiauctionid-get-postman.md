{
  "info": {
    "name": "Dezrez Get an auction by its id.",
    "_postman_id": "49d53086-7426-40f5-b0ed-8b32f6bb7ca2",
    "description": "Get an auction by its id..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auction",
      "item": [
        {
          "id": "4bfd19d0-37ae-4638-9b8c-48b5e36aefd7",
          "name": "Auction_GetByid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/auction/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get an auction by its id.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28ef182e-8b91-4524-accb-a4114941476d"
            }
          ]
        }
      ]
    }
  ]
}