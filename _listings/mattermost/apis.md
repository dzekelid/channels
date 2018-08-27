---
name: Mattermost
x-slug: mattermost
description: Open source, private cloud Slack-alternative, Workplace messaging for
  web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
  configurable, and scalable from teams to the enterprise.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
x-kinRank: "8"
x-alexaRank: "95684"
tags: Channels
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/apis.md
specificationVersion: "0.14"
apis:
- name: Mattermost API Reference - Get a list of channels by ids
  x-api-slug: teamsteam-idchannelsids-post
  description: |-
    Get a list of public channels on a team by id.
    ##### Permissions
    `view_team` for the team the channels are on.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsids-post-openapi.md
- name: Mattermost API Reference - Get a channels pinned posts
  x-api-slug: channelschannel-idpinned-get
  description: Get a list of pinned posts for channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idpinned-get-openapi.md
- name: Mattermost API Reference - Get public channels
  x-api-slug: teamsteam-idchannels-get
  description: |-
    Get a page of public channels on a team based on query string parameters - page and per_page.
    ##### Permissions
    Must be authenticated and have the `list_team_channels` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannels-get-openapi.md
- name: Mattermost API Reference - Get deleted channels
  x-api-slug: teamsteam-idchannelsdeleted-get
  description: |-
    Get a page of deleted channels on a team based on query string parameters - team_id, page and per_page.

    __Minimum server version__: 3.10

    ##### Permissions
    Must be authenticated and have the `manage_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsdeleted-get-openapi.md
- name: Mattermost API Reference - Autocomplete channels
  x-api-slug: teamsteam-idchannelsautocomplete-get
  description: |-
    Autocomplete public channels on a team based on the search term provided in the request URL.

    __Minimum server version__: 4.7

    ##### Permissions
    Must have the `list_team_channels` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsautocomplete-get-openapi.md
- name: Mattermost API Reference - Search channels
  x-api-slug: teamsteam-idchannelssearch-post
  description: |-
    Search public channels on a team based on the search term provided in the request body.
    ##### Permissions
    Must have the `list_team_channels` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelssearch-post-openapi.md
- name: Mattermost API Reference - Create a channel
  x-api-slug: channels-post
  description: |-
    Create a new channel.
    ##### Permissions
    If creating a public channel, `create_public_channel` permission is required. If creating a private channel, `create_private_channel` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channels-post-openapi.md
- name: Mattermost API Reference - Create a direct message channel
  x-api-slug: channelsdirect-post
  description: |-
    Create a new direct message channel between two users.
    ##### Permissions
    Must be one of the two users and have `create_direct_channel` permission. Having the `manage_system` permission voids the previous requirements.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsdirect-post-openapi.md
- name: Mattermost API Reference - Create a group message channel
  x-api-slug: channelsgroup-post
  description: |-
    Create a new group message channel to group of users. If the logged in user's id is not included in the list, it will be appended to the end.
    ##### Permissions
    Must have `create_group_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsgroup-post-openapi.md
- name: Mattermost API Reference - Get a channel
  x-api-slug: channelschannel-id-get
  description: |-
    Get channel from the provided channel id string.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-get-openapi.md
- name: Mattermost API Reference - Update a channel
  x-api-slug: channelschannel-id-put
  description: |-
    Update a channel. The fields that can be updated are listed as paramters. Omitted fields will be treated as blanks.
    ##### Permissions
    If updating a public channel, `manage_public_channel_members` permission is required. If updating a private channel, `manage_private_channel_members` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-put-openapi.md
- name: Mattermost API Reference - Delete a channel
  x-api-slug: channelschannel-id-delete
  description: |-
    Soft deletes a channel, by marking the channel as deleted in the database. Soft deleted channels will not be accessible in the user interface.
    ##### Permissions
    `delete_public_channel` permission if the channel is public,
    `delete_private_channel` permission if the channel is private,
    or have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-delete-openapi.md
- name: Mattermost API Reference - Patch a channel
  x-api-slug: channelschannel-idpatch-put
  description: |-
    Partially update a channel by providing only the fields you want to update. Omitted fields will not be updated. The fields that can be updated are defined in the request body, all other provided fields will be ignored.
    ##### Permissions
    If updating a public channel, `manage_public_channel_members` permission is required. If updating a private channel, `manage_private_channel_members` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idpatch-put-openapi.md
- name: Mattermost API Reference - Convert a channel from public to private
  x-api-slug: channelschannel-idconvert-post
  description: |-
    Convert into private channel from the provided channel id string.

    __Minimum server version__: 4.10

    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idconvert-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idconvert-post-openapi.md
