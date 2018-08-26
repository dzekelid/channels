---
swagger: "2.0"
x-collection-name: Google Apps Admin SDK
x-complete: 1
info:
  title: Google Apps Admin SDK Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/reports_v1/channels/stop:
    post:
      summary: Stop Watching Resource
      description: Stop watching resources through this channel
      operationId: admin.channels.stop
      x-api-path-slug: adminreports-v1channelsstop-post
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