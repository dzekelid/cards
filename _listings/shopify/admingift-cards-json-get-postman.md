{
  "info": {
    "name": "Shopify Get a list of all gift cards",
    "_postman_id": "da939a70-a7c2-48d3-816f-594c1aa3ef61",
    "description": "Get a list of all gift cards.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "f2844e4e-577c-411a-8183-dff139a9d0a1",
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
              "id": "734e57f4-5a0c-4905-bd7c-eefe25debfa0"
            }
          ]
        },
        {
          "id": "9fe2194c-2f71-49ee-93ec-a95c58a8f35f",
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
              "id": "579ebbd6-f69b-4823-96e1-0d71686a92a1"
            }
          ]
        },
        {
          "id": "544deca8-bb5a-4a41-944c-b4dc4a602882",
          "name": "getAdminGiftCards.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/gift_cards.json",
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
            "description": "Get a list of all gift cards."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65bfb578-d102-48b0-8bf4-0ae49f127308"
            }
          ]
        }
      ]
    }
  ]
}