- name: Mattermost API Reference - Restore a channel
  x-api-slug: channelschannel-idrestore-post
  description: |-
    Restore channel from the provided channel id string.

    __Minimum server version__: 3.10

    ##### Permissions
    `manage_team` permission for the team of channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idrestore-post-openapi.md
- name: Mattermost API Reference - Get channel statistics
  x-api-slug: channelschannel-idstats-get
  description: |-
    Get statistics for a channel.
    ##### Permissions
    Must have the `read_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idstats-get-openapi.md
- name: Mattermost API Reference - Get a channel by name
  x-api-slug: teamsteam-idchannelsnamechannel-name-get
  description: |-
    Gets channel from the provided team id and channel name strings.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsnamechannel-name-get-openapi.md
- name: Mattermost API Reference - Get a channel by name and team name
  x-api-slug: teamsnameteam-namechannelsnamechannel-name-get
  description: |-
    Gets a channel from the provided team name and channel name strings.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsnameteam-namechannelsnamechannel-name-get-openapi.md
- name: Mattermost API Reference - Get channel members
  x-api-slug: channelschannel-idmembers-get
  description: |-
    Get a page of members for a channel.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembers-get-openapi.md
- name: Mattermost API Reference - Add user to channel
  x-api-slug: channelschannel-idmembers-post
  description: Add a user to a channel by creating a channel member object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembers-post-openapi.md
- name: Mattermost API Reference - Get channel members by ids
  x-api-slug: channelschannel-idmembersids-post
  description: |-
    Get a list of channel members based on the provided user ids.
    ##### Permissions
    Must have the `read_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersids-post-openapi.md
- name: Mattermost API Reference - Get channel member
  x-api-slug: channelschannel-idmembersuser-id-get
  description: |-
    Get a channel member.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-id-get-openapi.md
- name: Mattermost API Reference - Remove user from channel
  x-api-slug: channelschannel-idmembersuser-id-delete
  description: |-
    Delete a channel member, effectively removing them from a channel.
    ##### Permissions
    `manage_public_channel_members` permission if the channel is public.
    `manage_private_channel_members` permission if the channel is private.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-id-delete-openapi.md
- name: Mattermost API Reference - Update channel roles
  x-api-slug: channelschannel-idmembersuser-idroles-put
  description: |-
    Update a user's roles for a channel.
    ##### Permissions
    Must have `manage_channel_roles` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-idroles-put-openapi.md
- name: Mattermost API Reference - Update channel notifications
  x-api-slug: channelschannel-idmembersuser-idnotify-props-put
  description: |-
    Update a user's notification properties for a channel. Only the provided fields are updated.
    ##### Permissions
    Must be logged in as the user or have `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-idnotify-props-put-openapi.md
- name: Mattermost API Reference - View channel
  x-api-slug: channelsmembersuser-idview-post
  description: |-
    Perform all the actions involved in viewing a channel. This includes marking channels as read, clearing push notifications, and updating the active channel.
    ##### Permissions
    Must be logged in as user or have `edit_other_users` permission.

    __Response only includes `last_viewed_at_times` in Mattermost server 4.3 and newer.__
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsmembersuser-idview-post-openapi.md
- name: Mattermost API Reference - Get channel members for user
  x-api-slug: usersuser-idteamsteam-idchannelsmembers-get
  description: |-
    Get all channel members on a team for a user.
    ##### Permissions
    Logged in as the user and `view_team` permission for the team. Having `manage_system` permission voids the previous requirements.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/usersuser-idteamsteam-idchannelsmembers-get-openapi.md
- name: Mattermost API Reference - Get posts for a channel
  x-api-slug: channelschannel-idposts-get
  description: |-
    Get a page of posts in a channel. Use the query parameters to modify the behaviour of this endpoint. The parameters `since`, `before` and `after` must not be used together.
    ##### Permissions
    Must have `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idposts-get-openapi.md
- name: Mattermost API Reference - Pin a post to the channel
  x-api-slug: postspost-idpin-post
  description: |-
    Pin a post to a channel it is in based from the provided post id string.
    ##### Permissions
    Must be authenticated and have the `read_channel` permission to the channel the post is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/postspost-idpin-post-openapi.md
- name: Mattermost API Reference - Unpin a post to the channel
  x-api-slug: postspost-idunpin-post
  description: |-
    Unpin a post to a channel it is in based from the provided post id string.
    ##### Permissions
    Must be authenticated and have the `read_channel` permission to the channel the post is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/postspost-idunpin-post-openapi.md
- name: Mattermost API Reference - Create a channel
  x-api-slug: channels-post
  description: |-
    Create a new channel.
    ##### Permissions
    If creating a public channel, `create_public_channel` permission is required. If creating a private channel, `create_private_channel` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channels-post-openapi.md
