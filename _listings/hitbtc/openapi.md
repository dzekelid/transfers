swagger: "2.0"
x-collection-name: HitBTC
x-complete: 1
info:
  title: HitBTC API
  description: create-api-keys-in-your-profile-httpshitbtc-comsettingsapikeys-and-use-public-api-key-as-username-and-secret-as-password-to-authorize-
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/transfer:
    post:
      summary: Transfer Amount To Trading
      description: Transfer amount to trading.
      operationId: postAccountTransfer
      x-api-path-slug: accounttransfer-post
      parameters:
      - in: formData
        name: amount
      - in: formData
        name: currency
      - in: formData
        name: type
      responses:
        200:
          description: OK
      tags:
      - Transfer
      - Amount
      - To
      - Trading