swagger: "2.0"
x-collection-name: NetLicensing
x-complete: 1
info:
  title: NetLicensing
  description: the-labs64-netlicensing-restful-api-gives-you-access-to-netlicensings-core-features--you-authenticate-to-the-netlicensing-api-by-providing-your-account-credentials-or-simply-use-our-demo-account--find-out-more-about-labs64-netlicensing-at-netlicensing-io-
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