- name: Mattermost API Reference - Create a channel
  x-api-slug: channels-post
  description: |-
    Create a new channel.
    ##### Permissions
    If creating a public channel, `create_public_channel` permission is required. If creating a private channel, `create_private_channel` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channels-post-openapi.md
- name: Mattermost API Reference - Create a channel
  x-api-slug: channels-post
  description: |-
    Create a new channel.
    ##### Permissions
    If creating a public channel, `create_public_channel` permission is required. If creating a private channel, `create_private_channel` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channels-post-openapi.md
- name: Mattermost API Reference - Create a direct message channel
  x-api-slug: channelsdirect-post
  description: |-
    Create a new direct message channel between two users.
    ##### Permissions
    Must be one of the two users and have `create_direct_channel` permission. Having the `manage_system` permission voids the previous requirements.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsdirect-post-openapi.md
- name: Mattermost API Reference - Create a direct message channel
  x-api-slug: channelsdirect-post
  description: |-
    Create a new direct message channel between two users.
    ##### Permissions
    Must be one of the two users and have `create_direct_channel` permission. Having the `manage_system` permission voids the previous requirements.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsdirect-post-openapi.md
- name: Mattermost API Reference - Create a direct message channel
  x-api-slug: channelsdirect-post
  description: |-
    Create a new direct message channel between two users.
    ##### Permissions
    Must be one of the two users and have `create_direct_channel` permission. Having the `manage_system` permission voids the previous requirements.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsdirect-post-openapi.md
- name: Mattermost API Reference - Create a group message channel
  x-api-slug: channelsgroup-post
  description: |-
    Create a new group message channel to group of users. If the logged in user's id is not included in the list, it will be appended to the end.
    ##### Permissions
    Must have `create_group_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsgroup-post-openapi.md
- name: Mattermost API Reference - Create a group message channel
  x-api-slug: channelsgroup-post
  description: |-
    Create a new group message channel to group of users. If the logged in user's id is not included in the list, it will be appended to the end.
    ##### Permissions
    Must have `create_group_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsgroup-post-openapi.md
