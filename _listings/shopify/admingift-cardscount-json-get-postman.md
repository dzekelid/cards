{
  "info": {
    "name": "Shopify Retrieve a count of all gift cards",
    "_postman_id": "a0550b19-6538-4577-8322-18f00110d41e",
    "description": "Retrieve a count of all gift cards.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "0e0a4ce8-9ac5-48ab-8609-3fe2f021d465",
          "name": "getAdminGiftCards61466894.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/gift_cards/61466894.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
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
            "description": "Show a specific gift card's details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f1472b9-9d4c-4ceb-b1f9-bc2a8952a730"
            }
          ]
        },
        {
          "id": "b6d5aed4-41e6-47f5-b864-8ba4412a7aa0",
          "name": "getAdminGiftCardsCount.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/gift_cards/count.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
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
            "description": "Retrieve a count of all gift cards."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b264afed-5543-4b68-a00b-912c3fb9c990"
            }
          ]
        }
      ]
    }
  ]
}