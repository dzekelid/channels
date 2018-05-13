---
swagger: "2.0"
info:
  title: Google Adsense API Add URL Channel
  version: 1.0.0
  description: Add a new URL channel to the host AdSense account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /adclients/{adClientId}/urlchannels:
    post:
      summary: Add URL Channel
      description: Add a new URL channel to the host AdSense account
      operationId: adsensehost.urlchannels.insert
      parameters:
      - in: path
        name: adClientId
        description: Ad client to which the new URL channel will be added
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - advertising
      - channels
definitions: []
x-collection-name: Google Adsense
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