- name: Mattermost API Reference - Create a group message channel
  x-api-slug: channelsgroup-post
  description: |-
    Create a new group message channel to group of users. If the logged in user's id is not included in the list, it will be appended to the end.
    ##### Permissions
    Must have `create_group_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsgroup-post-openapi.md
- name: Mattermost API Reference - Get a channel
  x-api-slug: channelschannel-id-get
  description: |-
    Get channel from the provided channel id string.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-get-openapi.md
- name: Mattermost API Reference - Get a channel
  x-api-slug: channelschannel-id-get
  description: |-
    Get channel from the provided channel id string.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-get-openapi.md
- name: Mattermost API Reference - Get a channel
  x-api-slug: channelschannel-id-get
  description: |-
    Get channel from the provided channel id string.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-get-openapi.md
- name: Mattermost API Reference - Update a channel
  x-api-slug: channelschannel-id-put
  description: |-
    Update a channel. The fields that can be updated are listed as paramters. Omitted fields will be treated as blanks.
    ##### Permissions
    If updating a public channel, `manage_public_channel_members` permission is required. If updating a private channel, `manage_private_channel_members` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-put-openapi.md
- name: Mattermost API Reference - Update a channel
  x-api-slug: channelschannel-id-put
  description: |-
    Update a channel. The fields that can be updated are listed as paramters. Omitted fields will be treated as blanks.
    ##### Permissions
    If updating a public channel, `manage_public_channel_members` permission is required. If updating a private channel, `manage_private_channel_members` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-put-openapi.md
- name: Mattermost API Reference - Update a channel
  x-api-slug: channelschannel-id-put
  description: |-
    Update a channel. The fields that can be updated are listed as paramters. Omitted fields will be treated as blanks.
    ##### Permissions
    If updating a public channel, `manage_public_channel_members` permission is required. If updating a private channel, `manage_private_channel_members` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-put-openapi.md
- name: Mattermost API Reference - Delete a channel
  x-api-slug: channelschannel-id-delete
  description: |-
    Soft deletes a channel, by marking the channel as deleted in the database. Soft deleted channels will not be accessible in the user interface.
    ##### Permissions
    `delete_public_channel` permission if the channel is public,
    `delete_private_channel` permission if the channel is private,
    or have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-delete-openapi.md
- name: Mattermost API Reference - Delete a channel
  x-api-slug: channelschannel-id-delete
  description: |-
    Soft deletes a channel, by marking the channel as deleted in the database. Soft deleted channels will not be accessible in the user interface.
    ##### Permissions
    `delete_public_channel` permission if the channel is public,
    `delete_private_channel` permission if the channel is private,
    or have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-delete-openapi.md
- name: Mattermost API Reference - Delete a channel
  x-api-slug: channelschannel-id-delete
  description: |-
    Soft deletes a channel, by marking the channel as deleted in the database. Soft deleted channels will not be accessible in the user interface.
    ##### Permissions
    `delete_public_channel` permission if the channel is public,
    `delete_private_channel` permission if the channel is private,
    or have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-delete-openapi.md
- name: Mattermost API Reference - Patch a channel
  x-api-slug: channelschannel-idpatch-put
  description: |-
    Partially update a channel by providing only the fields you want to update. Omitted fields will not be updated. The fields that can be updated are defined in the request body, all other provided fields will be ignored.
    ##### Permissions
    If updating a public channel, `manage_public_channel_members` permission is required. If updating a private channel, `manage_private_channel_members` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idpatch-put-openapi.md
- name: Mattermost API Reference - Patch a channel
  x-api-slug: channelschannel-idpatch-put
  description: |-
    Partially update a channel by providing only the fields you want to update. Omitted fields will not be updated. The fields that can be updated are defined in the request body, all other provided fields will be ignored.
    ##### Permissions
    If updating a public channel, `manage_public_channel_members` permission is required. If updating a private channel, `manage_private_channel_members` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idpatch-put-openapi.md
- name: Mattermost API Reference - Patch a channel
  x-api-slug: channelschannel-idpatch-put
  description: |-
    Partially update a channel by providing only the fields you want to update. Omitted fields will not be updated. The fields that can be updated are defined in the request body, all other provided fields will be ignored.
    ##### Permissions
    If updating a public channel, `manage_public_channel_members` permission is required. If updating a private channel, `manage_private_channel_members` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idpatch-put-openapi.md
- name: Mattermost API Reference - Convert a channel from public to private
  x-api-slug: channelschannel-idconvert-post
  description: |-
    Convert into private channel from the provided channel id string.

    __Minimum server version__: 4.10

    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idconvert-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idconvert-post-openapi.md
- name: Mattermost API Reference - Convert a channel from public to private
  x-api-slug: channelschannel-idconvert-post
  description: |-
    Convert into private channel from the provided channel id string.

    __Minimum server version__: 4.10

    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idconvert-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idconvert-post-openapi.md
- name: Mattermost API Reference - Convert a channel from public to private
  x-api-slug: channelschannel-idconvert-post
  description: |-
    Convert into private channel from the provided channel id string.

    __Minimum server version__: 4.10

    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idconvert-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idconvert-post-openapi.md
- name: Mattermost API Reference - Restore a channel
  x-api-slug: channelschannel-idrestore-post
  description: |-
    Restore channel from the provided channel id string.

    __Minimum server version__: 3.10

    ##### Permissions
    `manage_team` permission for the team of channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idrestore-post-openapi.md
- name: Mattermost API Reference - Restore a channel
  x-api-slug: channelschannel-idrestore-post
  description: |-
    Restore channel from the provided channel id string.

    __Minimum server version__: 3.10

    ##### Permissions
    `manage_team` permission for the team of channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idrestore-post-openapi.md
- name: Mattermost API Reference - Restore a channel
  x-api-slug: channelschannel-idrestore-post
  description: |-
    Restore channel from the provided channel id string.

    __Minimum server version__: 3.10

    ##### Permissions
    `manage_team` permission for the team of channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idrestore-post-openapi.md
- name: Mattermost API Reference - Get channel statistics
  x-api-slug: channelschannel-idstats-get
  description: |-
    Get statistics for a channel.
    ##### Permissions
    Must have the `read_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idstats-get-openapi.md
- name: Mattermost API Reference - Get channel statistics
  x-api-slug: channelschannel-idstats-get
  description: |-
    Get statistics for a channel.
    ##### Permissions
    Must have the `read_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idstats-get-openapi.md
- name: Mattermost API Reference - Get channel statistics
  x-api-slug: channelschannel-idstats-get
  description: |-
    Get statistics for a channel.
    ##### Permissions
    Must have the `read_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idstats-get-openapi.md
- name: Mattermost API Reference - Get a channel by name
  x-api-slug: teamsteam-idchannelsnamechannel-name-get
  description: |-
    Gets channel from the provided team id and channel name strings.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsnamechannel-name-get-openapi.md
- name: Mattermost API Reference - Get a channel by name
  x-api-slug: teamsteam-idchannelsnamechannel-name-get
  description: |-
    Gets channel from the provided team id and channel name strings.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsnamechannel-name-get-openapi.md
- name: Mattermost API Reference - Get a channel by name
  x-api-slug: teamsteam-idchannelsnamechannel-name-get
  description: |-
    Gets channel from the provided team id and channel name strings.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsnamechannel-name-get-openapi.md
