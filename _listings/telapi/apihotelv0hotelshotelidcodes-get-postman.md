{
  "info": {
    "name": "hetras Hotel API Version 0 Get a list of codes for the specified hotel either filtered by type or code.",
    "_postman_id": "854c1fcc-7bb2-4ba1-95f8-e2df9ded14aa",
    "description": "With this call you can find codes for a hotel by type or code. By default and without any filter criteria\r\n            defined it will return you all available codes.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Codesthe",
      "item": [
        {
          "id": "b423298a-4d23-49b0-a91f-4a69d3a0c292",
          "name": "Codes_GetCodes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.hetras-certification.net",
              "path": [
                "api/hotel/v0/hotels/:hotelId/codes"
              ],
              "query": [
                {
                  "key": "code",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "hotelId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "App-Id",
                "value": "{}",
                "description": "Application identifier",
                "disabled": false
              },
              {
                "key": "App-Key",
                "value": "{}",
                "description": "Application key",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "With this call you can find codes for a hotel by type or code. By default and without any filter criteria\r\n            defined it will return you all available codes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "345db0cf-65b7-43ef-9eca-f21b6cd74a1f"
            }
          ]
        }
      ]
    }
  ]
}