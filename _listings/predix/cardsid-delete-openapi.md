---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Views Delete a Card instance by id.
  version: 1.0.0
  description: Delete a card instance by id..
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
    get:
      summary: Find all instances of the Card matched by filter.
      description: Find all instances of the card matched by filter..
      operationId: getCards
      x-api-path-slug: cards-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields, where, include, order, offset, and limit
      responses:
        200:
          description: OK
      tags:
      - Find
      - ""
      - Instances
      - Of
      - Card
      - Matched
      - By
      - Filter
  /cards/count:
    get:
      summary: Counts cards.
      description: Counts cards..
      operationId: getCardsCount
      x-api-path-slug: cardscount-get
      parameters:
      - in: query
        name: where
        description: Criteria to match Card instances
      responses:
        200:
          description: OK
      tags:
      - Counts
      - Cards
  /cards/tags:
    get:
      summary: Get all cards by tags
      description: Get all cards by tags.
      operationId: getCardsTags
      x-api-path-slug: cardstags-get
      parameters:
      - in: query
        name: values
      responses:
        200:
          description: OK
      tags:
      - Cards
      - By
      - Tags
  /cards/{id}/tags:
    get:
      summary: Queries tags of Card.
      description: Queries tags of card..
      operationId: getCardsTags
      x-api-path-slug: cardsidtags-get
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
      - Tags
      - Of
      - Card
    post:
      summary: Creates a new instance in tags of this Card.
      description: Creates a new instance in tags of this card..
      operationId: postCardsTags
      x-api-path-slug: cardsidtags-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Instance
      - In
      - Tags
      - Of
      - This
      - Card
    delete:
      summary: Deletes all tags of this Card.
      description: Deletes all tags of this card..
      operationId: deleteCardsTags
      x-api-path-slug: cardsidtags-delete
      parameters:
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Tags
      - Of
      - This
      - Card
  /cards/{id}:
    get:
      summary: Find a Card instance by id.
      description: Find a card instance by id..
      operationId: getCards
      x-api-path-slug: cardsid-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields and include
      - in: path
        name: id
        description: Card id
      responses:
        200:
          description: OK
      tags:
      - Find
      - Card
      - Instance
      - By
      - Id
    delete:
      summary: Delete a Card instance by id.
      description: Delete a card instance by id..
      operationId: deleteCards
      x-api-path-slug: cardsid-delete
      parameters:
      - in: path
        name: id
        description: Card id
      responses:
        200:
          description: OK
      tags:
      - Card
      - Instance
      - By
      - Id
    put:
      summary: Update attributes for a Card instance and persist it.
      description: Update attributes for a card instance and persist it..
      operationId: putCards
      x-api-path-slug: cardsid-put
      parameters:
      - in: body
        name: data
        description: An object of Card property name/value pairs
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Attributesa
      - Card
      - Instance
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