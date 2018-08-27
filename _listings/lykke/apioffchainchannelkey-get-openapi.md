---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Get API Offchain Channelkey
  version: 1.0.0
  description: Get api offchain channelkey.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/offchain/channelkey:
    get:
      summary: Get API Offchain Channelkey
      description: Get api offchain channelkey.
      operationId: ApiOffchainChannelkeyGet
      x-api-path-slug: apioffchainchannelkey-get
      parameters:
      - in: query
        name: asset
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Channelkey
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