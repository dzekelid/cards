---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 1
info:
  title: Rebilly
  description: -introductionthe-rebilly-api-is-built-on-http---our-api-is-restful---it-has-predictableresource-urls---it-returns-http-response-codes-to-indicate-errors---it-alsoaccepts-and-returns-json-in-the-http-body---you-can-use-your-favoritehttprest-library-for-your-programming-language-to-use-rebillys-api-oryou-can-use-one-of-our-sdks-currently-available-in-phphttpsgithub-comrebillyrebillyphpand-chttpsgithub-comrebillyrebillydotnetclient--authenticationwhen-you-sign-up-for-an-account-you-are-given-your-first-api-key-you-can-generate-additional-api-keys-and-delete-api-keys-as-you-mayneed-to-rotate-your-keys-in-the-future--you-authenticate-to-therebilly-api-by-providing-your-secret-key-in-the-request-header-rebilly-offers-three-forms-of-authentication--private-key-json-web-tokens-andpublic-key--private-key-authenticates-each-request-by-searching-for-the-presenceof-an-http-header-rebapikey--jwt-authenticates-each-request-by-the-http-header-authorization--public-key-authenticates-by-the-http-header-rebauth-read-more-on-this-below-rebilly-also-offers-json-web-tokens-jwt-authentication-where-you-can-controlthe-specific-granular-permissions-and-expiration-for-that-jwt---we-call-our-resourcefor-generating-jwt-sessionstagsessions-rebilly-also-has-a-clientside-authentication-scheme-that-uses-anapiuser-and-hmacsha1-signature-only-for-the-tokens-resource-sothat-you-may-safely-create-tokens-from-the-clientside-without-compromisingyour-secret-keys-never-share-your-secret-keys--keep-them-guarded-and-secure-the-clientside-authentication-scheme-uses-one-http-header-named-rebauth--redocinject-securitydefinitions--php-sdkfor-all-php-sdk-examples-provided-in-this-spec-you-will-need-to-configure-client-you-may-do-it-like-thisphpclient--new-rebillyclient----apikey--yourapikeyhere----baseurl--httpsapi-rebilly-com
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
---