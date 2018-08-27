---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Create a payment card with predefined ID
  description: ""
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /payment-cards:
    get:
      summary: Retrieve a list of Payment Cards
      description: Retrieve a list of Payments Cards
      operationId: payment_cards.get
      x-api-path-slug: paymentcards-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Payment
      - Cards
    post:
      summary: Create a Payment Card
      description: Create a Payment Card
      operationId: payment_cards.post
      x-api-path-slug: paymentcards-post
      parameters:
      - in: body
        name: body
        description: PaymentCard resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Card
  /payment-cards/{id}:
    patch:
      summary: Update a payment card's cvv value with predefined ID
      description: Update a payment card's cvv value with predefined identifier string
      operationId: payment_cards.id.patch
      x-api-path-slug: paymentcardsid-patch
      parameters:
      - in: body
        name: body
        description: Payment card
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Cards
      - Cvv
      - Value
      - Predefined
      - ID
    get:
      summary: Retrieve a Payment Card
      description: Retrieve a Payment Card with specified identifier string
      operationId: payment_cards.id.get
      x-api-path-slug: paymentcardsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Payment
      - Card
    put:
      summary: Create a payment card with predefined ID
      description: ""
      operationId: payment_cards.id.put
      x-api-path-slug: paymentcardsid-put
      parameters:
      - in: body
        name: body
        description: Payment card
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Card
      - Predefined
      - ID
  /payment-cards-migrations:
    get:
      summary: Retrieve a list of payment cards ready for migration
      description: Retrieve a list of payment cards ready for migration
      operationId: retrieve-a-list-of-payment-cards-ready-for-migration
      x-api-path-slug: paymentcardsmigrations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Payment
      - Cards
      - Readymigration
  /payment-cards-migrations/migrate:
    post:
      summary: Migrate payment cards to another gateway account
      description: Migrate payment cards to another gateway account
      operationId: migrate-payment-cards-to-another-gateway-account
      x-api-path-slug: paymentcardsmigrationsmigrate-post
      parameters:
      - in: body
        name: body
        description: Payment card migration attributes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Migrate
      - Payment
      - Cards
      - To
      - Another
      - Gateway
      - Account
  /payment-cards/{id}/authorization:
    post:
      summary: Authorize a Payment Card
      description: Authorize a Payment Card
      operationId: payment_cards.id.authorization.post
      x-api-path-slug: paymentcardsidauthorization-post
      parameters:
      - in: body
        name: body
        description: Payment Card resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Authorize
      - Payment
      - Card
  /payment-cards/{id}/deactivation:
    post:
      summary: Deactivate a Payment Card
      description: Deactivate a Payment Card
      operationId: payment_cards.id.deactivation.post
      x-api-path-slug: paymentcardsiddeactivation-post
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Payment
      - Card
  /payment-cards/{id}/matched-rules:
    get:
      summary: Get matched rules for the payment card
      description: Get matched rules for the payment card
      operationId: payment_cards.id.matched_rules.get
      x-api-path-slug: paymentcardsidmatchedrules-get
      responses:
        200:
          description: OK
      tags:
      - Matched
      - Rulesthe
      - Payment
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