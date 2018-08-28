---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 0
info:
  title: HitBTC Transfer Amount To Trading
  description: Transfer amount to trading.
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