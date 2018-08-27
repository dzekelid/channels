---
swagger: "2.0"
x-collection-name: Slack
x-complete: 0
info:
  title: Slack Invite Channel User
  description: Invites a user to a channel.
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /channels.archive:
    post:
      summary: Archive Channel
      description: Archives a channel.
      operationId: channels_archive
      x-api-path-slug: channels-archive-post
      parameters:
      - in: formData
        name: channel
        description: Channel to archive
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
      - Archives
  /channels.info:
    get:
      summary: Get Channel
      description: Gets information about a channel.
      operationId: channels_info
      x-api-path-slug: channels-info-get
      parameters:
      - in: query
        name: channel
        description: Channel to get info on
      - in: query
        name: include_locale
        description: Set this to `true` to receive the locale for this channel
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
  /channels.kick:
    post:
      summary: Remove User From Channel
      description: Removes a user from a channel.
      operationId: channels_kick
      x-api-path-slug: channels-kick-post
      parameters:
      - in: formData
        name: channel
        description: Channel to remove user from
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: user
        description: User to remove from channel
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
  /channels.history:
    get:
      summary: Get Channel History
      description: Fetches history of messages and events from a channel.
      operationId: channels_history
      x-api-path-slug: channels-history-get
      parameters:
      - in: query
        name: channel
        description: Channel to fetch history for
      - in: query
        name: count
        description: Number of messages to return, between 1 and 1000
      - in: query
        name: inclusive
        description: Include messages with latest or oldest timestamp in results
      - in: query
        name: latest
        description: End of time range of messages to include in results
      - in: query
        name: oldest
        description: Start of time range of messages to include in results
      - in: query
        name: token
        description: Authentication token
      - in: query
        name: unreads
        description: Include `unread_count_display` in the output?
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
  /channels.leave:
    post:
      summary: Leave Channel
      description: Leaves a channel.
      operationId: channels_leave
      x-api-path-slug: channels-leave-post
      parameters:
      - in: formData
        name: channel
        description: Channel to leave
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
  /channels.rename:
    post:
      summary: Rename Channel
      description: Renames a channel.
      operationId: channels_rename
      x-api-path-slug: channels-rename-post
      parameters:
      - in: formData
        name: channel
        description: Channel to rename
      - in: formData
        name: name
        description: New name for channel
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: validate
        description: Whether to return errors on invalid channel name instead of modifying
          it to meet the specified criteria
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
  /channels.mark:
    post:
      summary: Mark Channel
      description: Sets the read cursor in a channel.
      operationId: channels_mark
      x-api-path-slug: channels-mark-post
      parameters:
      - in: formData
        name: channel
        description: Channel to set reading cursor in
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: ts
        description: Timestamp of the most recently seen message
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
  /channels.unarchive:
    post:
      summary: Unarchive Channel
      description: Unarchives a channel.
      operationId: channels_unarchive
      x-api-path-slug: channels-unarchive-post
      parameters:
      - in: formData
        name: channel
        description: Channel to unarchive
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
      - Archives
  /channels.create:
    post:
      summary: Create Channel
      description: Creates a channel.
      operationId: channels_create
      x-api-path-slug: channels-create-post
      parameters:
      - in: formData
        name: name
        description: Name of channel to create
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: validate
        description: Whether to return errors on invalid channel name instead of modifying
          it to meet the specified criteria
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
  /channels.join:
    post:
      summary: Join Channel
      description: Joins a channel, creating it if needed.
      operationId: channels_join
      x-api-path-slug: channels-join-post
      parameters:
      - in: formData
        name: name
        description: Name of channel to join
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: validate
        description: Whether to return errors on invalid channel name instead of modifying
          it to meet the specified criteria
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
  /channels.setTopic:
    post:
      summary: Set Channel Topic
      description: Sets the topic for a channel.
      operationId: channels_setTopic
      x-api-path-slug: channels-settopic-post
      parameters:
      - in: formData
        name: channel
        description: Channel to set the topic of
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: topic
        description: The new topic
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
  /channels.setPurpose:
    post:
      summary: Set Channel Purpose
      description: Sets the purpose for a channel.
      operationId: channels_setPurpose
      x-api-path-slug: channels-setpurpose-post
      parameters:
      - in: formData
        name: channel
        description: Channel to set the purpose of
      - in: formData
        name: purpose
        description: The new purpose
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
  /channels.list:
    get:
      summary: List Channels
      description: Lists all channels in a Slack team.
      operationId: channels_list
      x-api-path-slug: channels-list-get
      parameters:
      - in: query
        name: cursor
        description: Paginate through collections of data by setting the `cursor`
          parameter to a `next_cursor` attribute returned by a previous requests `response_metadata`
      - in: query
        name: exclude_archived
        description: Exclude archived channels from the list
      - in: query
        name: exclude_members
        description: Exclude the `members` collection from each `channel`
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
  /channels.invite:
    post:
      summary: Invite Channel User
      description: Invites a user to a channel.
      operationId: channels_invite
      x-api-path-slug: channels-invite-post
      parameters:
      - in: formData
        name: channel
        description: Channel to invite user to
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: user
        description: User to invite to channel
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
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