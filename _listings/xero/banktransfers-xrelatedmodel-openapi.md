---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting X-related-model Banks Transfers
  description: X-related-model banktransfers.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /BankTransfers:
    get:
      summary: Get Banks Transfers
      description: Get banktransfers.
      operationId: getBanktransfers
      x-api-path-slug: banktransfers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
    put:
      summary: Put Banks Transfers
      description: Put banktransfers.
      operationId: putBanktransfers
      x-api-path-slug: banktransfers-put
      parameters:
      - in: body
        name: BankTransfers
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
    x-related-model:
      summary: X-related-model Banks Transfers
      description: X-related-model banktransfers.
      operationId: x-related-modelBanktransfers
      x-api-path-slug: banktransfers-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
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