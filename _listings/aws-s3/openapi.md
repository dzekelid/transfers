swagger: "2.0"
x-collection-name: AWS S3
x-complete: 1
info:
  title: No Title
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?accelerate:
    get:
      summary: GET Bucket accelerate
      description: This implementation of the GET operation uses the acceleratesubresource
        to return the Transfer Acceleration state of a bucket, which is eitherEnabled
        or Suspended
      operationId: get-bucket-accelerate
      x-api-path-slug: accelerate-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Accelerate
    put:
      summary: PUT Bucket accelerate
      description: This implementation of the PUT operation uses the acceleratesubresource
        to set the Transfer Acceleration state of an existing bucket
      operationId: put-bucket-accelerate
      x-api-path-slug: accelerate-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Accelerate