---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get a list of channels by ids
  description: |-
    Get a list of public channels on a team by id.
    ##### Permissions
    `view_team` for the team the channels are on.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams/{team_id}/channels/ids:
    post:
      summary: Get a list of channels by ids
      description: |-
        Get a list of public channels on a team by id.
        ##### Permissions
        `view_team` for the team the channels are on.
      operationId: get-a-list-of-public-channels-on-a-team-by-id-permissionsview-team-for-the-team-the-channels-are-on
      x-api-path-slug: teamsteam-idchannelsids-post
      parameters:
      - in: body
        name: body
        description: List of channel ids
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Channels
      - By
      - Ids
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