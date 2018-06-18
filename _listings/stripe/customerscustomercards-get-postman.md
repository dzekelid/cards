{
  "info": {
    "name": "Stripe Get Customers Customer Cards",
    "_postman_id": "0ed5fb96-28bf-4914-a89e-8a9318ed7cc8",
    "description": "Get Customers, Customer, Cards",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "customers",
      "item": [
        {
          "id": "7a72d7f6-8225-40b2-a0a3-01b5aef6a92a",
          "name": "getCustomersCustomerCards",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "customers/:customer/cards"
              ],
              "query": [
                {
                  "key": "ending_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "starting_after",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "customer",
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
              "id": "3fe9d391-a6d7-41c6-95f3-92c49fbd522f"
            }
          ]
        }
      ]
    }
  ]
}