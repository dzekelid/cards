---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Views Create a new instance of the Cards and persist it.
  version: 1.0.0
  description: Create a new instance of the cards and persist it..
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /decks/{id}/cards:
    get:
      summary: Queries cards of Deck.
      description: Queries cards of deck..
      operationId: getDecksCards
      x-api-path-slug: decksidcards-get
      parameters:
      - in: query
        name: filter
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Queries
      - Cards
      - Of
      - Deck
  /decks/{id}/cards/count:
    get:
      summary: Counts cards of Deck.
      description: Counts cards of deck..
      operationId: getDecksCardsCount
      x-api-path-slug: decksidcardscount-get
      parameters:
      - in: path
        name: id
        description: PersistedModel id
      - in: query
        name: where
        description: Criteria to match Deck instances
      responses:
        200:
          description: OK
      tags:
      - Counts
      - Cards
      - Of
      - Deck
  /decks/{id}/cards/add:
    post:
      summary: Add Cards to Deck
      description: Add cards to deck.
      operationId: postDecksCardsAdd
      x-api-path-slug: decksidcardsadd-post
      parameters:
      - in: body
        name: cardIds
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Cards
      - To
      - Deck
  /decks/{id}/cards/remove:
    post:
      summary: Remove Cards from Deck
      description: Remove cards from deck.
      operationId: postDecksCardsRemove
      x-api-path-slug: decksidcardsremove-post
      parameters:
      - in: body
        name: cardIds
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Cards
      - From
      - Deck
  /decks/bulkCreateCardsAndDecks:
    post:
      summary: Bulk create decks and cards
      description: Bulk create decks and cards.
      operationId: postDecksBulkcreatecardsanddecks
      x-api-path-slug: decksbulkcreatecardsanddecks-post
      parameters:
      - in: body
        name: decks
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Create
      - Decks
      - Cards
  /cards:
    post:
      summary: Create a new instance of the Cards and persist it.
      description: Create a new instance of the cards and persist it..
      operationId: postCards
      x-api-path-slug: cards-post
      parameters:
      - in: body
        name: data
        description: Card instance data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Instance
      - Of
      - Cards
      - Persist
      - It
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