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
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/apis.md
specificationVersion: "0.14"
apis:
- name: Mattermost API Get a list of channels by ids
  x-api-slug: mattermost-api
  description: |-
    Get a list of public channels on a team by id.
    ##### Permissions
    `view_team` for the team the channels are on.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//teams/{team_id}/channels/ids
  tags: List,Of,Channels,By,Ids
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsids-post-openapi.md
- name: Mattermost API Get a channels pinned posts
  x-api-slug: mattermost-api
  description: Get a list of pinned posts for channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//channels/{channel_id}/pinned
  tags: Channels,Pinned,Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/channelschannel-idpinned-get-openapi.md
- name: Mattermost API Get public channels
  x-api-slug: mattermost-api
  description: |-
    Get a page of public channels on a team based on query string parameters - page and per_page.
    ##### Permissions
    Must be authenticated and have the `list_team_channels` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//teams/{team_id}/channels
  tags: Public,Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannels-get-openapi.md
- name: Mattermost API Get deleted channels
  x-api-slug: mattermost-api
  description: |-
    Get a page of deleted channels on a team based on query string parameters - team_id, page and per_page.

    __Minimum server version__: 3.10

    ##### Permissions
    Must be authenticated and have the `manage_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//teams/{team_id}/channels/deleted
  tags: Deleted,Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsdeleted-get-openapi.md
- name: Mattermost API Autocomplete channels
  x-api-slug: mattermost-api
  description: |-
    Autocomplete public channels on a team based on the search term provided in the request URL.

    __Minimum server version__: 4.7

    ##### Permissions
    Must have the `list_team_channels` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//teams/{team_id}/channels/autocomplete
  tags: Autocomplete,Channels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelsautocomplete-get-openapi.md
- name: Mattermost API Search channels
  x-api-slug: mattermost-api
  description: |-
    Search public channels on a team based on the search term provided in the request body.
    ##### Permissions
    Must have the `list_team_channels` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//teams/{team_id}/channels/search
  tags: Search,Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/teamsteam-idchannelssearch-post-openapi.md
- name: Mattermost API Get channels for user
  x-api-slug: mattermost-api
  description: |-
    Get all the channels on a team for a user.
    ##### Permissions
    Logged in as the user, or have `edit_other_users` permission, and `view_team` permission for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/teams/{team_id}/channels
  tags: Channelsuser
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/usersuser-idteamsteam-idchannels-get-openapi.md
- name: Mattermost API
  x-api-slug: mattermost-api
  description: Open source, private cloud Slack-alternative, Workplace messaging for
    web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
    configurable, and scalable from teams to the enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/mattermost/openapi.md
x-common:
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