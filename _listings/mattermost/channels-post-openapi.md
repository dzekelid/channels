---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Create a channel
  description: |-
    Create a new channel.
    ##### Permissions
    If creating a public channel, `create_public_channel` permission is required. If creating a private channel, `create_private_channel` permission is required.
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
  /channels:
    post:
      summary: Create a channel
      description: |-
        Create a new channel.
        ##### Permissions
        If creating a public channel, `create_public_channel` permission is required. If creating a private channel, `create_private_channel` permission is required.
      operationId: create-a-new-channel-permissionsif-creating-a-public-channel-create-public-channel-permission-is-req
      x-api-path-slug: channels-post
      parameters:
      - in: body
        name: body
        description: Channel object to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Channel
  /channels/direct:
    post:
      summary: Create a direct message channel
      description: |-
        Create a new direct message channel between two users.
        ##### Permissions
        Must be one of the two users and have `create_direct_channel` permission. Having the `manage_system` permission voids the previous requirements.
      operationId: create-a-new-direct-message-channel-between-two-users-permissionsmust-be-one-of-the-two-users-and-ha
      x-api-path-slug: channelsdirect-post
      parameters:
      - in: body
        name: body
        description: The two user ids to be in the direct message
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Direct
      - Message
      - Channel
  /channels/group:
    post:
      summary: Create a group message channel
      description: |-
        Create a new group message channel to group of users. If the logged in user's id is not included in the list, it will be appended to the end.
        ##### Permissions
        Must have `create_group_channel` permission.
      operationId: create-a-new-group-message-channel-to-group-of-users-if-the-logged-in-users-id-is-not-included-in-th
      x-api-path-slug: channelsgroup-post
      parameters:
      - in: body
        name: body
        description: User ids to be in the group message channel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Group
      - Message
      - Channel
  /channels/{channel_id}:
    get:
      summary: Get a channel
      description: |-
        Get channel from the provided channel id string.
        ##### Permissions
        `read_channel` permission for the channel.
      operationId: get-channel-from-the-provided-channel-id-string-permissionsread-channel-permission-for-the-channel
      x-api-path-slug: channelschannel-id-get
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      responses:
        200:
          description: OK
      tags:
      - Channel
    put:
      summary: Update a channel
      description: |-
        Update a channel. The fields that can be updated are listed as paramters. Omitted fields will be treated as blanks.
        ##### Permissions
        If updating a public channel, `manage_public_channel_members` permission is required. If updating a private channel, `manage_private_channel_members` permission is required.
      operationId: update-a-channel-the-fields-that-can-be-updated-are-listed-as-paramters-omitted-fields-will-be-treat
      x-api-path-slug: channelschannel-id-put
      parameters:
      - in: body
        name: body
        description: Channel object to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: channel_id
        description: Channel GUID
      responses:
        200:
          description: OK
      tags:
      - Channel
    delete:
      summary: Delete a channel
      description: |-
        Soft deletes a channel, by marking the channel as deleted in the database. Soft deleted channels will not be accessible in the user interface.
        ##### Permissions
        `delete_public_channel` permission if the channel is public,
        `delete_private_channel` permission if the channel is private,
        or have `manage_system` permission.
      operationId: soft-deletes-a-channel-by-marking-the-channel-as-deleted-in-the-database-soft-deleted-channels-will-
      x-api-path-slug: channelschannel-id-delete
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      responses:
        200:
          description: OK
      tags:
      - Channel
  /channels/{channel_id}/patch:
    put:
      summary: Patch a channel
      description: |-
        Partially update a channel by providing only the fields you want to update. Omitted fields will not be updated. The fields that can be updated are defined in the request body, all other provided fields will be ignored.
        ##### Permissions
        If updating a public channel, `manage_public_channel_members` permission is required. If updating a private channel, `manage_private_channel_members` permission is required.
      operationId: partially-update-a-channel-by-providing-only-the-fields-you-want-to-update-omitted-fields-will-not-b
      x-api-path-slug: channelschannel-idpatch-put
      parameters:
      - in: body
        name: body
        description: Channel object to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: channel_id
        description: Channel GUID
      responses:
        200:
          description: OK
      tags:
      - Channel
  /channels/{channel_id}/convert:
    post:
      summary: Convert a channel from public to private
      description: |-
        Convert into private channel from the provided channel id string.

        __Minimum server version__: 4.10

        ##### Permissions
        Must have `manage_system` permission.
      operationId: convert-into-private-channel-from-the-provided-channel-id-string-minimum-server-version--410-permiss
      x-api-path-slug: channelschannel-idconvert-post
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      responses:
        200:
          description: OK
      tags:
      - Convert
      - Channel
      - From
      - Public
      - To
      - Private
  /channels/{channel_id}/restore:
    post:
      summary: Restore a channel
      description: |-
        Restore channel from the provided channel id string.

        __Minimum server version__: 3.10

        ##### Permissions
        `manage_team` permission for the team of channel.
      operationId: restore-channel-from-the-provided-channel-id-string-minimum-server-version--310-permissionsmanage-te
      x-api-path-slug: channelschannel-idrestore-post
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      responses:
        200:
          description: OK
      tags:
      - Restore
      - Channel
  /channels/{channel_id}/stats:
    get:
      summary: Get channel statistics
      description: |-
        Get statistics for a channel.
        ##### Permissions
        Must have the `read_channel` permission.
      operationId: get-statistics-for-a-channel-permissionsmust-have-the-read-channel-permission
      x-api-path-slug: channelschannel-idstats-get
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      responses:
        200:
          description: OK
      tags:
      - Channel
      - Statistics
  /teams/{team_id}/channels/name/{channel_name}:
    get:
      summary: Get a channel by name
      description: |-
        Gets channel from the provided team id and channel name strings.
        ##### Permissions
        `read_channel` permission for the channel.
      operationId: gets-channel-from-the-provided-team-id-and-channel-name-strings-permissionsread-channel-permission-f
      x-api-path-slug: teamsteam-idchannelsnamechannel-name-get
      parameters:
      - in: path
        name: channel_name
        description: Channel Name
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Channel
      - By
      - Name
  /teams/name/{team_name}/channels/name/{channel_name}:
    get:
      summary: Get a channel by name and team name
      description: |-
        Gets a channel from the provided team name and channel name strings.
        ##### Permissions
        `read_channel` permission for the channel.
      operationId: gets-a-channel-from-the-provided-team-name-and-channel-name-strings-permissionsread-channel-permissi
      x-api-path-slug: teamsnameteam-namechannelsnamechannel-name-get
      parameters:
      - in: path
        name: channel_name
        description: Channel Name
      - in: path
        name: team_name
        description: Team Name
      responses:
        200:
          description: OK
      tags:
      - Channel
      - By
      - Name
      - Team
      - Name
  /channels/{channel_id}/members:
    get:
      summary: Get channel members
      description: |-
        Get a page of members for a channel.
        ##### Permissions
        `read_channel` permission for the channel.
      operationId: get-a-page-of-members-for-a-channel-permissionsread-channel-permission-for-the-channel
      x-api-path-slug: channelschannel-idmembers-get
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of members per page
      responses:
        200:
          description: OK
      tags:
      - Channel
      - Members
    post:
      summary: Add user to channel
      description: Add a user to a channel by creating a channel member object.
      operationId: add-a-user-to-a-channel-by-creating-a-channel-member-object
      x-api-path-slug: channelschannel-idmembers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: channel_id
        description: The channel ID
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Channel
  /channels/{channel_id}/members/ids:
    post:
      summary: Get channel members by ids
      description: |-
        Get a list of channel members based on the provided user ids.
        ##### Permissions
        Must have the `read_channel` permission.
      operationId: get-a-list-of-channel-members-based-on-the-provided-user-ids-permissionsmust-have-the-read-channel-p
      x-api-path-slug: channelschannel-idmembersids-post
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      - in: body
        name: user_ids
        description: List of user ids
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Channel
      - Members
      - By
      - Ids
  /channels/{channel_id}/members/{user_id}:
    get:
      summary: Get channel member
      description: |-
        Get a channel member.
        ##### Permissions
        `read_channel` permission for the channel.
      operationId: get-a-channel-member-permissionsread-channel-permission-for-the-channel
      x-api-path-slug: channelschannel-idmembersuser-id-get
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Channel
      - Member
    delete:
      summary: Remove user from channel
      description: |-
        Delete a channel member, effectively removing them from a channel.
        ##### Permissions
        `manage_public_channel_members` permission if the channel is public.
        `manage_private_channel_members` permission if the channel is private.
      operationId: delete-a-channel-member-effectively-removing-them-from-a-channel-permissionsmanage-public-channel-me
      x-api-path-slug: channelschannel-idmembersuser-id-delete
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Remove
      - User
      - From
      - Channel
  /channels/{channel_id}/members/{user_id}/roles:
    put:
      summary: Update channel roles
      description: |-
        Update a user's roles for a channel.
        ##### Permissions
        Must have `manage_channel_roles` permission for the channel.
      operationId: update-a-users-roles-for-a-channel-permissionsmust-have-manage-channel-roles-permission-for-the-chan
      x-api-path-slug: channelschannel-idmembersuser-idroles-put
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      - in: body
        name: roles
        description: Space-delimited channel roles to assign to the user
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Channel
      - Roles
  /channels/{channel_id}/members/{user_id}/notify_props:
    put:
      summary: Update channel notifications
      description: |-
        Update a user's notification properties for a channel. Only the provided fields are updated.
        ##### Permissions
        Must be logged in as the user or have `edit_other_users` permission.
      operationId: update-a-users-notification-properties-for-a-channel-only-the-provided-fields-are-updated-permission
      x-api-path-slug: channelschannel-idmembersuser-idnotify-props-put
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      - in: body
        name: notify_props
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Channel
      - Notifications
  /channels/members/{user_id}/view:
    post:
      summary: View channel
      description: |-
        Perform all the actions involved in viewing a channel. This includes marking channels as read, clearing push notifications, and updating the active channel.
        ##### Permissions
        Must be logged in as user or have `edit_other_users` permission.

        __Response only includes `last_viewed_at_times` in Mattermost server 4.3 and newer.__
      operationId: perform-all-the-actions-involved-in-viewing-a-channel-this-includes-marking-channels-as-read-clearin
      x-api-path-slug: channelsmembersuser-idview-post
      parameters:
      - in: body
        name: body
        description: Paremeters affecting how and which channels to view
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User ID to perform the view action for
      responses:
        200:
          description: OK
      tags:
      - View
      - Channel
  /users/{user_id}/teams/{team_id}/channels/members:
    get:
      summary: Get channel members for user
      description: |-
        Get all channel members on a team for a user.
        ##### Permissions
        Logged in as the user and `view_team` permission for the team. Having `manage_system` permission voids the previous requirements.
      operationId: get-all-channel-members-on-a-team-for-a-user-permissionslogged-in-as-the-user-and-view-team-permissi
      x-api-path-slug: usersuser-idteamsteam-idchannelsmembers-get
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
      - Channel
      - Membersuser
  /channels/{channel_id}/posts:
    get:
      summary: Get posts for a channel
      description: |-
        Get a page of posts in a channel. Use the query parameters to modify the behaviour of this endpoint. The parameters `since`, `before` and `after` must not be used together.
        ##### Permissions
        Must have `read_channel` permission for the channel.
      operationId: get-a-page-of-posts-in-a-channel-use-the-query-parameters-to-modify-the-behaviour-of-this-endpoint-t
      x-api-path-slug: channelschannel-idposts-get
      parameters:
      - in: query
        name: after
        description: A post id to select the posts that came after this one
      - in: query
        name: before
        description: A post id to select the posts that came before this one
      - in: path
        name: channel_id
        description: The channel ID to get the posts for
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of posts per page
      - in: query
        name: since
        description: Provide a non-zero value in Unix time milliseconds to select
          posts created after that time
      responses:
        200:
          description: OK
      tags:
      - Postsa
      - Channel
  /posts/{post_id}/pin:
    post:
      summary: Pin a post to the channel
      description: |-
        Pin a post to a channel it is in based from the provided post id string.
        ##### Permissions
        Must be authenticated and have the `read_channel` permission to the channel the post is in.
      operationId: pin-a-post-to-a-channel-it-is-in-based-from-the-provided-post-id-string-permissionsmust-be-authentic
      x-api-path-slug: postspost-idpin-post
      parameters:
      - in: path
        name: post_id
        description: Post GUID
      responses:
        200:
          description: OK
      tags:
      - Pin
      - Post
      - To
      - Channel
  /posts/{post_id}/unpin:
    post:
      summary: Unpin a post to the channel
      description: |-
        Unpin a post to a channel it is in based from the provided post id string.
        ##### Permissions
        Must be authenticated and have the `read_channel` permission to the channel the post is in.
      operationId: unpin-a-post-to-a-channel-it-is-in-based-from-the-provided-post-id-string-permissionsmust-be-authent
      x-api-path-slug: postspost-idunpin-post
      parameters:
      - in: path
        name: post_id
        description: Post GUID
      responses:
        200:
          description: OK
      tags:
      - Unpin
      - Post
      - To
      - Channel
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