- name: Mattermost API Reference - Get a channel by name and team name
  x-api-slug: teamsnameteam-namechannelsnamechannel-name-get
  description: |-
    Gets a channel from the provided team name and channel name strings.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsnameteam-namechannelsnamechannel-name-get-openapi.md
- name: Mattermost API Reference - Get a channel by name and team name
  x-api-slug: teamsnameteam-namechannelsnamechannel-name-get
  description: |-
    Gets a channel from the provided team name and channel name strings.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsnameteam-namechannelsnamechannel-name-get-openapi.md
- name: Mattermost API Reference - Get a channel by name and team name
  x-api-slug: teamsnameteam-namechannelsnamechannel-name-get
  description: |-
    Gets a channel from the provided team name and channel name strings.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsnameteam-namechannelsnamechannel-name-get-openapi.md
- name: Mattermost API Reference - Get channel members
  x-api-slug: channelschannel-idmembers-get
  description: |-
    Get a page of members for a channel.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembers-get-openapi.md
- name: Mattermost API Reference - Get channel members
  x-api-slug: channelschannel-idmembers-get
  description: |-
    Get a page of members for a channel.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembers-get-openapi.md
- name: Mattermost API Reference - Get channel members
  x-api-slug: channelschannel-idmembers-get
  description: |-
    Get a page of members for a channel.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembers-get-openapi.md
- name: Mattermost API Reference - Add user to channel
  x-api-slug: channelschannel-idmembers-post
  description: Add a user to a channel by creating a channel member object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembers-post-openapi.md
- name: Mattermost API Reference - Add user to channel
  x-api-slug: channelschannel-idmembers-post
  description: Add a user to a channel by creating a channel member object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembers-post-openapi.md
- name: Mattermost API Reference - Add user to channel
  x-api-slug: channelschannel-idmembers-post
  description: Add a user to a channel by creating a channel member object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembers-post-openapi.md
- name: Mattermost API Reference - Get channel members by ids
  x-api-slug: channelschannel-idmembersids-post
  description: |-
    Get a list of channel members based on the provided user ids.
    ##### Permissions
    Must have the `read_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersids-post-openapi.md
- name: Mattermost API Reference - Get channel members by ids
  x-api-slug: channelschannel-idmembersids-post
  description: |-
    Get a list of channel members based on the provided user ids.
    ##### Permissions
    Must have the `read_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersids-post-openapi.md
- name: Mattermost API Reference - Get channel members by ids
  x-api-slug: channelschannel-idmembersids-post
  description: |-
    Get a list of channel members based on the provided user ids.
    ##### Permissions
    Must have the `read_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersids-post-openapi.md
- name: Mattermost API Reference - Get channel member
  x-api-slug: channelschannel-idmembersuser-id-get
  description: |-
    Get a channel member.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-id-get-openapi.md
- name: Mattermost API Reference - Get channel member
  x-api-slug: channelschannel-idmembersuser-id-get
  description: |-
    Get a channel member.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-id-get-openapi.md
- name: Mattermost API Reference - Get channel member
  x-api-slug: channelschannel-idmembersuser-id-get
  description: |-
    Get a channel member.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-id-get-openapi.md
- name: Mattermost API Reference - Remove user from channel
  x-api-slug: channelschannel-idmembersuser-id-delete
  description: |-
    Delete a channel member, effectively removing them from a channel.
    ##### Permissions
    `manage_public_channel_members` permission if the channel is public.
    `manage_private_channel_members` permission if the channel is private.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-id-delete-openapi.md
- name: Mattermost API Reference - Remove user from channel
  x-api-slug: channelschannel-idmembersuser-id-delete
  description: |-
    Delete a channel member, effectively removing them from a channel.
    ##### Permissions
    `manage_public_channel_members` permission if the channel is public.
    `manage_private_channel_members` permission if the channel is private.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-id-delete-openapi.md
- name: Mattermost API Reference - Remove user from channel
  x-api-slug: channelschannel-idmembersuser-id-delete
  description: |-
    Delete a channel member, effectively removing them from a channel.
    ##### Permissions
    `manage_public_channel_members` permission if the channel is public.
    `manage_private_channel_members` permission if the channel is private.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-id-delete-openapi.md
- name: Mattermost API Reference - Update channel roles
  x-api-slug: channelschannel-idmembersuser-idroles-put
  description: |-
    Update a user's roles for a channel.
    ##### Permissions
    Must have `manage_channel_roles` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-idroles-put-openapi.md
- name: Mattermost API Reference - Update channel roles
  x-api-slug: channelschannel-idmembersuser-idroles-put
  description: |-
    Update a user's roles for a channel.
    ##### Permissions
    Must have `manage_channel_roles` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-idroles-put-openapi.md
- name: Mattermost API Reference - Update channel roles
  x-api-slug: channelschannel-idmembersuser-idroles-put
  description: |-
    Update a user's roles for a channel.
    ##### Permissions
    Must have `manage_channel_roles` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-idroles-put-openapi.md
- name: Mattermost API Reference - Update channel notifications
  x-api-slug: channelschannel-idmembersuser-idnotify-props-put
  description: |-
    Update a user's notification properties for a channel. Only the provided fields are updated.
    ##### Permissions
    Must be logged in as the user or have `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-idnotify-props-put-openapi.md
