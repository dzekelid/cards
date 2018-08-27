swagger: "2.0"
x-collection-name: PayJunction
x-complete: 1
info:
  title: PayJunction API Basic
  description: todo-add-description
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