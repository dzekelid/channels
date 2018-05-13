---
swagger: "2.0"
info:
  title: Google Adsense API Delete Custom Channel
  version: 1.0.0
  description: Delete a specific custom channel from the host AdSense account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /adclients/{adClientId}/customchannels/{customChannelId}:
    delete:
      summary: Delete Custom Channel
      description: Delete a specific custom channel from the host AdSense account
      operationId: adsensehost.customchannels.delete
      parameters:
      - in: path
        name: adClientId
        description: Ad client from which to delete the custom channel
      - in: path
        name: customChannelId
        description: Custom channel to delete
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