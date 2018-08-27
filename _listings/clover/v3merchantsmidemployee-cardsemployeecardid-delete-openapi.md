---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Delete employee cards
  version: 1.0.0
  description: .Delete employee cards
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
  /v3/merchants/{mId}/employee_cards:
    post:
      summary: Add employee cards
      description: .Add employee cards
      operationId: CreateOrUpdateEmployeeCard
      x-api-path-slug: v3merchantsmidemployee-cards-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employee
      - Cards
    get:
      summary: Get employee cards
      description: .Get employee cards
      operationId: GetEmployeeCards
      x-api-path-slug: v3merchantsmidemployee-cards-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [id, employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employee
      - Cards
  /v3/merchants/{mId}/employee_cards/{employeeCardId}:
    get:
      summary: Get employee card
      description: .Get employee card
      operationId: GetEmployeeCard
      x-api-path-slug: v3merchantsmidemployee-cardsemployeecardid-get
      parameters:
      - in: path
        name: employeeCardId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employee
      - Cards
      - EmployeeCardId
    delete:
      summary: Delete employee cards
      description: .Delete employee cards
      operationId: DeleteEmployeeCard
      x-api-path-slug: v3merchantsmidemployee-cardsemployeecardid-delete
      parameters:
      - in: path
        name: employeeCardId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employee
      - Cards
      - EmployeeCardId
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