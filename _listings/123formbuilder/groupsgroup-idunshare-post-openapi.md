---
swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 0
info:
  title: 123FormBuilder Unshare a group from a user
  version: 1.0.0
  description: This may not be available for your account. It is specific to certain
    users.
host: api.123contactform.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{group_id}/unshare:
    post:
      summary: Unshare a group from a user
      description: This may not be available for your account. It is specific to certain
        users.
      operationId: this-may-not-be-available-for-your-account-it-is-specific-to-certain-users
      x-api-path-slug: groupsgroup-idunshare-post
      parameters:
      - in: path
        name: group_id
        description: The ID of the group you want to unshare
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: subuser_email
        description: The username from whom you want to unshare the group
      - in: formData
        name: subuser_id
        description: The ID of the subuser from whom you want to unshare the group
      responses:
        200:
          description: OK
      tags:
      - Unshare
      - Group
      - From
      - User
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