- name: Mattermost API Reference - Update channel notifications
  x-api-slug: channelschannel-idmembersuser-idnotify-props-put
  description: |-
    Update a user's notification properties for a channel. Only the provided fields are updated.
    ##### Permissions
    Must be logged in as the user or have `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-idnotify-props-put-openapi.md
- name: Mattermost API Reference - Update channel notifications
  x-api-slug: channelschannel-idmembersuser-idnotify-props-put
  description: |-
    Update a user's notification properties for a channel. Only the provided fields are updated.
    ##### Permissions
    Must be logged in as the user or have `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-idnotify-props-put-openapi.md
- name: Mattermost API Reference - View channel
  x-api-slug: channelsmembersuser-idview-post
  description: |-
    Perform all the actions involved in viewing a channel. This includes marking channels as read, clearing push notifications, and updating the active channel.
    ##### Permissions
    Must be logged in as user or have `edit_other_users` permission.

    __Response only includes `last_viewed_at_times` in Mattermost server 4.3 and newer.__
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsmembersuser-idview-post-openapi.md
- name: Mattermost API Reference - View channel
  x-api-slug: channelsmembersuser-idview-post
  description: |-
    Perform all the actions involved in viewing a channel. This includes marking channels as read, clearing push notifications, and updating the active channel.
    ##### Permissions
    Must be logged in as user or have `edit_other_users` permission.

    __Response only includes `last_viewed_at_times` in Mattermost server 4.3 and newer.__
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsmembersuser-idview-post-openapi.md
- name: Mattermost API Reference - View channel
  x-api-slug: channelsmembersuser-idview-post
  description: |-
    Perform all the actions involved in viewing a channel. This includes marking channels as read, clearing push notifications, and updating the active channel.
    ##### Permissions
    Must be logged in as user or have `edit_other_users` permission.

    __Response only includes `last_viewed_at_times` in Mattermost server 4.3 and newer.__
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsmembersuser-idview-post-openapi.md
- name: Mattermost API Reference - Get channel members for user
  x-api-slug: usersuser-idteamsteam-idchannelsmembers-get
  description: |-
    Get all channel members on a team for a user.
    ##### Permissions
    Logged in as the user and `view_team` permission for the team. Having `manage_system` permission voids the previous requirements.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/usersuser-idteamsteam-idchannelsmembers-get-openapi.md
- name: Mattermost API Reference - Get channel members for user
  x-api-slug: usersuser-idteamsteam-idchannelsmembers-get
  description: |-
    Get all channel members on a team for a user.
    ##### Permissions
    Logged in as the user and `view_team` permission for the team. Having `manage_system` permission voids the previous requirements.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/usersuser-idteamsteam-idchannelsmembers-get-openapi.md
- name: Mattermost API Reference - Get channel members for user
  x-api-slug: usersuser-idteamsteam-idchannelsmembers-get
  description: |-
    Get all channel members on a team for a user.
    ##### Permissions
    Logged in as the user and `view_team` permission for the team. Having `manage_system` permission voids the previous requirements.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/usersuser-idteamsteam-idchannelsmembers-get-openapi.md
- name: Mattermost API Reference - Get posts for a channel
  x-api-slug: channelschannel-idposts-get
  description: |-
    Get a page of posts in a channel. Use the query parameters to modify the behaviour of this endpoint. The parameters `since`, `before` and `after` must not be used together.
    ##### Permissions
    Must have `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idposts-get-openapi.md
- name: Mattermost API Reference - Get posts for a channel
  x-api-slug: channelschannel-idposts-get
  description: |-
    Get a page of posts in a channel. Use the query parameters to modify the behaviour of this endpoint. The parameters `since`, `before` and `after` must not be used together.
    ##### Permissions
    Must have `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idposts-get-openapi.md
