---
swagger: "2.0"
x-collection-name: Akeneo
x-complete: 0
info:
  title: Akeneo PIM API channel (2.x only)
  description: Channel (2.x only).
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/channels:
    get:
      summary: channels
      description: Channels.
      operationId: RestV1ChannelsGet
      x-api-path-slug: restv1channels-get
      responses:
        200:
          description: OK
      tags:
      - Channels
    patch:
      summary: channels (2.x only)
      description: Channels (2.x only).
      operationId: RestV1ChannelsPatch
      x-api-path-slug: restv1channels-patch
      parameters:
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
      - Channels
      - (2
      - X
      - Only)
    post:
      summary: channel (2.x only)
      description: Assuming that there is no "new_channel" already existing
      operationId: RestV1ChannelsPost
      x-api-path-slug: restv1channels-post
      parameters:
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
      - Channel
      - (2
      - X
      - Only)
  /rest/v1/channels/ecommerce:
    get:
      summary: channel
      description: Assuming that the given code is the code of an existing channel
      operationId: RestV1ChannelsEcommerceGet
      x-api-path-slug: restv1channelsecommerce-get
      responses:
        200:
          description: OK
      tags:
      - Channel
  /rest/v1/channels/my_new_channel_3:
    patch:
      summary: channel (2.x only)
      description: Channel (2.x only).
      operationId: RestV1ChannelsMyNewChannel3Patch
      x-api-path-slug: restv1channelsmy-new-channel-3-patch
      parameters:
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
      - Channel
      - (2
      - X
      - Only)
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