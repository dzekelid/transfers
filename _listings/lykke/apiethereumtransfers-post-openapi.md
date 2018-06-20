---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Ethereum Transfers
  version: 1.0.0
  description: Add api ethereum transfers.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Ethereum/transfers:
    get:
      summary: Get API Ethereum Transfers
      description: Get api ethereum transfers.
      operationId: ApiEthereumTransfersGet
      x-api-path-slug: apiethereumtransfers-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Transfers
    post:
      summary: Add API Ethereum Transfers
      description: Add api ethereum transfers.
      operationId: ApiEthereumTransfersPost
      x-api-path-slug: apiethereumtransfers-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: operations
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Transfers
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