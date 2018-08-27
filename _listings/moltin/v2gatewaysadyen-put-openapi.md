---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Adyen - Card Update
  description: This endpoint allows you to pay for an order using Braintree and a
    users credit card.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/gateways/adyen:
    put:
      summary: Adyen - Card Update
      description: This endpoint allows you to pay for an order using Braintree and
        a users credit card.
      operationId: V2GatewaysAdyenPut
      x-api-path-slug: v2gatewaysadyen-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Adyen
      - '-'
      - Card
  /v2/orders/{ORDER_ID}/transactions/{TRANSACTION_ID}/capture:
    put:
      summary: Stripe - Card Update
      description: This endpoint allows you to pay for an order using Braintree and
        a users credit card.
      operationId: V2OrdersTransactionsCaptureByORDERIDAndTRANSACTIONIDPut
      x-api-path-slug: v2ordersorder-idtransactionstransaction-idcapture-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: ORDER_ID
      - in: path
        name: TRANSACTION_ID
      responses:
        200:
          description: Successful response
      tags:
      - Stripe
      - '-'
      - Card
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