---
swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 0
info:
  title: AWS Directory Service API Remove Tags From Resource
  version: 1.0.0
  description: Removes tags from a directory.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes tags from a directory.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceId
        description: Identifier (ID) of the directory from which to remove the tag
        type: string
      - in: query
        name: TagKeys
        description: The tag key (name) of the tag to be removed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
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