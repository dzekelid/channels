---
swagger: "2.0"
x-collection-name: Gitter
x-complete: 1
info:
  title: No Title
  version: 1.0.0
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
---