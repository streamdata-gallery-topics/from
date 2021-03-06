---
swagger: "2.0"
x-collection-name: Docsmore
x-complete: 0
info:
  title: Docsmore Fetch All Documents from Your Team Catalogue
  description: By design, the authenticated user can only view the files that are
    either created by them or shared with them. Make sure user has at least read permission
    to view the catalogue.
  version: "1.0"
host: api.docsmore.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/getworkflowlink:
    post:
      summary: Get Workflow Link
      description: |-
        This is the most popular use of Docsmore API. From your connected app, you can launch workflow and obtain the unique link for immediate launch or later on. You can also supply data in flat json format that can be used inside the document for pre-fill purpose saving your customer time.

        Please make sure you pay close attention to the requirement for this API call as there are several aspects of it as required parameters.
      operationId: ApiGetworkflowlinkPost
      x-api-path-slug: apigetworkflowlink-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Link
  /api/dmcatalogue:
    post:
      summary: Fetch All Documents from Your Team Catalogue
      description: By design, the authenticated user can only view the files that
        are either created by them or shared with them. Make sure user has at least
        read permission to view the catalogue.
      operationId: ApiDmcataloguePost
      x-api-path-slug: apidmcatalogue-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: items
      - in: query
        name: page
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - ""
      - Documents
      - From
      - Your
      - Team
      - Catalogue
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