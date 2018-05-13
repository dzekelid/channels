---
swagger: "2.0"
info:
  title: Google Adsense API Update Custom Channels
  version: 1.0.0
  description: Update a custom channel in the host AdSense account. This method supports
    patch semantics.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /adclients/{adClientId}/customchannels:
    patch:
      summary: Update Custom Channels
      description: Update a custom channel in the host AdSense account
      operationId: adsensehost.customchannels.patch
      parameters:
      - in: path
        name: adClientId
        description: Ad client in which the custom channel will be updated
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: customChannelId
        description: Custom channel to get
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