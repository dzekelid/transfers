---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 0
info:
  title: AWS Internet of Things API Accept Certificate Transfer
  version: 1.0.0
  description: Accepts a pending certificate transfer.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=TransferCertificate:
    get:
      summary: Transfer Certificate
      description: Transfers the specified certificate to the specified AWS account.
      operationId: transferCertificate
      x-api-path-slug: actiontransfercertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      - in: query
        name: targetAwsAccount
        description: The AWS account
        type: string
      - in: query
        name: transferMessage
        description: The transfer message
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=AcceptCertificateTransfer:
    get:
      summary: Accept Certificate Transfer
      description: Accepts a pending certificate transfer.
      operationId: acceptCertificateTransfer
      x-api-path-slug: actionacceptcertificatetransfer-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      - in: query
        name: setAsActive
        description: Specifies whether the certificate is active
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificate Transfers
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