- name: Mattermost API Reference - Get posts for a channel
  x-api-slug: channelschannel-idposts-get
  description: |-
    Get a page of posts in a channel. Use the query parameters to modify the behaviour of this endpoint. The parameters `since`, `before` and `after` must not be used together.
    ##### Permissions
    Must have `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idposts-get-openapi.md
- name: Mattermost API Reference - Pin a post to the channel
  x-api-slug: postspost-idpin-post
  description: |-
    Pin a post to a channel it is in based from the provided post id string.
    ##### Permissions
    Must be authenticated and have the `read_channel` permission to the channel the post is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/postspost-idpin-post-openapi.md
- name: Mattermost API Reference - Pin a post to the channel
  x-api-slug: postspost-idpin-post
  description: |-
    Pin a post to a channel it is in based from the provided post id string.
    ##### Permissions
    Must be authenticated and have the `read_channel` permission to the channel the post is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/postspost-idpin-post-openapi.md
- name: Mattermost API Reference - Pin a post to the channel
  x-api-slug: postspost-idpin-post
  description: |-
    Pin a post to a channel it is in based from the provided post id string.
    ##### Permissions
    Must be authenticated and have the `read_channel` permission to the channel the post is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/postspost-idpin-post-openapi.md
- name: Mattermost API Reference - Unpin a post to the channel
  x-api-slug: postspost-idunpin-post
  description: |-
    Unpin a post to a channel it is in based from the provided post id string.
    ##### Permissions
    Must be authenticated and have the `read_channel` permission to the channel the post is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/postspost-idunpin-post-openapi.md
- name: Mattermost API Reference - Unpin a post to the channel
  x-api-slug: postspost-idunpin-post
  description: |-
    Unpin a post to a channel it is in based from the provided post id string.
    ##### Permissions
    Must be authenticated and have the `read_channel` permission to the channel the post is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/postspost-idunpin-post-openapi.md
- name: Mattermost API Reference - Unpin a post to the channel
  x-api-slug: postspost-idunpin-post
  description: |-
    Unpin a post to a channel it is in based from the provided post id string.
    ##### Permissions
    Must be authenticated and have the `read_channel` permission to the channel the post is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/postspost-idunpin-post-openapi.md
- name: Mattermost API Reference - Unpin a post to the channel
  x-api-slug: postspost-idunpin-post
  description: |-
    Unpin a post to a channel it is in based from the provided post id string.
    ##### Permissions
    Must be authenticated and have the `read_channel` permission to the channel the post is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/postspost-idunpin-post-openapi.md
- name: Mattermost API Reference - Pin a post to the channel
  x-api-slug: postspost-idpin-post
  description: |-
    Pin a post to a channel it is in based from the provided post id string.
    ##### Permissions
    Must be authenticated and have the `read_channel` permission to the channel the post is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/postspost-idpin-post-openapi.md
- name: Mattermost API Reference - Get posts for a channel
  x-api-slug: channelschannel-idposts-get
  description: |-
    Get a page of posts in a channel. Use the query parameters to modify the behaviour of this endpoint. The parameters `since`, `before` and `after` must not be used together.
    ##### Permissions
    Must have `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idposts-get-openapi.md
- name: Mattermost API Reference - Get channel members for user
  x-api-slug: usersuser-idteamsteam-idchannelsmembers-get
  description: |-
    Get all channel members on a team for a user.
    ##### Permissions
    Logged in as the user and `view_team` permission for the team. Having `manage_system` permission voids the previous requirements.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/usersuser-idteamsteam-idchannelsmembers-get-openapi.md
- name: Mattermost API Reference - View channel
  x-api-slug: channelsmembersuser-idview-post
  description: |-
    Perform all the actions involved in viewing a channel. This includes marking channels as read, clearing push notifications, and updating the active channel.
    ##### Permissions
    Must be logged in as user or have `edit_other_users` permission.

    __Response only includes `last_viewed_at_times` in Mattermost server 4.3 and newer.__
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsmembersuser-idview-post-openapi.md
- name: Mattermost API Reference - Update channel notifications
  x-api-slug: channelschannel-idmembersuser-idnotify-props-put
  description: |-
    Update a user's notification properties for a channel. Only the provided fields are updated.
    ##### Permissions
    Must be logged in as the user or have `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-idnotify-props-put-openapi.md
- name: Mattermost API Reference - Update channel roles
  x-api-slug: channelschannel-idmembersuser-idroles-put
  description: |-
    Update a user's roles for a channel.
    ##### Permissions
    Must have `manage_channel_roles` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-idroles-put-openapi.md
- name: Mattermost API Reference - Remove user from channel
  x-api-slug: channelschannel-idmembersuser-id-delete
  description: |-
    Delete a channel member, effectively removing them from a channel.
    ##### Permissions
    `manage_public_channel_members` permission if the channel is public.
    `manage_private_channel_members` permission if the channel is private.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-id-delete-openapi.md
- name: Mattermost API Reference - Get channel member
  x-api-slug: channelschannel-idmembersuser-id-get
  description: |-
    Get a channel member.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersuser-id-get-openapi.md
- name: Mattermost API Reference - Get channel members by ids
  x-api-slug: channelschannel-idmembersids-post
  description: |-
    Get a list of channel members based on the provided user ids.
    ##### Permissions
    Must have the `read_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembersids-post-openapi.md
