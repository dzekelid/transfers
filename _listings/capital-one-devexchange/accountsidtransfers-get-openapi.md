---
swagger: "2.0"
x-collection-name: Capital One DevExchange
x-complete: 0
info:
  title: Capital One DevExchange Get all transfers
  description: Returns the transfers that you are involved in.
  version: 1.0.0
host: api.reimaginebanking.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/transfers:
    get:
      summary: Get all transfers
      description: Returns the transfers that you are involved in.
      operationId: returns-the-transfers-that-you-are-involved-in
      x-api-path-slug: accountsidtransfers-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the transfer
      - in: query
        name: type
        description: When param is empty, will return transfers associated with account
          where account is payer AND payee
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
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