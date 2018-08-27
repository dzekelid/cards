{
  "info": {
    "name": "Stripe Get Customers Customer Cards",
    "_postman_id": "81fa9952-05c4-4ca8-898d-6b5672b60cb3",
    "description": "Get Customers, Customer, Cards",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "customers",
      "item": [
        {
          "id": "a6e20196-81f8-4651-afd5-5a46c0eb48bb",
          "name": "getCustomersCustomerCards",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "customers/:customer/cards/:id"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "customer",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Customers, Customer, Cards"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d96665f-2c2c-48df-a6cc-25ccf7172007"
            }
          ]
        }
      ]
    }
  ]
}