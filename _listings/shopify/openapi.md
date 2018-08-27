swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/gift_cards/61466894.json:
    get:
      summary: Show a specific gift card's details
      description: Show a specific gift card's details.
      operationId: getAdminGiftCards61466894.json
      x-api-path-slug: admingift-cards61466894-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Show
      - Specific
      - Gift
      - Cards
      - Details
  /admin/gift_cards/count.json:
    get:
      summary: Retrieve a count of all gift cards
      description: Retrieve a count of all gift cards.
      operationId: getAdminGiftCardsCount.json
      x-api-path-slug: admingift-cardscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Count
      - Gift
      - Cards
  /admin/gift_cards.json:
    get:
      summary: Get a list of all gift cards
      description: Get a list of all gift cards.
      operationId: getAdminGiftCards.json
      x-api-path-slug: admingift-cards-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Gift
      - Cards
    post:
      summary: Create a new gift card with an automatically generated code
      description: Create a new gift card with an automatically generated code.
      operationId: postAdminGiftCards.json
      x-api-path-slug: admingift-cards-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Gift
      - Card
      - Automatically
      - Generated
      - Code
  /admin/gift_cards/search.json:
    get:
      summary: Get all gift cards that matches the query
      description: Get all gift cards that matches the query.
      operationId: getAdminGiftCardsSearch.json
      x-api-path-slug: admingift-cardssearch-json-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: query
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Gift
      - Cards
      - That
      - Matches
      - Query
  /admin/gift_cards/61810574/disable.json:
    post:
      summary: Disable a gift card
      description: Disable a gift card.
      operationId: postAdminGiftCards61810574Disable.json
      x-api-path-slug: admingift-cards61810574disable-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Disable
      - Gift
      - Card
  /admin/gift_cards/61810574.json:
    put:
      summary: Update the expiry date of a gift card
      description: Update the expiry date of a gift card.
      operationId: putAdminGiftCards61810574.json
      x-api-path-slug: admingift-cards61810574-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Expiry
      - Date
      - Gift
      - Card