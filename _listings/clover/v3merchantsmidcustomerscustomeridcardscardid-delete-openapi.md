---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Delete a customer card
  version: 1.0.0
  description: Delete a customer card.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/customers/{customerId}/cards:
    post:
      summary: Create a credit/debit card entry for a customer
      description: Create a credit/debit card entry for a customer.
      operationId: DelegatedCreateCustomerCard
      x-api-path-slug: v3merchantsmidcustomerscustomeridcards-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Cards
  /v3/merchants/{mId}/customers/{customerId}/cards/{cardId}:
    post:
      summary: Update a credit/debit card record for a customer
      description: Update a credit/debit card record for a customer.
      operationId: DelegatedUpdateCustomerCard
      x-api-path-slug: v3merchantsmidcustomerscustomeridcardscardid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: cardId
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Cards
      - CardId
    delete:
      summary: Delete a customer card
      description: Delete a customer card.
      operationId: DelegatedDeleteCustomerCard
      x-api-path-slug: v3merchantsmidcustomerscustomeridcardscardid-delete
      parameters:
      - in: path
        name: cardId
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Cards
      - CardId
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