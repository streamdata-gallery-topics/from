---
swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 0
info:
  title: BigCommerce Add a video to a product using a video ID from Youtube
  description: Creates an video on a product using a video ID from Youtube
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store_hash}/v3/catalog/products/{id}/videos:
    post:
      summary: Add a video to a product using a video ID from Youtube
      description: Creates an video on a product using a video ID from Youtube
      operationId: V3CatalogProductsVideosByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogproductsidvideos-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Video
      - To
      - Product
      - Using
      - Video
      - ID
      - From
      - Youtube
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