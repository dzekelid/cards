---
swagger: "2.0"
x-collection-name: PayJunction
x-complete: 0
info:
  title: PayJunction Put Customers Vaults Card Vault
  description: /customers/{customerid}/vaults/{vaultid} (card).
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customers/{customerId}/vaults/{cardVault}:
    put:
      summary: Put Customers Vaults Card Vault
      description: /customers/{customerid}/vaults/{vaultid} (card).
      operationId: CustomersVaultsByCustomerIdAndCardVaultPut
      x-api-path-slug: customerscustomeridvaultscardvault-put
      parameters:
      - in: formData
        name: address
      - in: formData
        name: addressId
      - in: formData
        name: cardExpMonth
        description: 1-12
      - in: formData
        name: cardExpYear
        description: YYYY, YY
      - in: path
        name: cardVault
      - in: formData
        name: city
      - in: path
        name: customerId
      - in: formData
        name: state
      - in: header
        name: X-PJ-Application-Key
      - in: formData
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Vaults
      - Card
      - Vault
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