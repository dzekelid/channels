---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost API Reference
  description: -api-v4-is-stable-with-the-mattermost-server-40-release-api-v3-was-deprecated-on-january-16th-2018-and-scheduled-for-removal-in-mattermost-v50-details-heretagapiv3deprecation-looking-for-the-api-v3-reference-it-has-moved-herehttpsapimattermostcomv3
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
  /channels/{channel_id}/pinned:
    get:
      summary: Get a channels pinned posts
      description: Get a list of pinned posts for channel.
      operationId: get-a-list-of-pinned-posts-for-channel
      x-api-path-slug: channelschannel-idpinned-get
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      responses:
        200:
          description: OK
      tags:
      - Channels
      - Pinned
      - Posts
  /teams/{team_id}/channels:
    get:
      summary: Get public channels
      description: |-
        Get a page of public channels on a team based on query string parameters - page and per_page.
        ##### Permissions
        Must be authenticated and have the `list_team_channels` permission.
      operationId: get-a-page-of-public-channels-on-a-team-based-on-query-string-parameters--page-and-per-page-permissi
      x-api-path-slug: teamsteam-idchannels-get
      parameters:
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of public channels per page
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Public
      - Channels
  /teams/{team_id}/channels/deleted:
    get:
      summary: Get deleted channels
      description: |-
        Get a page of deleted channels on a team based on query string parameters - team_id, page and per_page.

        __Minimum server version__: 3.10

        ##### Permissions
        Must be authenticated and have the `manage_team` permission.
      operationId: get-a-page-of-deleted-channels-on-a-team-based-on-query-string-parameters--team-id-page-and-per-page
      x-api-path-slug: teamsteam-idchannelsdeleted-get
      parameters:
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of public channels per page
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Deleted
      - Channels
  /teams/{team_id}/channels/autocomplete:
    get:
      summary: Autocomplete channels
      description: |-
        Autocomplete public channels on a team based on the search term provided in the request URL.

        __Minimum server version__: 4.7

        ##### Permissions
        Must have the `list_team_channels` permission.
      operationId: autocomplete-public-channels-on-a-team-based-on-the-search-term-provided-in-the-request-url-minimum-
      x-api-path-slug: teamsteam-idchannelsautocomplete-get
      parameters:
      - in: query
        name: name
        description: Name or display name
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Autocomplete
      - Channels
  /teams/{team_id}/channels/search:
    post:
      summary: Search channels
      description: |-
        Search public channels on a team based on the search term provided in the request body.
        ##### Permissions
        Must have the `list_team_channels` permission.
      operationId: search-public-channels-on-a-team-based-on-the-search-term-provided-in-the-request-body-permissionsmu
      x-api-path-slug: teamsteam-idchannelssearch-post
      parameters:
      - in: body
        name: body
        description: Search criteria
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Search
      - Channels
  /users/{user_id}/teams/{team_id}/channels:
    get:
      summary: Get channels for user
      description: |-
        Get all the channels on a team for a user.
        ##### Permissions
        Logged in as the user, or have `edit_other_users` permission, and `view_team` permission for the team.
      operationId: get-all-the-channels-on-a-team-for-a-user-permissionslogged-in-as-the-user-or-have-edit-other-users-
      x-api-path-slug: usersuser-idteamsteam-idchannels-get
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Channelsuser
---