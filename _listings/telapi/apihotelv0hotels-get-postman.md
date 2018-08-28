{
  "info": {
    "name": "hetras Hotel API Version 0 Get a list of all the hotels of a chain your application has access to.",
    "_postman_id": "df0789a5-d5ca-417d-ba84-c44a7e030b0c",
    "description": "Get a list of all the hotels of a chain your application has access to..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "8bdf20e7-c579-48ae-bee3-1448219241ed",
      "name": "Hotels_GetHotels",
      "request": {
        "url": "http://api.hetras-certification.net/api/hotel/v0/hotels",
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
        "description": "Get a list of all the hotels of a chain your application has access to.."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "cbe6f54d-a6f9-4d2f-a2b0-41ef11a7844d"
        }
      ]
    }
  ]
}