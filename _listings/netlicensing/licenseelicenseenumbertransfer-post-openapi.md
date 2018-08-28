---
swagger: "2.0"
x-collection-name: NetLicensing
x-complete: 0
info:
  title: NetLicensing Transfer licenses
  description: Licenses transfer between licensees
  termsOfService: https://www.labs64.com/legal/terms-of-service/netlicensing
  version: 2.x
host: go.netlicensing.io
basePath: /core/v2/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /licensee/{licenseeNumber}/transfer:
    post:
      summary: Transfer licenses
      description: Licenses transfer between licensees
      operationId: transferLicenses
      x-api-path-slug: licenseelicenseenumbertransfer-post
      parameters:
      - in: path
        name: licenseeNumber
        description: Licensee number with a maximum length of 1000 characters
      - in: formData
        name: sourceLicenseeNumber
        description: Licensee number which licenses to be transferred
      responses:
        200:
          description: OK
      tags:
      - Licensee
      - LicenseeNumber
      - Transfer
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