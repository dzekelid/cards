swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
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