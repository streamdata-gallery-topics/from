---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Removes a fee assocation from an item, meaning the fee
    is no longer automatically applied to the item in Square Register.
  description: Removes a fee assocation from an item, meaning the fee is no longer
    automatically applied to the item in Square Register.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/me/timecards/{timecard_id}:
    delete:
      summary: Deletes a timecard. Deleted timecards are still accessible from Connect
        API endpoints, but the value of their deleted field is set to true. See Handling
        deleted timecards for more information.
      description: Deletes a timecard. Deleted timecards are still accessible from
        Connect API endpoints, but the value of their deleted field is set to true.
        See Handling deleted timecards for more information.
      operationId: DeleteTimecard
      x-api-path-slug: v1metimecardstimecard-id-delete
      parameters:
      - in: path
        name: timecard_id
        description: The ID of the timecard to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Timecard
      - ""
      - D
      - Timecards
      - Are
      - Still
      - Accessible
      - From
      - Connect
      - Endpoints
      - ""
      - But
      - Value
      - Of
      - Their
      - Deleted
      - Field
      - Is
      - Set
      - To
      - "True"
      - ""
      - See
      - Handling
      - Deleted
      - Timecardsmore
      - Information
  /v1/{location_id}/items/{item_id}/fees/{fee_id}:
    delete:
      summary: Removes a fee assocation from an item, meaning the fee is no longer
        automatically applied to the item in Square Register.
      description: Removes a fee assocation from an item, meaning the fee is no longer
        automatically applied to the item in Square Register.
      operationId: RemoveFee
      x-api-path-slug: v1location-iditemsitem-idfeesfee-id-delete
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to apply
      - in: path
        name: item_id
        description: The ID of the item to add the fee to
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Fee
      - Assocation
      - From
      - Item
      - ""
      - Meaning
      - Fee
      - Is
      - "No"
      - Longer
      - Automatically
      - Applied
      - To
      - Item
      - In
      - Square
      - Register
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