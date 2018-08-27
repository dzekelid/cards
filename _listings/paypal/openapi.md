swagger: "2.0"
x-collection-name: PayPal
x-complete: 1
info:
  title: PayPal (Sandbox)
  description: bring-payments-to-apps-mobile-and-social-with-adaptive-payments-bsandbox-api-b
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /AdaptiveAccounts/AddPaymentCard:
    post:
      summary: Add Payment Card
      description: The AddPaymentCard API operation lets your application set up credit
        cards as funding sources for PayPal accounts.
      operationId: AdaptiveAccounts.AddPaymentCard.post
      x-api-path-slug: adaptiveaccountsaddpaymentcard-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Credit Card