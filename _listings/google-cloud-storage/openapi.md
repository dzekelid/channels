---
swagger: "2.0"
x-collection-name: Google Cloud Storage
x-complete: 1
info:
  title: Google Cloud Storage
  version: 1.0.0
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
---