---
swagger: "2.0"
x-collection-name: Google Cloud Storage
x-complete: 0
info:
  title: Google Cloud Storage Stop Watching Channel
  version: 1.0.0
  description: Stop watching resources through this channel
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /channels/stop:
    post:
      summary: Stop Watching Channel
      description: Stop watching resources through this channel
      operationId: storage.channels.stop
      x-api-path-slug: channelsstop-post
      parameters:
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Channel
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