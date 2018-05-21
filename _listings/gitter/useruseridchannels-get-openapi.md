---
swagger: "2.0"
x-collection-name: Gitter
x-complete: 0
info:
  title: Gitter API Get User Channels
  version: 1.0.0
  description: List of Gitter channels nested under the current user.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/:userId/channels:
    get:
      summary: Get User Channels
      description: List of Gitter channels nested under the current user.
      operationId: getUserChannels
      x-api-path-slug: useruseridchannels-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Channels
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