- name: Mattermost API Reference - Add user to channel
  x-api-slug: channelschannel-idmembers-post
  description: Add a user to a channel by creating a channel member object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembers-post-openapi.md
- name: Mattermost API Reference - Get channel members
  x-api-slug: channelschannel-idmembers-get
  description: |-
    Get a page of members for a channel.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idmembers-get-openapi.md
- name: Mattermost API Reference - Get a channel by name and team name
  x-api-slug: teamsnameteam-namechannelsnamechannel-name-get
  description: |-
    Gets a channel from the provided team name and channel name strings.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsnameteam-namechannelsnamechannel-name-get-openapi.md
- name: Mattermost API Reference - Get a channel by name
  x-api-slug: teamsteam-idchannelsnamechannel-name-get
  description: |-
    Gets channel from the provided team id and channel name strings.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsnamechannel-name-get-openapi.md
- name: Mattermost API Reference - Get channel statistics
  x-api-slug: channelschannel-idstats-get
  description: |-
    Get statistics for a channel.
    ##### Permissions
    Must have the `read_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idstats-get-openapi.md
- name: Mattermost API Reference - Restore a channel
  x-api-slug: channelschannel-idrestore-post
  description: |-
    Restore channel from the provided channel id string.

    __Minimum server version__: 3.10

    ##### Permissions
    `manage_team` permission for the team of channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idrestore-post-openapi.md
- name: Mattermost API Reference - Convert a channel from public to private
  x-api-slug: channelschannel-idconvert-post
  description: |-
    Convert into private channel from the provided channel id string.

    __Minimum server version__: 4.10

    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idconvert-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idconvert-post-openapi.md
- name: Mattermost API Reference - Patch a channel
  x-api-slug: channelschannel-idpatch-put
  description: |-
    Partially update a channel by providing only the fields you want to update. Omitted fields will not be updated. The fields that can be updated are defined in the request body, all other provided fields will be ignored.
    ##### Permissions
    If updating a public channel, `manage_public_channel_members` permission is required. If updating a private channel, `manage_private_channel_members` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idpatch-put-openapi.md
- name: Mattermost API Reference - Delete a channel
  x-api-slug: channelschannel-id-delete
  description: |-
    Soft deletes a channel, by marking the channel as deleted in the database. Soft deleted channels will not be accessible in the user interface.
    ##### Permissions
    `delete_public_channel` permission if the channel is public,
    `delete_private_channel` permission if the channel is private,
    or have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-delete-openapi.md
- name: Mattermost API Reference - Update a channel
  x-api-slug: channelschannel-id-put
  description: |-
    Update a channel. The fields that can be updated are listed as paramters. Omitted fields will be treated as blanks.
    ##### Permissions
    If updating a public channel, `manage_public_channel_members` permission is required. If updating a private channel, `manage_private_channel_members` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-put-openapi.md
- name: Mattermost API Reference - Get a channel
  x-api-slug: channelschannel-id-get
  description: |-
    Get channel from the provided channel id string.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-id-get-openapi.md
- name: Mattermost API Reference - Create a group message channel
  x-api-slug: channelsgroup-post
  description: |-
    Create a new group message channel to group of users. If the logged in user's id is not included in the list, it will be appended to the end.
    ##### Permissions
    Must have `create_group_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsgroup-post-openapi.md
- name: Mattermost API Reference - Create a direct message channel
  x-api-slug: channelsdirect-post
  description: |-
    Create a new direct message channel between two users.
    ##### Permissions
    Must be one of the two users and have `create_direct_channel` permission. Having the `manage_system` permission voids the previous requirements.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelsdirect-post-openapi.md
- name: Mattermost API Reference - Create a channel
  x-api-slug: channels-post
  description: |-
    Create a new channel.
    ##### Permissions
    If creating a public channel, `create_public_channel` permission is required. If creating a private channel, `create_private_channel` permission is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channels-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://matrix.api.gallery.streamdata.io
- type: x-api-stack
  url: http://mattermost.stack.network
- type: x-blog
  url: https://about.mattermost.com/blog/
- type: x-blog-rss
  url: https://about.mattermost.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/mattermost
- type: x-developer
  url: https://api.mattermost.com/
- type: x-github
  url: https://github.com/mattermost
- type: x-pricing
  url: https://about.mattermost.com/pricing/
- type: x-security
  url: https://docs.mattermost.com/overview/security.html
- type: x-twitter
  url: https://twitter.com/mattermosthq
- type: x-website
  url: https://mattermost.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---